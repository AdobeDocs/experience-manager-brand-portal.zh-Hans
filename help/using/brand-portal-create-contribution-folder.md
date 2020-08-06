---
title: 创建贡献文件夹
seo-title: 创建贡献文件夹
description: '了解如何在AEM Assets创建贡献文件夹。 '
seo-description: 了解如何在AEM Assets创建贡献文件夹。
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: c359cf9c467fa6d20bebfdf2f8a72e8dd0e50916
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---


# Create contribution folder {#create-contribution-folder}


AEM管理员和非管理员用户有权创建新文件夹，可在AEM Assets创建贡献文件夹。
要创建贡献文件夹，请新建一个“资产贡献”类型的文件夹，确保创建的新文件夹可由Brand Portal用户提交资产。  这会自动触发一个工作流，该工作流会在贡献文件夹内创建另外两个子文件夹，称为SHARED和NEW。

>[!NOTE]
>
>您可以在一个文件夹中创建多个贡献文件夹，但不得在另一个贡献文件夹内创建贡献文件夹。

要创建贡献文件夹，请执行以下操作：
1. 登录到AEM作者实例。

   默认URL为http:// localhost:4502/aem/start.html。

1. 导航到 **[!UICONTROL 资产]** > **[!UICONTROL 文件]**。 它将列表AEM Assets存储库中的所有现有文件夹。

1. Click **[!UICONTROL Create]** to create a new folder. **[!UICONTROL “创建文件夹]** ”对话框打开。

1. 输入 **[!UICONTROL 文]** 件夹的 **[!UICONTROL 标题]** 和名称 **[!UICONTROL ，然后启用“资]** 产贡献”复选框。
建议使用小写字母来命名文件夹，但不要有任何空格。

1. 单击&#x200B;**[!UICONTROL 创建]**。您可以看到列在AEM Assets存储库中的贡献文件夹。

   >[!NOTE]
   >
   >非管理员用户可以创建和共享资产贡献文件夹，但无法修改或删除它。

   ![](assets/create-contribution-folder.png)

1. 单击打开贡献文件夹，您可以看到两个子文件夹-**[!UICONTROL SHARED]****[!UICONTROL 和NEW]** 在贡献文件夹中自动创建。

   ![](assets/contribution-folder.png)

您现在可以 [配置贡献文件夹属性](brand-portal-configure-contribution-folder-properties.md)。


