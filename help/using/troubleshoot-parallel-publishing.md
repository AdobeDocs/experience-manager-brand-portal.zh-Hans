---
title: 解决并行发布到Brand Portal的问题
seo-title: 解决并行发布到Brand Portal的问题
description: 并行发布疑难解答。
seo-description: 并行发布疑难解答。
uuid: 51e45cca-8c96-4c69-84ef-2ef34f3bcde2
products: SG_ EXPERIENCE MANAGER/Brand_ Portal
content-type: 引用
topic-tags: 品牌门户
discoiquuid: a4801024-b509-4c51-afd8-e337417 e658 b
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# 解决并行发布到Brand Portal的问题 {#troubleshoot-issues-in-parallel-publishing-to-brand-portal}

Brand Portal支持与AEM Assets集成，以便在AEM资产作者实例中无缝摄取(或发布)已批准的品牌资产。[集成](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html)后，AEM作者会使用复制代理将选定资源复制到Brand Portal云服务以获得Brand Portal用户批准的使用。多个复制代理使用AEM6.2SP1-CFP5]、AEM CFP6.3.0.2及自定义，以允许高速并行发布。

>[!NOTE]
>
>Adobe建议升级到AEM6.4.1.0以确保AEM Assets Brand Portal与AEM Assets成功集成。AEM6.4限制了在配置与Brand Portal集成的同时出错，而且复制失败。

在为/etc/cloudservice下 [!UICONTROL 的品牌门户配置云服务时]，所有必需的用户和令牌都是自动生成的并保存在存储库中。创建云服务配置，同时创建复制和复制代理所需的服务用户以复制内容。这将创建四个复制代理。因此，当您将大量资源从AEM发布到Brand Portal时，这些资源将在这些复制代理之间排队并通过Root Robin分发。

但是，由于较大的sling作业、在AEM作者实例上增加的网络和 [!UICONTROL 磁盘I/O] 以及AEM Author实例的性能降低，发布可能会失败。因此，建议在开始发布之前测试与复制代理的连接。

![](assets/test-connection.png)

## 首次发布故障诊断失败：验证发布配置 {#troubleshoot-failures-in-first-time-publishing-validating-your-publish-configuration}

验证发布配置：

1. 检查错误日志
2. 检查复制代理是否创建
3. 测试连接

**创建云服务时的尾部日志**

检查尾部日志。检查是否创建复制代理。如果复制代理创建失败，请在云服务中进行少量更改以编辑云服务。验证和检查是否创建了复制代理。否则，请重新编辑服务。

如果在多次编辑云服务时无法正确配置，请报告日托票。

**测试与复制代理的连接**

查看日志(如果在复制日志中发现错误)：

1. 联系Adobe支持。

2. 再次尝试 [清理](../using/troubleshoot-parallel-publishing.md#clean-up-existing-config) 并再次创建发布配置。

<!--
Comment Type: remark
Last Modified By: Mini Gulati (mgulati)
Last Modified Date: 2018-06-21T22:56:21.256-0400
<p>?? check and compare public key. At times public key is different</p>
<p>?? another thing to check in /useradmin</p>
-->

### 清理现有的Brand Portal发布配置 {#clean-up-existing-config}

大多数发布不起作用的情况下，其原因可能是要发布的用户(例如： [!UICONTROL mac-&lt; tenand&gt;-复制])没有最新私钥，因此发布失败，“401未授权”错误，并且复制代理日志中没有报告其他错误。您可能希望避免故障排除并改为创建新配置。为使新配置正常工作，请从AEM创作设置中清除以下内容：

1. 转到 [!UICONTROL localhost：4502/crx/de] (考虑在localhost上 [!UICONTROL 运行作者实例：4502])：\
   i. 删除/etc/replication/agents.author/mp_replication*\
   ii. 删除/etc/cloudservices/mediaportal/&lt; config_ name&gt;

2. 转到 [!UICONTROL localhost：4502/usermin]：\
   i搜索用户[！UICONTRL mac-&lt; tenand&gt;-copy
ii删除此用户

现在系统已清理完毕。现在，您可以尝试创建一个新的云服务配置，并且仍然在 [https://legacy-oauth.cloud.adobe.io/中使用现有的JWT应用程序](https://legacy-oauth.cloud.adobe.io/)。无需创建新的应用程序，而只需要从新创建的云配置更新公钥。

## 开发人员连接JWT应用程序租户可见性问题 {#developer-connection-jwt-application-tenant-visibility-issue}

如果在 [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/)上，则列出当前用户持有系统管理员的所有组织(租户)。如果在此处找不到org名称，或者无法在此处为必需租户创建应用程序，请检查您是否拥有足够的权限(系统管理员)。

此用户界面上存在一个已知问题，该问题仅适用于任何租户，才可见。创建应用程序时，请保留该页面并将URL书签。您无需转到应用程序的列表页面并找到您创建的应用程序。您可以直接点击此书签URL，并根据需要更新/删除应用程序。

JWT应用程序可能无法正确列出。因此，建议在创建JWT应用程序时记下/标记URL。

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

如果复制代理(刚刚发布到品牌门户)停止处理发布作业，请检查复制日志。AEM已自动重新尝试内置，因此如果某个特定资源发布失败，将自动重试它。如果某些间歇性问题如网络错误，在重试期间可能会成功。

如果存在连续发布失败和队列被阻止的情况，则应检查 **[!UICONTROL 测试连接]** 并尝试解决正在报告的错误。

根据错误，建议您记录支持票证，这样Brand Portal工程师团队可以帮助您解决问题。
