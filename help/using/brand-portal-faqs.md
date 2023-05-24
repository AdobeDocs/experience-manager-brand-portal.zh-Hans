---
title: 常见问题解答
seo-title: null
description: 深入了解Adobe Experience Manager Assets Brand Portal中的常见问题解答。
seo-description: null
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 4a8f7fbd-7485-421d-a8db-755324d2dbef
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '1509'
ht-degree: 0%

---

# 常见问题解答 {#frequently-asked-questions}

Brand Portal常见问题解答侧重于最终用户在使用最新Experience Manager Assets Brand Portal 6.4.6版本或更早版本时可能遇到的查询和问题。


## Brand Portal 6.4.6常见问题解答  {#faqs-bp646}

**各位。 现有旧版OAuth端点(`https://legacy-oauth.cloud.adobe.io/login`)不起作用。 可能的原因是什么？**

**无。** 已弃用旧版OAuth配置。 您必须将Experience Manager Assets创作实例升级到最新的Service Pack并通过Adobe Developer控制台进行配置。 参见 [使用Brand Portal配置Experience Manager Assets](configure-aem-assets-with-brand-portal.md) 了解详细信息。 但是，要使旧版OAuth配置在升级之前一直有效，请将旧版OAuth端点更新为 `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`.

<!--
**Ques. I have created a collection using the asset link shared by the administrator. But I am unable to create a share link for my collection. Do I need special permissions to do this?**

**Ans.** The functionality is by design, the viewer users are not permitted to share link for collections as they have limited privileges due to which they cannot add users to create a share link. It is a known issue that the share link for collections is currently visible to the viewer users. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.    
-->

**各位。 升级到Adobe Developer控制台后，我无法将贡献文件夹的资产从Brand Portal发布到Experience Manager Assets。 我的创作实例位于Experience Manager Assets 6.5.4。可能的原因是什么？**

**无。** 是，通过Adobe Developer控制台将贡献文件夹中的资产发布到Experience Manager Assets 6.5.4时存在一个已知问题。

已在Experience Manager Assets 6.5.5中修复此问题。您可以将Experience Manager Assets实例升级到最新的Service Pack，并且 [升级配置](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) 在Adobe Developer控制台上。

<!--
Broken link of download hotfix, comment out this section until we have the latest URL.

For immediate fix on AEM 6.5.4, it is recommended to [download the hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) and install on your AEM author instance.
-->

**各位。 我没有在Experience Manager Assets中看到从Brand Portal发布的contribution文件夹的内容。 可能的原因是什么？**

**无。** 请联系您的Experience Manager Assets管理员以验证配置，并确保您的Brand Portal租户仅配置了一个Experience Manager Assets创作实例。

当您在多个Brand Portal创作实例上配置了一个Experience Manager Assets租户时，可能会发生此问题。 例如，管理员在暂存和生产环境的Experience Manager Assets创作实例上配置相同的Brand Portal租户。 在这种情况下，资产发布将在Brand Portal中触发，但Experience Manager Assets创作实例无法导入资产，因为复制代理未收到请求令牌。


**各位。 我无法将资源从Experience Manager Assets发布到Brand Portal。 复制日志指出连接超时。 有快速修复方法吗？**

**无。** 如果复制队列中有多个挂起的请求，则发布通常会失败并出现超时错误。 要解决此问题，请确保将复制代理配置为避免超时。

执行以下步骤来配置复制代理：

1. 登录到您的Experience Manager Assets创作实例。
1. 从 **工具** 面板，导航到 **[!UICONTROL 部署]** > **[!UICONTROL 复制]**.
1. 在“复制”页中，单击 **[!UICONTROL 作者代理]**. 您可以看到您的Brand Portal租户的四个复制代理。
1. 单击复制代理URL以打开代理详细信息。
1. 单击 **[!UICONTROL 编辑]** 修改复制代理设置。
1. 在“代理设置”中，单击 **[!UICONTROL 扩展]** 选项卡。
1. 选择 **[!UICONTROL 关闭连接]** 复选框。
1. 重复步骤4至7以配置所有四个复制代理。
1. 重新启动服务器并验证连接。


## Brand Portal 6.4.5常见问题解答  {#faqs-bp645}

**各位。 Brand Portal 6.4.5版本中的主要更改是什么？**

**无。** Experience Manager Assets Brand Portal 6.4.5是一个功能版本，它允许Brand Portal用户从Brand Portal实例中上传内容并将Contribution文件夹发布回Experience Manager Assets，而无需管理员权限。
有关更多信息，请参阅 [Brand Portal中的资源源](brand-portal-asset-sourcing.md).



**各位。 我是否将失去对已创建的任何现有资源、功能或配置的访问权限？**

**无。** 所有现有功能和配置保持不变。 最终用户不受影响，您的内容保持不变。



**各位。 我何时可以迁移到新版本的Brand Portal？**

**无。** Brand Portal 6.4.5于2019年10月发布到生产环境。 下一版Brand Portal预计于2020年第三季度发布。
有关更新和版本更改，建议跟踪 [发行说明](brand-portal-release-notes.md) 和 [Brand Portal的新增功能](whats-new.md).



**各位。 我的用户是否会受到影响？**

**无。** Brand Portal 6.4.5版本仅包含在Brand Portal中，因此不会对最终用户产生影响。



**各位。 作为Brand Portal用户，我是否需要执行任何操作？**

**无。** Brand Portal 6.4.5版本中提供了名为Asset Sourcing的新功能。 管理员必须在Experience Manager Assets中配置Asset Sourcing功能，以便为Brand Portal用户启用该功能。 有关更多信息，请参阅 [启用资产源](brand-portal-asset-sourcing.md).



**各位。 谁可以创建Contribution文件夹？**

**无。** 任何有权在Experience Manager Assets中创建新文件夹的Experience Manager Assets用户都可以创建 **贡献** 文件夹。 创建 **贡献** 文件夹，新建类型为的文件夹 **资产贡献**.
此文件夹与活动的Brand Portal用户共享，以便进行贡献。



**各位。 Contribution文件夹包含什么？**

**无。** **贡献** 文件夹包含两个子文件夹 **新** 和 **已共享**. 最初，NEW文件夹为空，而SHARED文件夹包含Brand Portal用户的引用内容（可重用资源）。
Brand Portal用户访问 **贡献** 文件夹并上传内容于 **新** 文件夹。



**各位。  我是否可以修改现有“贡献”文件夹的名称？**

**无。** **否**，则无法修改现有项目的名称 **贡献** 文件夹。



**各位。 资产要求与RT贡献是什么？**

**无。** 此 **摘要** 文档附加到 **贡献** 文件夹和上传到的引用内容（可重用资源） **已共享** 文件夹有助于Brand Portal用户了解作为投稿人的贡献和期望的需求，它统称为资源要求。



**各位。 我是否可以将资产上传到任何允许的文件夹？**

**无。** 并非所有允许的文件夹。 Brand Portal用户只能将内容上传到 **贡献** Experience Manager Assets或Brand Portal管理员共享的文件夹。



**各位。 如何获取“贡献”文件夹的访问权限？**

**无。** 您可以访问 **贡献** 仅当已与您共享该文件夹时，才使用它。 每当您共享“贡献”文件夹时，您都会收到电子邮件/脉冲通知。 您可以通过电子邮件中共享的链接访问Contribution文件夹，也可以登录您的Brand Portal实例并导航到铃铛图标以进行通知，以访问Contribution文件夹。

>[!NOTE]
>
>如果您不是现有Brand Portal用户，请请求Experience Manager Assets管理员在Admin Console中创建您的用户，并将您的配置文件添加到Brand Portal用户列表中的用户配置文件中。

**各位。 用于用户导入的CSV文件的格式是什么？**

**无。** 格式与Admin Console支持批量用户导入的格式相同。 电子邮件、名字和姓氏是必填项。



**各位。 “资产贡献用户”下拉列表中的用户(Brand Portal参与者)中填充了哪些内容？**

**无。** 下拉列表中的用户会从Experience Manager Assets中上传的Brand Portal用户配置(.csv)文件中填充。



**各位。 可在何处查看导入和发布作业的状态？**

**无。** 在Experience Manager Assets中，您可以在中查看导入的状态 **异步** 作业页面。 在Brand Portal中，您可以在中查看发布作业的状态 **[!UICONTROL 工具>资产贡献状态]**.



**各位。 定期在Experience Manager中运行的导入作业的频率是多少？**

**无。** 在Experience Manager Assets中，每5分钟运行一次轮询。



**各位。 能否限制文件夹从Brand Portal发布到Experience Manager Assets的次数？**

**无。** 否，中的所有资产 **新** 文件夹将发布到Experience Manager Assets，而不管它们之前是否发布。 每次a **贡献** 文件夹从Brand Portal发布到Experience Manager Assets，它覆盖 **新** 文件夹。



**各位。 如何在“贡献”文件夹中上传新资产？**

**无。** 请参阅详细文档，了解 [将资产上传到“贡献”文件夹](brand-portal-publish-contribution-folder-to-brand-portal.md).



**各位。 我是否未看到由Brand Portal用户上传到NEW文件夹的资源的缩略图/预览？**

**无。** 它是按预期设计的，因为Brand Portal端不会运行任何工作流。



**各位。 如果将某个文件夹从Experience Manager Assets发布到处于动态变化状态的Brand Portal，会发生什么情况？**

**无。** 在Experience Manager Assets中，每次将文件夹发布到Brand Portal时都会维护日志。 发布时，所有未发布到Brand Portal的资产都放入复制队列中。 触发发布作业后添加到文件夹的任何资源都不会发布到Brand Portal。 当Experience Manager Assets用户再次发布该文件夹时，只有之前未发布的资源（位于复制队列中）才会发布到Brand Portal。
对于从Experience Manager Assets发布到Brand Portal的任何文件夹，以及Contribution文件夹中的SHARED文件夹，情况均如此。

**各位。 如有疑问，我应该联系谁？**

**无。** 请联系您的Adobe客户经理或客户支持。

>[!NOTE]
>
>发布计划是暂定的，可能会有变化。 请联系您的Adobe客户经理或客户支持部门以获取更新的发布计划。


## 产品访问和支持（受限制的站点） {#product-access-and-support-restricted-sites}

这些网站仅对客户可用。 如果您是客户并需要访问权限，请联系您的Adobe客户经理。

<!--
* [](https://daycare.day.com) [Product Access](https://login.marketing.adobe.com)

* [Adobe Customer Support]()
-->
