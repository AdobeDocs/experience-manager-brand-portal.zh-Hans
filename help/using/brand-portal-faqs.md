---
title: 常见问题
seo-title: null
description: 深入了解Adobe Experience Manager Assets品牌门户中的常见问题。
seo-description: null
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: aefffb21b277d93fab2754dae407de7602f614c7
workflow-type: tm+mt
source-wordcount: '1536'
ht-degree: 0%

---


# 常见问题 {#frequently-asked-questions}

Brand Portal常见问题解答侧重于最终用户在使用最新的AEM Assets Brand Portal 6.4.6版本或更早版本时可能遇到的查询和问题。


## Brand Portal 6.4.6常见问题解答  {#faqs-bp646}



**Ques。 现有旧版OAuth端点(`https://legacy-oauth.cloud.adobe.io/login`)无效。 可能的原因是什么？**

**安。** 旧版OAuth配置已弃用。 您必须将AEM Assets作者实例升级到最新的Service Pack，并通过Adobe Developer Console进行配置。 有关详 [细信息，请参阅配置AEM资产与Brand](configure-aem-assets-with-brand-portal.md) Portal。 但是，要使旧版OAuth配置在升级之前正常工作，请将旧版OAuth端点更新为 `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`。


**Ques。 升级到Adobe开发人员控制台后，我无法将贡献文件夹的资产从Brand Portal发布到AEM资产。 我的作者实例位于AEM 6.5.4上。可能的原因是什么？**

**安。** 是的，通过Adobe开发人员控制台将贡献文件夹的资产发布到AEM 6.5.4上的AEM资产时存在已知问题。

此问题在AEM 6.5.5中已解决。您可以将AEM资产实例升级到最新的Service Pack AEM 6.5.5，并在Adobe开发人 [员控制台上](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) 升级您的配置。

要立即修复AEM 6.5.4，建议下载 [修补程序](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) ，并在AEM作者实例上安装。


**Ques。 我要在AEM Assets云实例上启用资产来源补充功能。 如何配置它？**

**安。** 否，AEM Assets云服务当前不支持资产来源补充功能。

保持联系并查看发行说明，了解有关即将发布的版本中功能可用性的通知。


**Ques。 我无法将资产从AEM资产发布到Brand Portal，且复制代理日志引发异常`java.net.SocketException: Connection timed out`。 有速效药吗？**

**安。** 如果复制队列中有待处理的请求数，则复制代理可能不处理发布资产的请求并引发异常： `java.net.SocketException: Connection timed out`.

请执行以下步骤来修复问题：

1. 打开复制代理，然后单 **[!UICONTROL 击]** “编辑”以修改复制代理设置。
1. 在“代理设置”中，单击“扩展”选 **[!UICONTROL 项卡]**。
1. 启用复选框“ **[!UICONTROL 关闭连接]**”。
1. 重新启动复制捆绑包（服务器）。

对所有四个复制代理启用设置，以避免任何复制代理出现问题。


**Ques。 在AEM资产中，我看不到从Brand Portal发布的贡献文件夹的内容。 可能的原因是什么？**

**安。** 请与AEM资产管理员联系，以验证配置并确保您的Brand Portal租户仅配置了一个AEM资产作者实例。

在多个AEM资产作者实例上配置Brand Portal租户时，可能会出现此问题。 例如，管理员在AEM资产作者实例上配置登台和生产环境的同一Brand Portal租户。 在这种情况下，资产发布会在Brand Portal中触发，但AEM资产作者实例无法导入资产coz，复制代理未收到请求令牌。

## Brand Portal 6.4.5常见问题解答  {#faqs-bp645}

**Ques。 Brand Portal 6.4.5版本中有哪些主要更改？**

**安。** AEM Assets Brand Portal 6.4.5是一项功能发行，通过该功能，Brand Portal用户无需管理员权限即可从Brand Portal实例内上传内容并将贡献文件夹发布回AEM资产。
有关详细信息，请参 [阅品牌门户中的资产来源补充](brand-portal-asset-sourcing.md)。



**Ques。 我是否将失去对已创建的任何现有资产、功能或配置的访问权限？**

**安。** 您的所有现有功能和配置均保持原样。 您的最终用户不受影响，您的内容将保持原样。



**Ques。 我何时将转向新版Brand Portal?**

**安。** Brand Portal 6.4.5已于2019年10月发布并投入生产。 下一个品牌门户版本预计将于2020年第3季度发布。
对于更新和版本更改，建议跟踪 [Brand Portal的](brand-portal-release-notes.md)[发行说明和新增功能](whats-new.md)。



**Ques。 我的用户是否会受到影响？**

**安。** Brand Portal 6.4.5版本只包含在Brand Portal中，因此对最终用户没有影响。



**Ques。 作为Brand Portal用户，我是否需要执行任何操作？**

**安。** Brand Portal 6.4.5版本提供了名为“资产来源补充”的新增功能。 AEM管理员必须在AEM资产中配置资产来源补充功能，以为品牌门户用户启用该功能。 有关详细信息，请参阅启 [用资产来源补充](brand-portal-configure-asset-sourcing.md)。



**Ques。 谁可以创建贡献文件夹？**

**安。** 任何具有在AEM资产中创建新文件夹权限的AEM用户都可以创建贡 **献文** 件夹。 要创建贡 **献文件** ，请新建一个“资产贡献”类 **型的文件夹**。
此文件夹将与活动的Brand Portal用户共享，以供参与。



**Ques。 贡献文件夹包含什么？**

**安。** **贡献** 文件夹包含两个子文 **件夹** NEW **和**SHARED。 最初，NEW文件夹为空，SHARED文件夹包含Brand Portal用户的参考内容（可重用资产）。
Brand Portal用户访问Contribution **文件夹** ，并上传NEW文 **件夹中** 的内容。



**Ques。  我是否可以修改现有贡献文件夹的名称？**

**安。** **否**，您无法修改现有贡献文件 **夹的** 名称。



**Ques。 资产要求w.r.t的贡献是什么？**

**安。** 附 **加到Contribution** 文件夹的Brief ******** 文档以及SHARED文件夹中上传的参考内容（可重用资产）可帮助Brand Portal用户了解作为参与者的贡献和期望，并统称为资产要求。



**Ques。 我是否可以将资产上传到任何允许的文件夹？**

**安。** 并非所有允许的文件夹。 Brand Portal用户只能将内容上传到AEM或 **Brand** Portal管理员共享的Contribution文件夹。



**Ques。 如何获取对贡献文件夹的访问权限？**

**安。** 只有已与您共 **享Contribution** 文件夹，您才能访问它。 只要您共享贡献文件夹，您就会收到电子邮件／脉冲通知。 您可以通过电子邮件中共享的链接访问贡献文件夹，或登录到您的Brand Portal实例并导航到铃图标，以便通知访问贡献文件夹。

>[!NOTE]
>
>如果您不是现有Brand Portal用户，请请求AEM管理员在AEM管理控制台中创建您的用户，并将您的用户档案添加到Brand Portal用户列表中的用户配置文件。 请参阅 [添加Brand Portal用户](brand-portal-configure-asset-sourcing.md)。




**Ques。 用户导入的CSV文件的格式是什么？**

**安。** 格式与Admin Console支持的批量用户导入格式相同。 电子邮件、名字和姓氏是必填项。



**Ques。 在“资产贡献用户”下拉列表中填充用户列表（Brand Portal参与者）的内容是什么？**

**安。** 下拉列表中的用户将通过AEM中上传的Brand Portal用户配置(.csv)文件进行填充。



**Ques。 在哪里可以看到导入和发布作业的状态？**

**安。** 在AEM中，您可以在异步作业页面中看到导 **入的** 状态。 在Brand Portal中，您可以在工具>资产贡献状态中 **[!UICONTROL 查看发布作业的状态]**。



**Ques。 在AEM中定期运行的导入作业的频率是多少？**

**安。** 在AEM中，轮询每5分钟运行一次。



**Ques。 文件夹从Brand Portal发布到AEM资产的次数是否存在问题？**

**安。** 否，NEW文件夹中的所 **有资产** 都将发布到AEM资产，而不管之前发布了这些资产。 每次将 **Contribution** 文件夹从Brand Portal发布到AEM资产时，它都会覆盖NEW文件 **夹的内** 容。



**Ques。 如何上传贡献文件夹中的新资产？**

**安。** 请参阅将资产上传到贡 [献文件夹的详细文档](brand-portal-upload-assets-to-contribution-folder.md)。



**Ques。 我看不到品牌门户用户上传到NEW文件夹的资产的缩略图/预览?**

**安。** 它是按照设计的，coz在Brand Portal端没有运行工作流。



**Ques。 如果文件夹从AEM资产发布到处于动态状态的Brand Portal，会发生什么情况？**

**安。** 在AEM中，每次将文件夹发布到Brand Portal时，都会保留日志。 在发布时，所有未发布到Brand Portal的资产都将放在复制队列中。 触发发布作业后添加到文件夹的任何资产均不会发布到Brand Portal。 当AEM用户再次发布文件夹时，只有之前未发布的资产（在复制队列中存在）才会发布到Brand Portal。
对于从AEM资产发布到Brand Portal的任何文件夹以及贡献文件夹中的SHARED文件夹，此情况均适用。



**Ques。 如有问题，应与谁联系？**

**安。** 联系您的Adobe客户经理或客户支持。


>[!NOTE]
>
>释放计划是暂时性的，可能会发生变化。 联系您的Adobe客户经理或客户支持以获取更新的发行计划。




## Product Access and Support (Restricted Sites) {#product-access-and-support-restricted-sites}

这些网站仅适用于客户。如果您是客户并需要访问，请与您的Adobe客户经理联系。

* [](https://daycare.day.com) [产品访问](https://login.marketing.adobe.com)

* [Adobe客户关怀](https://helpx.adobe.com/contact.html)
