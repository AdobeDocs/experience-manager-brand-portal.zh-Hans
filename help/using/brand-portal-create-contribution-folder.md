---
title: 创建贡献文件夹
seo-title: 创建贡献文件夹
description: '获取有关如何在AEM资产中创建贡献文件夹的分析。 '
seo-description: 获取有关如何在AEM资产中创建贡献文件夹的分析。
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 5bc5d8db777b31da82b7c68896d881c1fcdaed8f
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Create contribution folder {#create-contribution-folder}

AEM管理员和具有创建新文件夹权限的非管理员用户可以在AEM资 **产中** 创建贡献文件夹。
要创建贡 **献文件** ，请新建一个“资产贡献”类型的 **文件夹**，确保创建的新文件夹可由Brand Portal用户提交资产。  这会自动触发一个工作流，该工作流会在新创建的Contribution **文件夹内** ，创建另外两个名 **为** SHARED和NEW **** 的子文件夹。

**要创建新贡献文件夹，请执行以下操作：**
1. 登录AEM作者实例默认URL: http://本地主机：4502/aem/start.html
1. 导航到 **[!UICONTROL 资产>文]**&#x200B;件它会列表AEM资产存储库中的所有现有文件夹。
1. Click **[!UICONTROL Create]** to create a new folder. “创建文件夹”弹出窗口将打开。
1. 输 **[!UICONTROL 入文]** 件夹的 **[!UICONTROL 标题]** 和名称 **[!UICONTROL ，并标记复选框“资]**产贡献”。
建议使用没有空格的小字母来命名文件夹。
1. 单击&#x200B;**[!UICONTROL 创建]**。
   ![](assets/create-contribution-folder.png)
1. 您可以在AEM资产存储库中看到新创建的贡献文件夹。
1. 单击打开贡献文件夹，您可以看到两个子文件夹-**[!UICONTROL SHARED]****[!UICONTROL 和NEW]** 在贡献文件夹中自动创建。\
   ![](assets/contribution-folder.png)

您现在可以配置贡献文件夹属性。 请参阅配 [置贡献文件夹属性](brand-portal-configure-contribution-folder-properties.md)。

>[!NOTE]
>
>请确保为贡献文件夹提供适当的名称，因为您在创建后无法修改文件夹名称。