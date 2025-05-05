---
title: 常见问题解答
description: 深入了解Adobe Experience Manager Assets Brand Portal中的常见问题解答。
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 4a8f7fbd-7485-421d-a8db-755324d2dbef
source-git-commit: 32a67abf466dd3bf635b851b02377ed23591915e
workflow-type: tm+mt
source-wordcount: '1500'
ht-degree: 0%

---

# 常见问题解答 {#frequently-asked-questions}

Brand Portal常见问题解答侧重于最终用户在使用最新Experience Manager Assets Brand Portal 6.4.6版本或更早版本时可能遇到的查询和问题。


## Brand Portal 6.4.6常见问题解答 {#faqs-bp646}

**问题：现有旧版OAuth终结点(`https://legacy-oauth.cloud.adobe.io/login`)无法正常工作。 可能的原因是什么？**

**答案：**&#x200B;旧版OAuth配置已弃用。 将Experience Manager Assets创作实例升级到最新的Service Pack并通过Adobe Developer Console进行配置。 有关详细信息，请参阅[使用Brand Portal配置Experience Manager Assets](configure-aem-assets-with-brand-portal.md)。 但是，要使旧版OAuth配置在升级之前一直有效，请将旧版OAuth端点更新为`https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`。

**问题：升级到Adobe Developer Console后，我无法将贡献文件夹的资源从Brand Portal发布到Experience Manager Assets。 我的创作实例位于Experience Manager Assets 6.5.4。可能的原因是什么？**

**回答：**&#x200B;是，通过Adobe Developer Console将贡献文件夹的资源发布到Experience Manager Assets 6.5.4时出现已知问题。

已在Experience Manager Assets 6.5.5中修复此问题。您可以在Adobe Developer Console上将Experience Manager Assets实例升级到最新的Service Pack并[升级配置](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/brandportal/configure-aem-assets-with-brand-portal#upgrade-integration-65)。


**问题：我在Experience Manager Assets中看不到从Brand Portal发布的contribution文件夹的内容。 可能的原因是什么？**

**回答：**&#x200B;请联系您的Experience Manager Assets管理员以验证配置，并确保您的Brand Portal租户仅配置了一个Experience Manager Assets创作实例。

当您在多个Brand Portal创作实例上配置了一个Experience Manager Assets租户时，可能会出现此问题。 例如，管理员在暂存和生产环境的Brand Portal创作实例上配置相同的Experience Manager Assets租户。 在这种情况下，资产发布会在Brand Portal中触发，但Experience Manager Assets创作实例无法导入资产，因为复制代理未收到请求令牌。


**问题：我无法将资源从Experience Manager Assets发布到Brand Portal。 复制日志指出连接超时。 有快速修复方法吗？**

**回答：**&#x200B;如果复制队列中有多个挂起的请求，则发布通常会失败，并出现超时错误。 要解决此问题，请确保将复制代理配置为避免超时。

执行以下步骤来配置复制代理：

1. 登录到您的Experience Manager Assets创作实例。
1. 从&#x200B;**工具**&#x200B;面板，导航到&#x200B;**[!UICONTROL 部署]** > **[!UICONTROL 复制]**。
1. 在“复制”页面中，单击&#x200B;**[!UICONTROL `Agents on author`]**。 您可以看到您的Brand Portal租户的四个复制代理。
1. 单击复制代理URL可打开代理详细信息。
1. 单击&#x200B;**[!UICONTROL 编辑]**&#x200B;可编辑复制代理设置。
1. 在代理设置中，单击&#x200B;**[!UICONTROL 扩展]**&#x200B;选项卡。
1. 选中&#x200B;**[!UICONTROL 关闭连接]**&#x200B;复选框。
1. 重复步骤4至7以配置所有四个复制代理。
1. 重新启动服务器并验证连接。


## Brand Portal 6.4.5常见问题解答 {#faqs-bp645}

**问题：Brand Portal 6.4.5版本中的主要更改是什么？**

**答案：** Experience Manager Assets Brand Portal 6.4.5允许用户直接从Brand Portal上传内容并将Contribution文件夹发布回Experience Manager Assets，而无需管理员权限。 有关详细信息，请参阅[Brand Portal中的资源源](brand-portal-asset-sourcing.md)。



**问题：我是否丧失了对我创建的任何现有资源、功能或配置的访问权限？**

**回答：**&#x200B;所有现有功能和配置保持不变。 最终用户不受影响，您的内容将保持不变。



**问题：何时可以迁移到Brand Portal的新版本？**

**答案：** Brand Portal 6.4.5已于2019年10月发布到生产环境。 下一版Brand Portal预计将于2020年3月发布。
有关更新和版本更改，Adobe建议您跟踪[发行说明](brand-portal-release-notes.md)和[Brand Portal的新增功能](whats-new.md)。



**问题：我的用户是否受到影响？**

**回答：** Brand Portal 6.4.5版本仅包含在Brand Portal中，因此不会对最终用户产生影响。



**问题：作为Brand Portal用户，我是否需要执行任何操作？**

**答案：** Brand Portal 6.4.5版本中新增了一项名为Asset Sourcing的功能。 管理员必须在Experience Manager Assets中配置Asset Sourcing功能，以便为Brand Portal用户启用该功能。 有关详细信息，请参阅[启用资产源](brand-portal-asset-sourcing.md)。



**问题：谁可以创建贡献文件夹？**

**回答：**&#x200B;任何有权在Experience Manager Assets中创建文件夹的Experience Manager Assets用户都可以创建&#x200B;**贡献**&#x200B;文件夹。 要创建&#x200B;**贡献**&#x200B;文件夹，请创建&#x200B;**资产贡献**&#x200B;类型的文件夹。
此文件夹与活动的Brand Portal用户共享，以便进行贡献。



**问题：“贡献”文件夹包含什么？**

**答案：** **贡献**&#x200B;文件夹包含两个子文件夹&#x200B;**NEW**&#x200B;和&#x200B;**SHARED**。 最初，NEW文件夹为空，并且SHARED文件夹包含Brand Portal用户的引用内容（可重用资源）。
Brand Portal用户访问&#x200B;**贡献**&#x200B;文件夹并上传&#x200B;**新建**&#x200B;文件夹中的内容。



**问题：是否可以修改现有贡献文件夹的名称？**

**答案：** **否**，您无法修改现有&#x200B;**贡献**&#x200B;文件夹的名称。



**问题：资产要求w.r.t.贡献是什么？**

**回答：** **贡献**&#x200B;文件夹中的&#x200B;**Brief**&#x200B;文档和&#x200B;**共享**&#x200B;文件夹中的引用内容可帮助Brand Portal用户了解贡献需求和期望。 这些需求统称为资产要求。

**问题：我是否可以将资源上传到任何允许的文件夹？**

**回答：**&#x200B;并非所有允许的文件夹。 Brand Portal用户只能将内容上传到Experience Manager Assets或Brand Portal管理员共享的&#x200B;**贡献**&#x200B;文件夹。



**问题：如何获取“贡献”文件夹的访问权限？**

**回答：**&#x200B;只有已与您共享的&#x200B;**贡献**&#x200B;文件夹才可访问。 每当您共享“贡献”文件夹时，您都会收到电子邮件/脉冲通知。 您可以通过电子邮件中共享的链接访问“贡献”文件夹。 或者，您可以登录到Brand Portal实例，然后导航到铃铛图标以发送通知，从而访问Contribution文件夹。

>[!NOTE]
>
>如果您不是Brand Portal用户，请请求Experience Manager Assets管理员在Admin Console中创建您的用户。 然后，将您的配置文件添加到Brand Portal用户列表中的用户配置文件。


**问题：用于用户导入的CSV文件格式是什么？**

**答案：**&#x200B;格式与批量用户导入所支持的Admin Console匹配。 电子邮件、名字和姓氏是必填项。



**问题：在“资产贡献用户”下拉列表中填充用户(Brand Portal参与者)列表的变量是什么？**

**回答：**&#x200B;下拉列表中的用户是从Experience Manager Assets中上传的Brand Portal用户配置(.csv)文件中填充的。



**问题：可在何处查看导入和发布作业的状态？**

**答案：**&#x200B;在Experience Manager Assets中，您可以在&#x200B;**异步**&#x200B;作业页面中查看导入的状态。 在Brand Portal中，您可以在&#x200B;**[!UICONTROL 工具>资源贡献状态]**&#x200B;中查看发布作业的状态。



**问题：在Experience Manager中定期运行的导入作业的频率是多少？**

**答案：**&#x200B;在Experience Manager Assets中，每5分钟运行一次轮询。



**问题：文件夹从Brand Portal发布到Experience Manager Assets的次数是否存在阈值？**

**答案：**&#x200B;否，不管&#x200B;**NEW**&#x200B;文件夹中的所有资源是否都已发布到Experience Manager Assets，实际上它们已发布过较早。 每次将&#x200B;**Contribution**&#x200B;文件夹从Brand Portal发布到Experience Manager Assets时，它都会替换&#x200B;**NEW**&#x200B;文件夹的内容。



**问题：如何在“贡献”文件夹中上传新资产？**

**答案：**&#x200B;请参阅有关[将资产上传到贡献文件夹](brand-portal-publish-contribution-folder-to-brand-portal.md)的详细文档。



**问题：对于上传到NEW文件夹的资源，我看不到其缩略图或预览。**

**答案：**&#x200B;它是按设计设计的，因为没有工作流在Brand Portal末尾运行。



**问题：如果将文件夹从Experience Manager Assets发布到处于动态变化中的Brand Portal，会发生什么情况？**

**答案：**&#x200B;在Experience Manager Assets中，每次将文件夹发布到Brand Portal时都会维护日志。 发布时，所有未发布到Brand Portal的资源都会添加到复制队列中。 触发发布作业后添加到文件夹的任何资产都不会发布到Brand Portal。 当Experience Manager Assets用户再次发布该文件夹时，只有之前未发布的资产（位于复制队列中）才会发布到Brand Portal。 对于从Experience Manager Assets发布到Brand Portal的任何文件夹，以及Contribution文件夹中的SHARED文件夹，此过程均适用。

**问题：我应向谁咨询问题？**

**回答：**&#x200B;请联系您的Adobe客户经理或客户支持。

>[!NOTE]
>
>发布计划是暂定的，可能会发生变化。 请联系您的Adobe客户经理或客户支持以获取更新的发布计划。


## 产品访问和支持（受限制的站点） {#product-access-and-support-restricted-sites}

这些网站仅供客户使用。 如果您是客户并且需要访问权限，请联系您的Adobe客户经理。

<!--
* [](https://daycare.day.com) [Product Access](https://login.marketing.adobe.com)

* [Adobe Customer Support]()
-->
