---
title: 对并行发布到 Brand Portal 时出现的问题进行故障诊断
seo-title: Troubleshoot issues in parallel publishing to Brand Portal
description: 并行发布故障诊断。
seo-description: Troubleshoot parallel publishing.
uuid: 51e45cca-8c96-4c69-84ef-2ef34f3bcde2
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: brand-portal
discoiquuid: a4801024-b509-4c51-afd8-e337417e658b
role: Admin
exl-id: 631beabc-b145-49ba-a8e4-f301497be6da
source-git-commit: 72cd0ebbf05067287d94e1dc4e1b68f5fb6c2888
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 1%

---

# 对并行发布到 Brand Portal 时出现的问题进行故障诊断 {#troubleshoot-issues-in-parallel-publishing-to-brand-portal}

Brand Portal已使用Experience Manager Assets进行配置，以便能够从Experience Manager Assets创作实例无缝摄取（或发布）已批准的品牌资产。 一次 [已配置](../using/configure-aem-assets-with-brand-portal.md)，则Experience Manager作者会使用复制代理将选定的资产复制到Brand Portal云服务，以供Brand Portal用户使用。 Experience Manager6.2 SP1-CFP5、Experience ManagerCFP 6.3.0.2及以上版本使用多个复制代理，以允许高速并行发布。

>[!NOTE]
>
>Adobe建议升级到Experience Manager6.4.1.0，以确保已成功配置Experience Manager Assets Brand Portal。 Experience Manager6.4中的限制在使用Brand Portal配置Experience Manager Assets时出错，并且复制失败。

关于为Brand Portal配置云服务，请在 **[!UICONTROL /etc/cloudservice]**，所有必需的用户和令牌都将自动生成并保存在存储库中。 云服务配置已创建，复制代理和复制代理复制内容所需的服务用户也已创建。 它创建四个复制代理。 因此，当您将大量资产从Experience Manager发布到Brand Portal时，这些资产将通过轮询在复制代理之间排队和分发。

但是，发布可能会因为大型sling作业、网络增加和 **[!UICONTROL 磁盘I/O]** ，或者减慢了Experience Manager创作实例的性能。 因此，建议在开始发布之前测试与复制代理的连接。

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

1. 联系客户支持。

1. 重试 [清理](../using/troubleshoot-parallel-publishing.md#clean-up-existing-config) 并再次创建发布配置。

<!--
Comment Type: remark
Last Modified By: Mini Gulati (mgulati)
Last Modified Date: 2018-06-21T22:56:21.256-0400
<p>?? check and compare public key. At times public key is different</p>
<p>?? another thing to check in /useradmin</p>
-->

## 清理现有Brand Portal发布配置 {#clean-up-existing-config}

大多数情况下，发布不起作用，原因可能是正在发布的用户(例如： `mac-<tenantid>-replication` 没有最新的私钥，因此发布失败，出现“401未授权”错误，并且复制代理日志中未报告任何其他错误。 您可能希望避免进行故障诊断，而改为创建配置。 要使新配置正常工作，请从Experience Manager作者设置中清除以下内容：

1. 转到 `localhost:4502/crx/de/` (考虑您在localhost上运行创作实例:4502:\
   i.删除 `/etc/replication/agents.author/mp_replication`
ii. 删除 
`/etc/cloudservices/mediaportal/<config_name>`

1. 转到localhost:4502/useradmin:\
   i.搜索用户 `mac-<tenantid>replication`
ii. 删除此用户

现在系统已全部清理完毕。 现在，您可以尝试创建云服务配置，并仍然使用现有的JWT应用程序。 无需创建应用程序，而是从新创建的云配置中更新公钥。

>[!NOTE]
>
>请勿修改任何自动生成的设置。


## 开发人员连接JWT应用程序租户可见性问题 {#developer-connection-jwt-application-tenant-visibility-issue}

如果开启 `https://legacy-oauth.cloud.adobe.io/`，将列出当前用户持有系统管理员的所有组织（租户）。 如果您在此处找不到组织名称，或者无法在此处为所需租户创建应用程序，请检查您是否具有足够的（系统管理员）权限。

此用户界面上存在一个已知问题，即对于任何租户，只显示前十个应用程序。 创建应用程序时，请停留在该页面上，并为URL添加书签。 您无需转到应用程序的列表页面，并找到您创建的应用程序。 您可以直接点击此标为书签的URL，并根据需要更新/删除应用程序。

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

如果复制代理(刚刚发布到Brand Portal)停止处理发布作业，请检查复制日志。 Experience Manager具有自动重试内置功能，因此，如果特定资产发布失败，则会自动重试。 如果出现网络错误等间歇性问题，则在重试期间可能会成功。

如果连续发布失败并阻止队列，则应检查 **[!UICONTROL 测试连接]** 并尝试解决所报告的错误。

根据错误，建议您记录支持票证，以便Brand Portal工程团队可以帮助您解决问题。

## Brand Portal IMS配置令牌已过期 {#token-expired}

如果您的Brand Portal环境突然停止，则可能IMS配置无法正常运行。 系统会显示不正常的IMS配置，并反映出一条错误消息（类似于以下内容），指出您的访问令牌已过期。

`com.adobe.granite.auth.oauth.AccessTokenProvider failed to get access token from authorization server status: 400 response: Unknown macro: {"error"}`

要解决此问题，建议手动保存并关闭IMS配置，并再次检查运行状况状态。 如果配置不起作用，请删除现有配置并创建新配置。


## 配置复制代理以避免连接超时错误 {#connection-timeout}

如果复制队列中存在多个待处理请求，则发布作业通常会失败并出现超时错误。 要解决此问题，请确保将复制代理配置为避免超时。

要配置复制代理，请执行以下操作：

1. 登录到您的AEM Assets创作实例。
1. 从 **工具** 面板，导航到 **[!UICONTROL 部署]** > **[!UICONTROL 复制]**.
1. 在复制页面中，单击 **[!UICONTROL 作者代理]**. 您可以看到Brand Portal租户的四个复制代理。
1. 单击复制代理URL，然后单击 **[!UICONTROL 编辑]**.
1. 在代理设置中，单击 **[!UICONTROL 扩展]** 选项卡。
1. 选择 **[!UICONTROL 关闭连接]** 复选框。
1. 重复步骤4至7以配置所有四个复制代理。
1. 重新启动服务器。
