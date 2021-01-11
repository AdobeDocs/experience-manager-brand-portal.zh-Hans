---
title: 发布到贡献文件夹到AEM Assets
seo-title: 发布到贡献文件夹到AEM Assets
description: 深入了解在Brand Portal中将贡献文件夹发布到AEM Assets。
seo-description: 深入了解在Brand Portal中将贡献文件夹发布到AEM Assets。
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 6eb01e2eec7de6b704976c990fb6ffacbc67471a
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---


# 将贡献文件夹发布到AEM Assets{#publish-contribution-folder-to-aem}

Brand Portal用户可以将贡献文件夹发布到AEM Assets，无需访问AEM作者实例。

请确保已完成[资产要求](brand-portal-download-asset-requirements.md)，并上传贡献文件夹&#x200B;**NEW**&#x200B;文件夹中新创建的资产。 请参阅[将资产上传到贡献文件夹](brand-portal-upload-assets-to-contribution-folder.md)。

**要发布贡献文件夹，请执行以下操作：**

1. 登录您的Brand Portal实例。

1. 从Brand Portal仪表板中选择贡献文件夹。
1. 单击&#x200B;**[!UICONTROL 发布到AEM]**。

   ![](assets/export.png)

   ![](assets/publish-contribution-folder-to-aem.png)

将向位于发布工作流程不同阶段的Brand Portal用户和管理员发送电子邮件／脉冲通知：
1. **排队** -在Brand Portal中触发发布工作流时，将向Brand Portal用户和Brand Portal管理员发送通知。

1. **完成** -贡献文件夹成功发布到AEM Assets时，将向Brand Portal用户和Brand Portal管理员发送通知。


**发布作业状态**

管理员可以利用两种报告来视图从Brand Portal发布到AEM Assets的资产贡献文件夹的状态。

* 在Brand Portal中，导航到&#x200B;**[!UICONTROL 工具]** > **[!UICONTROL 资产贡献状态]**。 此报告反映了发布工作流程不同阶段的所有发布作业的状态。

   ![](assets/contribution-folder-status.png)

* 在AEM Assets创作实例中，导航到&#x200B;**[!UICONTROL 工具]** > **[!UICONTROL 作业]**。 此报告反映了所有发布作业的最终状态（成功或错误）。

   ![](assets/publishing-status.png)




