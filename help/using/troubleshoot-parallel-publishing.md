---
title: 对并行发布到 Brand Portal 时出现的问题进行故障诊断
seo-title: 对并行发布到 Brand Portal 时出现的问题进行故障诊断
description: 并行发布故障诊断。
seo-description: 并行发布故障诊断。
uuid: 51e45cca-8c96-4c69-84ef-2ef34f3bcde2
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: brand-portal
discoiquuid: a4801024-b509-4c51-afd8-e337417e658b
role: Admin
exl-id: 631beabc-b145-49ba-a8e4-f301497be6da
source-git-commit: 22104bff436b432e2198bd770f1f39d5c4350518
workflow-type: tm+mt
source-wordcount: '884'
ht-degree: 2%

---

# 对并行发布到 Brand Portal 时出现的问题进行故障诊断 {#troubleshoot-issues-in-parallel-publishing-to-brand-portal}

Brand Portal已使用AEM Assets进行配置，以便能够从AEM Assets创作实例无缝摄取（或发布）已批准的品牌资产。 配置[](../using/configure-aem-assets-with-brand-portal.md)后，AEM作者会使用复制代理将选定的资产复制到Brand Portal云服务，以供Brand Portal用户批准使用。 AEM 6.2 SP1-CFP5、AEM CFP 6.3.0.2及以上版本使用了多个复制代理，以允许高速并行发布。

>[!NOTE]
>
>Adobe建议升级到AEM 6.4.1.0，以确保已成功使用AEM Assets配置AEM Assets Brand Portal。 AEM 6.4中的限制在使用Brand Portal配置AEM Assets时出错，并且复制失败。

在&#x200B;**[!UICONTROL /etc/cloudservice]**&#x200B;下为brand portal配置云服务时，将自动生成所有必需的用户和令牌并将其保存在存储库中。 云服务配置已创建，复制代理和复制代理复制内容所需的服务用户也已创建。 这会创建四个复制代理。 因此，当您将大量资产从AEM发布到Brand Portal时，这些资产会通过Round Robin排队并分发到这些复制代理中。

但是，发布可能会间歇性失败，原因是：AEM创作实例上存在大型sling作业、增加了网络和&#x200B;**[!UICONTROL 磁盘I/O]**，或者降低了AEM创作实例的性能。 因此，建议在开始发布之前测试与复制代理的连接。

![](assets/test-connection.png)

## 首次发布失败故障诊断：验证发布配置 {#troubleshoot-failures-in-first-time-publishing-validating-your-publish-configuration}

要验证发布配置，请执行以下操作：

1. 检查错误日志
1. 检查复制代理是否已创建
1. 测试连接

**创建尾日志时Cloud Service**

检查尾日志。 检查是否创建了复制代理。 如果复制代理创建失败，请通过在云服务中进行细微更改来编辑云服务。 验证并再次检查是否创建了复制代理。 如果没有，请重新编辑服务。

如果重复编辑云服务时配置不正确，请报告日托票证。

**测试与复制代理的连接**

查看日志（如果在复制日志中发现错误）：

1. 联系Adobe支持。

1. 重试[清理](../using/troubleshoot-parallel-publishing.md#clean-up-existing-config)，然后再次创建发布配置。

<!--
Comment Type: remark
Last Modified By: Mini Gulati (mgulati)
Last Modified Date: 2018-06-21T22:56:21.256-0400
<p>?? check and compare public key. At times public key is different</p>
<p>?? another thing to check in /useradmin</p>
-->

### 清理现有Brand Portal发布配置 {#clean-up-existing-config}

大多数情况下，发布不起作用，原因可能是正在发布的用户(例如：`mac-<tenantid>-replication`没有最新的私钥，因此发布失败，出现“401 unauthorized”错误，并且复制代理日志中未报告任何其他错误。 您可能希望避免疑难解答，而是创建新配置。 要使新配置正常工作，请从AEM创作设置中清除以下内容：

1. 转到`localhost:4502/crx/de/`（考虑到您正在localhost:4502:上运行创作实例）\
   i.删除`/etc/replication/agents.author/mp_replication`
ii. 删除 
`/etc/cloudservices/mediaportal/<config_name>`

1. 转到localhost:4502/useradmin:\
   i.搜索用户`mac-<tenantid>replication`
ii. 删除此用户

现在系统已全部清理完毕。 现在，您可以尝试创建新的cloudservice配置，并仍使用`https://legacy-oauth.cloud.adobe.io/`中已有的JWT应用程序。 无需创建新应用程序，而只需从新创建的云配置中更新公共密钥。

## 开发人员连接JWT应用程序租户可见性问题 {#developer-connection-jwt-application-tenant-visibility-issue}

如果在`https://legacy-oauth.cloud.adobe.io/`上，则列出当前用户持有系统管理员的所有组织（租户）。 如果您在此处找不到组织名称，或者无法在此处为所需租户创建应用程序，请检查您是否具有足够的（系统管理员）权限来执行此操作。

此用户界面上存在一个已知问题，即对于任何租户，仅显示前10个应用程序。 创建应用程序时，请停留在该页面上，并为URL添加书签。 您无需转到应用程序的列表页面，并找到您创建的应用程序。 您可以直接点击此标为书签的URL，并根据需要更新/删除应用程序。

JWT应用程序可能未正确列出。 因此，建议在创建JWT应用程序时记下URL/为其添加书签。

## 运行配置停止工作 {#running-configuration-stops-working}

<!--
Comment Type: draft

<p>If the running configuration stops working, either of the following two possibilities
<g class="gr_ gr_15 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar multiReplace" data-gr-id="15" id="15" style="font-size: 12px;">
are
</g> there:</p>
<p>1.
<g class="gr_ gr_14 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar only-ins doubleReplace replaceWithoutSep" data-gr-id="14" id="14">
Connection
</g> has failed, or</p>
<p>2. Publish has failed with permission to dam-replication-service denied, while connection has passed </p>
<p>If the connection has failed [1], the
<g class="gr_ gr_10 gr-alert gr_spell gr_inline_cards gr_run_anim ContextualSpelling ins-del multiReplace" data-gr-id="10" id="10">
fail safe
</g> way to fix it is to <a href="../using/troubleshoot-parallel-publishing.md#main-pars-header-1664955658">clean up</a> the existing Brand Portal publish configuration and recreate a publish configuration. </p>
<p>However, if the
<g class="gr_ gr_18 gr-alert gr_spell gr_inline_cards gr_run_anim ContextualSpelling" data-gr-id="18" id="18">
publish
</g> has failed with
<g class="gr_ gr_16 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar only-ins doubleReplace replaceWithoutSep" data-gr-id="16" id="16">
permission
</g> denied to dam-replication-service, raise a support ticket.</p>
-->

如果复制代理（刚刚发布到brand portal）停止处理发布作业，请检查复制日志。 AEM具有自动重试内置功能，因此，如果特定资产发布失败，则会自动重试。 如果出现网络错误等间歇性问题，则在重试期间可能会成功。

如果连续发布失败且队列被阻止，则应检查&#x200B;**[!UICONTROL 测试连接]**&#x200B;并尝试解决正在报告的错误。

根据错误，建议您记录支持票证，以便Brand Portal工程团队可以帮助您解决问题。


## 配置复制代理以避免连接超时错误 {#connection-timeout}

如果复制队列中存在多个待处理请求，则发布作业通常会失败并出现超时错误。 要解决此问题，请确保将复制代理配置为避免超时。

请执行以下步骤以配置复制代理：
1. 登录到您的AEM Assets创作实例。
1. 从&#x200B;**工具**&#x200B;面板中，导航到&#x200B;**[!UICONTROL 部署]** > **[!UICONTROL 复制]**。
1. 在“复制”页中，单击&#x200B;**[!UICONTROL 创作代理]**。 您可以看到Brand Portal租户的四个复制代理。
1. 单击复制代理URL以打开代理详细信息。
1. 单击&#x200B;**[!UICONTROL 编辑]**&#x200B;以修改复制代理设置。
1. 在“代理设置”中，单击&#x200B;**[!UICONTROL Extended]**&#x200B;选项卡。
1. 选中&#x200B;**[!UICONTROL 关闭连接]**&#x200B;复选框。
1. 重复步骤4至7以配置所有四个复制代理。
1. 重新启动服务器。
