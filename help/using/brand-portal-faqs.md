---
title: 常见问题
seo-title: null
description: 深入了解Adobe Experience Manager Assets Brand Portal中的常见问题。
seo-description: null
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 4983e2e160b5cfb213e249f731e1858fab2cf972
workflow-type: tm+mt
source-wordcount: '1516'
ht-degree: 2%

---


# 常见问题 {#frequently-asked-questions}

Brand Portal常见问题解答侧重于最终用户在使用最新的AEM Assets Brand Portal 6.4.6版本或更早版本时可能遇到的查询和问题。


## Brand Portal 6.4.6常见问题解答{#faqs-bp646}

**凯斯。现有旧版OAuth端点(`https://legacy-oauth.cloud.adobe.io/login`)无法工作。 可能的原因是什么？**

**安。** 旧版OAuth配置已弃用。您必须将AEM Assets作者实例升级到最新的Service Pack，并通过Adobe Developer Console进行配置。 有关详细信息，请参阅[配置AEM Assets with Brand Portal](configure-aem-assets-with-brand-portal.md)。 但是，要使旧版OAuth配置在您升级之前正常工作，请将旧版OAuth终结点更新为`https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`。

<!--
**Ques. I have created a collection using the asset link shared by the administrator. But I am unable to create a share link for my collection. Do I need special permissions to do this?**

**Ans.** The functionality is by design, the viewer users are not permitted to share link for collections as they have limited privileges due to which they cannot add users to create a share link. It is a known issue that the share link for collections is currently visible to the viewer users. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.    
-->

**凯斯。升级到Adobe Developer Console后，我无法将贡献文件夹的资产从Brand Portal发布到AEM Assets。 我的作者实例位于AEM 6.5.4上。可能的原因是什么？**

**安。** 是的，通过Adobe开发人员控制台将贡献文件夹的资产发布到AEM 6.5.4上的AEM Assets时出现已知问题。

此问题在AEM 6.5.5中已解决。您可以将AEM Assets实例升级到最新的Service Pack AEM 6.5.5和[升级Adobe开发人员控制台上的配置](https://docs.adobe.com/content/help/zh-Hans/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65)。

对于AEM 6.5.4上的即时修复，建议[下载修补程序](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041)并安装在AEM作者实例上。

**凯斯。我看不到从AEM Assets的Brand Portal发布的贡献文件夹内容。 可能的原因是什么？**

**安。** 请与AEM Assets管理员联系以验证配置并确保您的Brand Portal租户仅配置了一个AEM Assets作者实例。

在多个AEM Assets作者实例上配置Brand Portal租户时，可能会发生此问题。 例如，管理员在AEM Assets的暂存和生产环境的作者实例上配置同一Brand Portal租户。 在这种情况下，资产发布会在Brand Portal中触发，但AEM Assets作者实例无法导入资产coz，复制代理未收到请求令牌。


**凯斯。我无法将资产从AEM Assets发布到Brand Portal。 复制日志表明连接超时。 是否有快速修复？**

**安。** 通常，如果复制队列中有多个挂起请求，则发布会失败并出现超时错误。要解决此问题，请确保将复制代理配置为避免超时。

请执行以下步骤来配置复制代理：
1. 登录到AEM Assets作者实例。
1. 从&#x200B;**工具**&#x200B;面板，导航到&#x200B;**[!UICONTROL 部署]** > **[!UICONTROL 复制]**。
1. 在复制页中，单击作者&#x200B;]**上的**[!UICONTROL &#x200B;代理。 您可以看到Brand Portal租户的四个复制代理。
1. 单击复制代理URL以打开代理详细信息。
1. 单击&#x200B;**[!UICONTROL 编辑]**&#x200B;以修改复制代理设置。
1. 在“代理设置”中，单击&#x200B;**[!UICONTROL Extended]**&#x200B;选项卡。
1. 选中&#x200B;**[!UICONTROL 关闭连接]**&#x200B;复选框。
1. 重复步骤4至7以配置所有四个复制代理。
1. 重新启动服务器并验证连接。


## Brand Portal 6.4.5常见问题解答{#faqs-bp645}

**凯斯。Brand Portal 6.4.5版本中有哪些主要更改？**

**安。** AEM Assets Brand Portal 6.4.5是一个功能版本，它允许Brand Portal用户从Brand Portal实例内上传内容并将贡献文件夹发布回AEM Assets，而无需管理员权限。有关详细信息，请参阅[品牌门户中的资产来源补充](brand-portal-asset-sourcing.md)。



**凯斯。我是否将失去对已创建的任何现有资产、功能或配置的访问权限？**

**安。** 您的所有现有功能和配置均保持不变。您的最终用户不会受到影响，您的内容将保持不变。



**凯斯。我何时要迁移到新版本的Brand Portal?**

**安。** Brand Portal 6.4.5已于2019年10月发布并投入生产。下一个Brand Portal版本预计将于2020年第3季度发布。
对于更新和版本更改，建议跟踪[发行说明](brand-portal-release-notes.md)和[Brand Portal](whats-new.md)中的新增功能。



**凯斯。我的用户是否会受到影响？**

**安。** Brand Portal 6.4.5版本只包含在Brand Portal中，因此不会对您的最终用户产生影响。



**凯斯。作为Brand Portal用户，我是否需要执行任何操作？**

**安。** Brand Portal 6.4.5版本附带一个名为“资产来源补充”的新功能。AEM管理员必须在AEM Assets中配置“资产来源补充”功能，才能为品牌门户用户启用该功能。 有关详细信息，请参阅[启用资产来源补充](brand-portal-asset-sourcing.md)。



**凯斯。谁可以创建贡献文件夹？**

**安。** 任何具有在AEM Assets中创建新文件夹权限的AEM用户都可以创建Contribution文 **** 件夹。要创建&#x200B;**Contribution**&#x200B;文件夹，请新建一个类型为&#x200B;**Asset Contribution**的文件夹。
此文件夹会与活动的Brand Portal用户共享以供贡献。



**凯斯。Contribution文件夹包含什么？**

**安。** **Contribution** 文件夹包含两个子文 **** 件 **夹NEW**。最初，NEW文件夹为空，且SHARED文件夹包含Brand Portal用户的参考内容（可重用资源）。
Brand Portal用户访问**Contribution**&#x200B;文件夹，并上传&#x200B;**NEW**&#x200B;文件夹中的内容。



**凯斯。我是否可以修改现有贡献文件夹的名称？**

**安。** **否**，您无法修改现有Contribution文件夹的 **** 名称。



**凯斯。资产要求w.r.t贡献是什么？**

**安。** 附 **** 加到Contribution文件夹的简 **** 要文档以及SHAREDfolder中上传的参考内容(可重用资 **** 产)可帮助Brand Portal用户了解作为投稿人的贡献和期望的需求，并被统称为资产需求。



**凯斯。是否可以将资产上传到任何允许的文件夹？**

**安。** 并非所有允许的文件夹。Brand Portal用户只能将内容上传到AEM或Brand Portal管理员共享的&#x200B;**Contribution**&#x200B;文件夹。



**凯斯。如何获取对贡献文件夹的访问权限？**

**安。** 只有已与您共 **** 享Contribution文件夹，才能访问它。每次与您共享一个贡献文件夹时，您都会收到电子邮件/脉冲通知。 您可以通过电子邮件中共享的链接访问贡献文件夹，或登录到您的Brand Portal实例，然后导航到铃图标，以便通知您访问贡献文件夹。

>[!NOTE]
>
>如果您不是现有的Brand Portal用户，请请求AEM管理员在AEM管理控制台中创建您的用户，并将用户档案添加到Brand Portal用户列表中的用户配置文件。

**凯斯。用户导入的CSV文件的格式是什么？**

**安。** 格式与批量用户导入Admin Console支持的格式相同。电子邮件、名和姓是必填项。



**凯斯。在“资产贡献”用户下拉列表中填充用户列表（Brand Portal参与者）的内容**

**安。** 下拉列表中的用户将通过AEM中上传的Brand Portal用户配置(.csv)文件进行填充。



**凯斯。在哪里可以看到导入和发布作业的状态？**

**安。** 在AEM中，您可以在异步作业页面中查看导入 **** 的状态。在Brand Portal中，您可以在&#x200B;**[!UICONTROL 工具>资产贡献状态]**&#x200B;中查看发布作业的状态。



**凯斯。在AEM中定期运行的导入作业的频率是多少？**

**安。** 在AEM中，轮询每5分钟运行一次。



**凯斯。文件夹从Brand Portal发布到AEM Assets的次数是否存在任何原因？**

**安。** 否，NEWfolder中的所有资 **** 产都将发布到AEM Assets，而不管它们之前发布的事实如何。每次将&#x200B;**Contribution**&#x200B;文件夹从Brand Portal发布到AEM Assets时，它都会覆盖&#x200B;**NEW**&#x200B;文件夹的内容。



**凯斯。如何上传贡献文件夹中的新资产？**

**安。** 请参阅将资产上传到贡 [献文件夹的详细文档](brand-portal-publish-contribution-folder-to-brand-portal.md)。



**凯斯。我看不到由Brand Portal用户上传到NEW文件夹的资产的缩略图/预览?**

**安。** 它按照设计，coz没有在Brand Portal端运行工作流。



**凯斯。如果文件夹从AEM Assets发布到正在流量中的Brand Portal，会发生什么情况？**

**安。** 在AEM中，每次将文件夹发布到Brand Portal时都会保留日志。在发布时，所有未发布到Brand Portal的资产都将放在复制队列中。 触发发布作业后添加到文件夹的任何资产都不会发布到Brand Portal。 当AEM用户再次发布文件夹时，只有之前未发布的资产（在复制队列中存在）才会发布到Brand Portal。
对于从AEM Assets发布到Brand Portal的任何文件夹以及贡献文件夹中的SHARED文件夹，此情况均适用。

**凯斯。如有疑问，应与谁联系？**

**安。** 联系您的Adobe客户经理或客户支持。

>[!NOTE]
>
>释放计划是试探性的，可能会有变化。 请联系您的Adobe客户经理或客户支持以获取更新的发行计划。


## 产品访问和支持（受限站点）{#product-access-and-support-restricted-sites}

这些网站仅适用于客户。如果您是Adobe并需要访问，请与您的客户经理联系。

* [](https://daycare.day.com) [产品访问](https://login.marketing.adobe.com)

* [Adobe客户关怀](https://helpx.adobe.com/contact.html)
