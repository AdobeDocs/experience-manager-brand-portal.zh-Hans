---
title: 创建贡献文件夹
seo-title: 创建贡献文件夹
description: '了解如何在AEM资产中创建贡献文件夹。 '
seo-description: 了解如何在AEM资产中创建贡献文件夹。
uuid: null
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 22b327619eb73c0099f903bb7314d2cb2d796bc4

---


# Create contribution folder {#create-contribution-folder}

AEM管理员和具有创建新文件夹权限的非管理员用户可以在AEM资产中创建 **Contribution** 文件夹。
要创建贡 **献文件夹** ，请新建一个“资产贡献”类型的文件夹 ****，确保创建的新文件夹可由Brand Portal用户提交资产。  这会自动触发一个工作流，该工作流在新创建的 **Contribution** （贡献）文件夹内创建另外两个子文件夹，名 **为** SHARED **（共享）和NEW（新建）** 。

**要创建新贡献文件夹，请执行以下操作：**
1. 登录AEM作者实例默认URL:http://本地主机：4502/aem/start.html
1. 导航到“ **[!UICONTROL 资产”>“文]**件”。它会列出AEM资产存储库中的所有现有文件夹。
1. Click **[!UICONTROL Create]**to create a new folder. “创建文件夹”弹出窗口将打开。
1. 输入 **[!UICONTROL 文件夹的标]**题和名称**[!UICONTROL ，并标记复选框“资]** 产贡献” ****。
建议使用没有空格的小字母来命名文件夹。
1. 单击&#x200B;**[!UICONTROL 创建]**。   ![](assets/create-contribution-folder.png)
1. 您可以在AEM资产存储库中看到列出的新创建的贡献文件夹。
1. 单击以打开贡献文件夹，您可以看到两个子文件夹-**[!UICONTROL SHARED]**,**[!UICONTROL  NEW]** are automatically created in the contribution folder.\
   ![](assets/contribution-folder.png)

您现在可以配置贡献文件夹属性。 请参阅配置 [贡献文件夹属性](brand-portal-configure-contribution-folder-properties.md)。

>[!NOTE]
>
>请确保为“贡献”文件夹提供相应的名称，因为您无法在创建后修改文件夹名称。