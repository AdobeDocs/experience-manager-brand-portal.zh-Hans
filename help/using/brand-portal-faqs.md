---
title: 常见问题
seo-title: null
description: 深入了解Adobe Experience Manager Assets Brand Portal中的常见问题解答。
seo-description: null
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 9169407bbbfabd94be31c89c028be64e55afc064

---


# 常见问题 {#frequently-asked-questions}

Brand Portal常见问题解答侧重于最终用户在使用最新的AEM Assets Brand Portal 6.4.5版本或更早版本时可能遇到的查询和问题。


## Brand Portal 6.4.6常见问题解答 {#faqs-bp646}

**Ques. 现有的旧版OAuth端点(`https://legacy-oauth.cloud.adobe.io/login`)无效。 可能的原因是什么？**

**安。** 旧版OAuth配置已弃用。 您必须将AEM Assets作者实例升级到最新的Service Pack，然后使用Adobe IO对其进行配置。 有关详 [细信息，请参阅配置AEM资产与Brand Portal](configure-aem-assets-with-brand-portal.md) 。 但是，要使旧版OAuth配置在升级之前正常工作，请将旧版OAuth端点更新为 `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`。

**Ques. 升级到Adobe I/O后，我无法将贡献文件夹的资产从Brand Portal发布到AEM资产。我的作者实例位于AEM 6.5.4上。可能的原因是什么？**

**安。** 是，使用Adobe I/O将分发文件夹的资产发布到AEM 6.5.4上的AEM资产时存在已知问题。此问题将在下一个服务包中修复。

要立即修复AEM 6.5.4，建议下载 [修补程序](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) ，并安装在AEM作者实例上。


## Brand Portal 6.4.5常见问题解答 {#faqs-bp645}

**Ques. Brand Portal 6.4.5版本中的主要更改是什么？**

**安。** AEM Assets Brand Portal 6.4.5是一项功能发行版，通过该版本，Brand Portal用户无需管理员权限即可从Brand Portal实例中上传内容并将贡献文件夹发布回AEM资产。
有关详细信息，请参 [阅品牌门户中的资产来源补充](brand-portal-asset-sourcing.md)。



**Ques. 我是否将失去对我创建的任何现有资产、功能或配置的访问权？**

**安。** 您的所有现有功能和配置均保持不变。 您的最终用户不会受到影响，您的内容将保持不变。



**Ques. 我何时将转向新版本的Brand Portal?**

**安。** Brand Portal 6.4.5已于2019年10月发布至生产。 下一个Brand Portal版本预计将在2020年第3季度发布。
对于更新和版本更改，建议跟踪 [Brand Portal的发行说明](brand-portal-release-notes.md)[和新增功能](whats-new.md)。



**Ques. 我的用户是否会受到影响？**

**安。** Brand Portal 6.4.5版本仅在Brand Portal中提供，因此对最终用户没有影响。



**Ques. 作为Brand Portal用户，我是否需要执行任何操作？**

**安。** Brand Portal 6.4.5版本提供了名为“资产来源补充”的新功能。 AEM管理员必须在AEM资产中配置资产来源补充功能，以为Brand Portal用户启用该功能。 有关详细信息，请参阅启 [用资产来源补充](brand-portal-configure-asset-sourcing.md)。



**Ques. 谁可以创建贡献文件夹？**

**安。** 任何具有在AEM资产中创建新文件夹权限的AEM用户都可以创建“贡 **献** ”文件夹。 要创建贡献文 **件夹** ，请新建一个“资产贡献”类型 **的文件夹**。
此文件夹将与活动的Brand Portal用户共享以供贡献。



**Ques. 贡献文件夹包含什么？**

**安。** Contribution **** 文件夹包含两个子文 **件夹** NEW ****和SHARED。 最初，NEW文件夹为空，而SHARED文件夹包含Brand Portal用户的参考内容（可重用资产）。
Brand Portal用户访问Contribution **文件夹** ，并上传 **NEW** 文件夹中的内容。



**Ques.  我是否可以修改现有贡献文件夹的名称？**

**安。** 否 ****，您无法修改现有贡献文件夹 **的名称** 。



**Ques. 资产要求w.r.t的贡献是什么？**

**安。** 附加到 **** Contribution **文件夹的简短文档以及上传到** SHARED **** 文件夹中的参考内容（可重用资产）可帮助Brand Portal用户了解作为参与者的贡献和期望的需求，并统称为资产要求。



**Ques. 我是否可以将资产上传到任何允许的文件夹？**

**安。** 并非所有允许的文件夹。 Brand Portal用户只能将内容上传到AEM或Brand Portal **管理员共享的** Contribution文件夹。



**Ques. 如何访问贡献文件夹？**

**安。** 仅当Contribution文件夹已 **与您共享** ，您才可以访问它。 只要您共享了贡献文件夹，您就会收到电子邮件／脉冲通知。 您可以通过电子邮件中共享的链接访问贡献文件夹，或登录到您的Brand Portal实例，然后导航到铃图标以便获得通知以访问贡献文件夹。

>[!NOTE]
>
>如果您不是现有Brand Portal用户，请请求AEM管理员在AEM管理控制台中创建您的用户，并将您的用户档案添加到Brand Portal用户列表中的用户配置文件。 请参阅添 [加Brand Portal用户](brand-portal-configure-asset-sourcing.md)。



**Ques. 用户导入的CSV文件的格式是什么？**

**安。** 格式与Admin Console支持的批量用户导入格式相同。 电子邮件、名字和姓氏是必填项。



**Ques. 什么内容会在“资产贡献”用户下拉列表中填充用户（Brand Portal参与者）的列表?**

**安。** 下拉列表中的用户将从AEM中上传的Brand Portal用户配置(.csv)文件中填充。



**Ques. 在哪里可以看到导入和发布作业的状态？**

**安。** 在AEM中，您可以在异步作业页面中查看导入 **的状** 态。 在Brand Portal中，您可以在“工具”>“资产贡献”状态中 **[!UICONTROL 查看发布作业的状态]**。



**Ques. 在AEM中定期运行的导入作业的频率是多少？**

**安。** 在AEM中，轮询每5分钟运行一次。



**Ques. 是否存在将文件夹从Brand Portal发布到AEM资产的次数的问题？**

**安。** 否，NEW文件夹中的所有资 **产将发布到** AEM资产，而不管之前发布了这些资产。 每次将 **Contribution** 文件夹从Brand Portal发布到AEM Assets时，它都会覆盖 **NEW** 文件夹的内容。



**Ques. 如何上传贡献文件夹中的新资产？**

**安。** 请参阅将资产上传到贡献 [文件夹的详细文档](brand-portal-upload-assets-to-contribution-folder.md)。



**Ques. 我看不到由Brand Portal用户上传到NEW文件夹的资产的缩略图/预览?**

**安。** 它是按照设计的，coz没有在Brand Portal端运行的工作流。



**Ques. 如果文件夹从AEM资产发布到处于流动状态的Brand Portal，会发生什么情况？**

**安。** 在AEM中，每次将文件夹发布到Brand Portal时都会维护日志。 在发布时，所有未发布到Brand Portal的资产都将放在复制队列中。 触发发布作业后添加到该文件夹的任何资产都不会发布到Brand Portal。 当AEM用户再次发布文件夹时，只有之前未发布的资产（在复制队列中存在）才会发布到Brand Portal。
对于从AEM资产发布到Brand Portal的任何文件夹以及贡献文件夹中的SHARED文件夹，此情况均适用。



**Ques. 如有疑问，应与谁联系？**

**安。** 联系您的Adobe客户经理或客户支持。


>[!NOTE]
>
>释放计划是试探性的，可能会发生变化。 请联系您的Adobe客户经理或客户支持以获取更新的发行计划。




## Product Access and Support (Restricted Sites) {#product-access-and-support-restricted-sites}

这些网站仅适用于客户。如果您是客户并需要访问，请与您的Adobe客户经理联系。

* [](https://daycare.day.com) 产 [品访问](https://login.marketing.adobe.com)

* [Adobe客户关怀](https://helpx.adobe.com/contact.html)
