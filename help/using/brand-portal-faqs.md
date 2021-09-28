---
title: 常见问题解答
seo-title: null
description: 深入了解Adobe Experience Manager Assets Brand Portal中的常见问题。
seo-description: null
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 4a8f7fbd-7485-421d-a8db-755324d2dbef
source-git-commit: d7dbf9ae2d27dda2edb60d8f861e618fb6332ec7
workflow-type: tm+mt
source-wordcount: '1480'
ht-degree: 1%

---

# 常见问题解答 {#frequently-asked-questions}

Brand Portal常见问题解答主要介绍最终用户在使用最新的AEM Assets Brand Portal 6.4.6版本或更早版本时可能遇到的查询和问题。


## Brand Portal 6.4.6常见问题解答  {#faqs-bp646}

**是的。现有旧版OAuth端点(`https://legacy-oauth.cloud.adobe.io/login`)不起作用。 可能的原因是什么？**

**安。** 已弃用旧版OAuth配置。您必须将AEM Assets创作实例升级到最新的Service Pack，并通过Adobe开发人员控制台对其进行配置。 有关详细信息，请参阅[使用Brand Portal配置AEM Assets](configure-aem-assets-with-brand-portal.md)。 但是，要使旧版OAuth配置在升级之前一直有效，请将旧版OAuth端点更新为`https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`。

<!--
**Ques. I have created a collection using the asset link shared by the administrator. But I am unable to create a share link for my collection. Do I need special permissions to do this?**

**Ans.** The functionality is by design, the viewer users are not permitted to share link for collections as they have limited privileges due to which they cannot add users to create a share link. It is a known issue that the share link for collections is currently visible to the viewer users. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.    
-->

**是的。升级到“Adobe开发人员控制台”后，我无法将贡献文件夹的资产从Brand Portal发布到AEM Assets。 我的创作实例位于AEM 6.5.4上。原因可能是什么？**

**安。** 是，在AEM 6.5.4上通过Adobe开发人员控制台将贡献文件夹的资产发布到AEM Assets时，出现已知问题。

此问题已在AEM 6.5.5中修复。您可以将AEM Assets实例升级到最新的Service Pack AEM 6.5.5，并在Adobe开发人员控制台上[升级您的配置。](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65)

<!--
Broken link of download hotfix, comment out this section until we have the latest URL.

For immediate fix on AEM 6.5.4, it is recommended to [download the hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) and install on your AEM author instance.
-->

**是的。我在AEM Assets中看不到从Brand Portal发布的贡献文件夹内容。 可能的原因是什么？**

**安。** 请联系AEM Assets管理员以验证配置，并确保您的Brand Portal租户仅配置了一个AEM Assets创作实例。

当您在多个Brand Portal创作实例上配置了AEM Assets租户时，可能会出现此问题。 例如，管理员在暂存和生产环境的AEM Assets创作实例上配置相同的Brand Portal租户。 在这种情况下，资产发布会在Brand Portal中触发，但AEM Assets创作实例无法导入资产，因为复制代理未收到请求令牌。


**是的。我无法将资产从AEM Assets发布到Brand Portal。 复制日志指示连接超时。 是否有快速修复？**

**安。** 如果复制队列中存在多个待处理请求，发布通常会失败并出现超时错误。要解决此问题，请确保将复制代理配置为避免超时。

请执行以下步骤以配置复制代理：

1. 登录到您的AEM Assets创作实例。
1. 从&#x200B;**工具**&#x200B;面板中，导航到&#x200B;**[!UICONTROL 部署]** > **[!UICONTROL 复制]**。
1. 在“复制”页中，单击&#x200B;**[!UICONTROL 创作代理]**。 您可以看到Brand Portal租户的四个复制代理。
1. 单击复制代理URL以打开代理详细信息。
1. 单击&#x200B;**[!UICONTROL 编辑]**&#x200B;以修改复制代理设置。
1. 在“代理设置”中，单击&#x200B;**[!UICONTROL Extended]**&#x200B;选项卡。
1. 选中&#x200B;**[!UICONTROL 关闭连接]**&#x200B;复选框。
1. 重复步骤4至7以配置所有四个复制代理。
1. 重新启动服务器并验证连接。


## Brand Portal 6.4.5常见问题解答  {#faqs-bp645}

**是的。Brand Portal 6.4.5版本中有哪些主要更改？**

**安。** AEM Assets Brand Portal 6.4.5是一个功能版本，该版本允许Brand Portal用户从Brand Portal实例内上传内容，并将Contribution文件夹发布回AEM Assets，而无需管理员权限。有关更多信息，请参阅Brand Portal中的[资产源](brand-portal-asset-sourcing.md)。



**是的。我是否会失去对已创建的任何现有资产、功能或配置的访问权限？**

**安。** 您的所有现有功能和配置均保持不变。您的最终用户不会受到影响，您的内容将保持不变。



**是的。我何时要迁移到新版Brand Portal?**

**安。** Brand Portal 6.4.5已于2019年10月发布生产。下一个Brand Portal版本预计将于2020年第3季度发布。
对于更新和版本更改，建议跟踪[发行说明](brand-portal-release-notes.md)和[Brand Portal的新增功能](whats-new.md)。



**是的。我的用户会受到影响吗？**

**安。** Brand Portal 6.4.5版本仅在Brand Portal中发行，因此对最终用户没有影响。



**是的。作为Brand Portal用户，我是否需要执行任何操作？**

**安。** Brand Portal 6.4.5版本附带了名为“资产源”的新功能。AEM管理员必须在AEM Assets中配置资产源功能，才能为Brand Portal用户启用该功能。 有关更多信息，请参阅[启用资产源](brand-portal-asset-sourcing.md)。



**是的。谁可以创建Contribution文件夹？**

**安。** 任何AEM用户有权在AEM Assets中创建新文件夹，都可以创建Contribution文 **** 件夹。要创建&#x200B;**Contribution**&#x200B;文件夹，请创建类型为&#x200B;**Asset Contribution**的新文件夹。
此文件夹将与活动的Brand Portal用户共享以供贡献。



**是的。Contribution文件夹包含什么？**

**安。** **** Contribution文件夹包含两个新建和共 **** 享 **的子文件夹**。最初，NEW文件夹为空，并且SHARED文件夹包含Brand Portal用户的引用内容（可重用资产）。
Brand Portal用户访问**Contribution**&#x200B;文件夹，并上传&#x200B;**NEW**&#x200B;文件夹中的内容。



**是的。我是否可以修改现有Contribution文件夹的名称？**

**安。** **否**，您无法修改现有Contribution文件夹的名 **** 称。



**是的。w.r.t贡献的资产要求是什么？**

**安。** 附加 **** 到Contribution文件夹的简 **** 要文档以及SHARED文件夹中上传的参考内容（可重用资产），可 **** 帮助Brand Portal用户了解作为贡献者的贡献和期望需求，并统称为资产要求。



**是的。我能否将资产上传到任何允许的文件夹？**

**安。** 并非所有允许的文件夹。Brand Portal用户只能将内容上传到AEM或Brand Portal管理员共享的&#x200B;**Contribution**&#x200B;文件夹。



**是的。如何访问Contribution文件夹？**

**安。** 只有与您共 **** 享了Contribution文件夹，才能访问该文件夹。每当与您共享贡献文件夹时，您都会收到电子邮件/脉冲通知。 您可以通过电子邮件中共享的链接访问Contribution文件夹，或登录到Brand Portal实例，然后导航到铃铛图标以获取相关说明，以访问Contribution文件夹。

>[!NOTE]
>
>如果您不是现有的Brand Portal用户，请请求AEM管理员在AEM Admin Console中创建您的用户，并将您的配置文件添加到Brand Portal用户列表的用户配置文件中。

**是的。用户导入的CSV文件格式是什么？**

**安。** 格式与批量用户导入Admin Console支持的格式相同。电子邮件、名字和姓氏是必填项。



**是的。“资产贡献用户”下拉列表中填充了哪些用户(Brand Portal参与者)列表？**

**安。** 下拉菜单中的用户是从AEM中上传的Brand Portal用户配置(.csv)文件填充的。



**是的。在哪里可以看到导入和发布作业的状态？**

**安。** 在AEM中，您可以在异步作业页面中查看导入 **** 的状态。在Brand Portal中，您可以在&#x200B;**[!UICONTROL 工具>资产贡献状态]**&#x200B;中查看发布作业的状态。



**是的。在AEM中定期运行的导入作业的频率是多少？**

**安。** 在AEM中，轮询每5分钟运行一次。



**是的。文件夹可以从Brand Portal发布到AEM Assets的次数是否存在任何原因？**

**安。** 不会，NEWfolder中的所有资 **** 产都会发布到AEM Assets，而不考虑它们之前发布的事实。每次将&#x200B;**Contribution**&#x200B;文件夹从Brand Portal发布到AEM Assets时，它都会覆盖&#x200B;**NEW**&#x200B;文件夹的内容。



**是的。如何在Contribution文件夹中上传新资产？**

**安。** 请参阅将资产上传到 [贡献文件夹](brand-portal-publish-contribution-folder-to-brand-portal.md)的详细文档。



**是的。我看不到Brand Portal用户上传到NEW文件夹的资产的缩略图/预览？**

**安。** 它按照设计要求运行，因此Brand Portal端没有运行工作流。



**是的。如果文件夹从AEM Assets发布到Brand Portal的流量中，会发生什么情况？**

**安。** 在AEM中，每次将文件夹发布到Brand Portal时，都会维护日志。发布时，所有未发布到Brand Portal的资产都会放入复制队列。 触发发布作业后添加到文件夹的任何资产都不会发布到Brand Portal。 当AEM用户再次发布文件夹时，只有之前未发布的资产（复制队列中的现有资产）才会发布到Brand Portal。
对于从AEM Assets发布到Brand Portal的任何文件夹以及Contribution文件夹中的SHARED文件夹，均适用此条件。

**是的。我应该与谁联系？**

**安。** 请联系您的Adobe客户经理或客户支持。

>[!NOTE]
>
>发布计划是暂定的，可能会发生更改。 请联系您的Adobe客户经理或客户支持以获取更新的发行计划。


## 产品访问和支持（受限网站） {#product-access-and-support-restricted-sites}

这些网站仅适用于客户。如果您是客户并需要访问，请联系您的Adobe客户经理。

* [](https://daycare.day.com) [产品访问](https://login.marketing.adobe.com)

* [Adobe客户关怀](https://helpx.adobe.com/contact.html)
