---
title: 对并行发布到Brand Portal时出现的问题进行故障诊断
description: 并行发布疑难解答。
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: brand-portal
role: Admin
exl-id: 631beabc-b145-49ba-a8e4-f301497be6da
source-git-commit: ce3a7a5232f32c86b4930f9079bed5f04d001d8f
workflow-type: tm+mt
source-wordcount: '947'
ht-degree: 0%

---

# 对并行发布到Brand Portal时出现的问题进行故障诊断 {#troubleshoot-issues-in-parallel-publishing-to-brand-portal}

Brand Portal通过Experience Manager Assets进行配置，以批准从Experience Manager Assets创作实例中无缝摄取（或发布）Brand Assets。 配置[后](../using/configure-aem-assets-with-brand-portal.md)，Experience Manager作者将使用复制代理将一个或多个选定的资源复制到Brand Portal云服务，以供Brand Portal用户批准使用。 Experience Manager6.2 SP1-CFP5、Experience ManagerCFP 6.3.0.2及更高版本使用了多个复制代理，以允许高速并行发布。

>[!NOTE]
>
>要确保使用Experience Manager Assets成功配置Experience Manager Assets Brand Portal，Adobe建议升级到Experience Manager6.4.1.0。Experience Manager6.4中的限制会在使用Brand Portal配置Experience Manager Assets时出错，并且复制失败。

为&#x200B;**[!UICONTROL /etc/cloudservice]**&#x200B;下的Brand Portal配置云服务时，将自动生成所有必需的用户和令牌并将其保存在存储库中。 创建了云服务配置，还创建了复制和复制代理复制内容所需的服务用户。 它将创建四个复制代理。 因此，当您将Experience Manager中的大量资源发布到Brand Portal时，这些资源会排队并通过Round Robin在复制代理之间分发。

但是，发布可能会间歇性地失败，原因是Sling作业过大、Experience Manager创作实例上的网络和&#x200B;**[!UICONTROL 磁盘I/O]**&#x200B;增加或Experience Manager创作实例的性能降低。 Adobe建议在开始发布之前测试与一个或多个复制代理的连接。

![](assets/test-connection.png)

## 首次发布失败疑难解答：验证发布配置 {#troubleshoot-failures-in-first-time-publishing-validating-your-publish-configuration}

验证发布配置：

1. 检查错误日志
1. 检查是否创建了复制代理
1. 测试连接

创建Cloud Service时&#x200B;**尾日志**

检查尾日志。 检查是否创建了复制代理。 如果复制代理创建失败，请通过在云服务中进行细微更改来编辑云服务。 验证并再次检查是否创建了复制代理。 如果没有，请重新编辑该服务。

如果在反复编辑云服务时未正确配置，则报告Daycare票证。

**测试与复制代理的连接**

查看日志，如果在复制日志中发现错误：

1. 联系客户支持。

1. 重试[清理](../using/troubleshoot-parallel-publishing.md#clean-up-existing-config)并再次创建发布配置。

<!--
Comment Type: remark
Last Modified By: Mini Gulati (mgulati)
Last Modified Date: 2018-06-21T22:56:21.256-0400
<p>?? check and compare public key. At times public key is different</p>
<p>?? another thing to check in /useradmin</p>
-->

## 清理现有Brand Portal发布配置 {#clean-up-existing-config}

发布通常会失败并出现“401未授权”错误，因为用户（例如`mac-<tenantid>-replication`）缺少最新的私钥，并且复制代理日志中未报告任何其他错误。 您可能希望避免进行故障排除，而改为创建配置。 要使新配置正常工作，请从Experience Manager创作设置中清理以下内容：

1. 转到`localhost:4502/crx/de/` （考虑到您正在`localhost:4502:`上运行创作实例）
i.删除`/etc/replication/agents.author/mp_replication`
二、 删除`/etc/cloudservices/mediaportal/<config_name>`

1. 转到localhost：4502/useradmin：\
   i.搜索用户`mac-<tenantid>replication`
二、 删除此用户

现在，系统已全部清理。 现在，您可以尝试创建云服务配置，并且仍使用现有的JWT应用程序。 无需创建应用程序，只需从新创建的云配置中更新公钥即可。

>[!NOTE]
>
>请勿修改任何自动生成的设置。


## 开发人员连接JWT应用程序租户可见性问题 {#developer-connection-jwt-application-tenant-visibility-issue}

如果在`https://legacy-oauth.cloud.adobe.io/`，则列出当前用户拥有系统管理员的所有组织（租户）。 如果您在此处找不到组织名称，或者您在此处无法为所需的租户创建应用程序，请检查您是否有足够的（系统管理员）权限。

此用户界面存在一个已知问题，即对于任何租户，只有前十个应用程序可见。 创建应用程序时，请停留在页面上并将URL加入书签。 不要转到应用程序的列表页并找到您创建的应用程序。 您可以直接点击此已添加书签的URL，并在需要时更新或删除应用程序。

可能未正确列出JWT应用程序。 因此，建议您在创建JWT应用程序时记下或将URL加入书签。

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

如果复制代理(可以正常发布到Brand Portal)停止处理发布作业，请检查复制日志。 Experience Manager内置了自动重试功能，因此，如果特定资源发布失败，则会自动重试该资源。 如果存在网络错误等间歇性问题，则在重试期间可能会成功。

如果连续发布失败，并且队列被阻止，请检查&#x200B;**[!UICONTROL 测试连接]**。 尝试解决正在报告的错误。

根据错误，建议您记录支持工单，以便Brand Portal工程团队可以帮助您解决问题。

## Brand Portal IMS配置令牌已过期 {#token-expired}

如果您的Brand Portal环境突然停止，IMS配置可能会无法正常运行。 系统显示不正常的IMS配置，并反映您的访问令牌已过期的错误消息（类似于以下内容）。

`com.adobe.granite.auth.oauth.AccessTokenProvider failed to get access token from authorization server status: 400 response: Unknown macro: {"error"}`

要解决此问题，Adobe建议您手动保存并关闭IMS配置，然后再次检查运行状况状态。 如果配置不起作用，请删除现有配置并创建新配置。


## 配置复制代理以避免连接超时错误 {#connection-timeout}

通常，如果复制队列中有多个挂起的请求，发布作业会失败并出现超时错误。 要解决此问题，请确保将复制代理配置为避免超时。

要配置复制代理，请执行以下操作：

1. 登录到您的AEM Assets创作实例。
1. 从&#x200B;**工具**&#x200B;面板，导航到&#x200B;**[!UICONTROL 部署]** > **[!UICONTROL 复制]**。
1. 在“复制”页面中，单击&#x200B;**[!UICONTROL `Agents on author`]**。 您可以看到Brand Portal租户的四个复制代理。
1. 单击复制代理URL，然后单击&#x200B;**[!UICONTROL 编辑]**。
1. 在“代理设置”中，单击&#x200B;**[!UICONTROL 扩展]**&#x200B;选项卡。
1. 选中&#x200B;**[!UICONTROL 关闭连接]**&#x200B;复选框。
1. 重复步骤4至7以配置所有四个复制代理。
1. 重新启动服务器。
