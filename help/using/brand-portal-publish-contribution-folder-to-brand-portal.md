---
title: 配置贡献文件夹并将其从Experience Manager Assets发布到Brand Portal
description: 通过insight配置贡献文件夹并将其从Experience Manager Assets发布到Brand Portal。
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
exl-id: 9acad588-977a-45de-b544-f2cc8874ba12
source-git-commit: 8cde9e84262e25ff22d5b2d06e3c5df9cc2ae557
workflow-type: tm+mt
source-wordcount: '1057'
ht-degree: 1%

---

# 在 Experience Manager Assets 中配置贡献文件夹 {#configure-contribution-folder}

对于协作资源源，Experience Manager Assets用户（具有权限的管理员和非管理员用户）可以创建类型为&#x200B;**资源贡献**&#x200B;的文件夹，确保创建的文件夹可供Brand Portal用户提交资源。  此方法会自动触发一个工作流，该工作流在新创建的&#x200B;**Contribution**&#x200B;文件夹中创建两个名为&#x200B;**SHARED**&#x200B;和&#x200B;**NEW**&#x200B;的子文件夹。

Experience Manager Assets用户通过上传有关应添加到贡献文件夹的资源类型的简短信息来定义资源要求。 此外，他们还会将一组基线资产上传到共享文件夹，以确保Brand Portal用户获得所需的信息。 随后，管理员可以向活动Brand Portal用户授予对贡献文件夹的访问权限，然后再将新创建的Contribution文件夹发布到Brand Portal。

以下视频演示了如何在Experience Manager Assets中配置Contribution文件夹：

>[!VIDEO](https://video.tv.adobe.com/v/30547)

Experience Manager Assets用户在配置贡献文件夹时执行以下操作：

* [创建贡献文件夹](#create-contribution-folder)
* [上传资源要求并分配参与者](#configure-contribution-folder-properties)
* [上载基线资源](#uplad-new-assets-to-contribution-folder)
* [将贡献文件夹从Experience Manager Assets发布到Brand Portal](#publish-contribution-folder-to-brand-portal)

## 创建贡献文件夹 {#create-contribution-folder}

Experience Manager Assets管理员和具有创建新文件夹权限的非管理员用户可以在Experience Manager Assets中创建“贡献”文件夹。
要创建贡献文件夹，请创建一个资源贡献类型的文件夹，以确保创建的文件夹可供Brand Portal用户提交资源。 此方法会自动触发一个工作流，该工作流会在contribution文件夹中创建两个额外的子文件夹，分别称为SHARED和NEW。

>[!NOTE]
>
>管理员可以在一个文件夹中创建多个资产贡献文件夹。
>
>资产贡献文件夹包含用于资产分发和贡献的NEW和SHARED文件夹。 请勿在贡献文件夹中创建资产文件夹或贡献文件夹。


您可以在创建贡献文件夹时单独配置贡献文件夹属性。 在本例中，这些属性是单独配置的。

**要创建贡献文件夹：**

1. 登录到您的Experience Manager Assets实例。

1. 导航到&#x200B;**[!UICONTROL Assets]** > **[!UICONTROL 文件]**。 它列出了Experience Manager Assets存储库中的所有现有文件夹。

1. 单击&#x200B;**[!UICONTROL 创建]**&#x200B;以创建新文件夹。 **[!UICONTROL 创建文件夹]**&#x200B;对话框打开。

1. 输入文件夹的&#x200B;**[!UICONTROL Title]**&#x200B;和&#x200B;**[!UICONTROL Name]**，然后选择&#x200B;**[!UICONTROL 资产贡献]**&#x200B;复选框。
Adobe建议您使用小写字母来命名文件夹，且不要留任何空格。

1. 单击&#x200B;**[!UICONTROL 创建]**。您可以看到Experience Manager Assets存储库中列出的贡献文件夹。

   >[!NOTE]
   >
   > * 源文件夹不能为空，并且必须至少包含一个资源，因为无法将空文件夹从Brand Portal发布到AEM。
   > * 非管理员用户可以创建和共享资产贡献文件夹，但无法修改或删除它。


   ![](assets/create-contribution-folder.png)

1. 打开贡献文件夹。 您可以看到在贡献文件夹中自动创建的两个子文件夹 — **[!UICONTROL SHARED]**&#x200B;和&#x200B;**[!UICONTROL NEW]**。

   ![](assets/contribution-folder.png)


## 配置贡献文件夹属性 {#configure-contribution-folder-properties}

Experience Manager Assets管理员在配置“贡献”文件夹的属性时执行以下操作。

* **添加描述**：提供贡献文件夹的高级别描述。
* **上载摘要**：上载包含资产相关信息的资产需求文档。
* **添加参与者**：添加Brand Portal用户，以授予他们访问贡献文件夹的权限。

资源要求是指管理员为帮助参与者(Brand Portal用户)了解贡献文件夹的需要和要求而提供的详细信息。 管理员会上传一个资源需求文档，其中详细介绍了contribution文件夹的资源类型，包括用途、图像类型和最大大小。

**要配置贡献文件夹属性：**

1. 登录到您的Experience Manager Assets实例。

1. 导航到&#x200B;**[!UICONTROL Assets > Files]**，然后找到贡献文件夹。
1. 选择贡献文件夹并单击&#x200B;**[!UICONTROL 属性]**&#x200B;以打开文件夹属性窗口。

   ![](assets/properties.png)

   ![](assets/contribution-folder-property1.png)

1. 导航到&#x200B;**[!UICONTROL 资产贡献]**&#x200B;选项卡。
1. 输入贡献文件夹的高级别的&#x200B;**[!UICONTROL 描述]**。
1. 单击&#x200B;**[!UICONTROL 上载摘要]**&#x200B;从本地计算机浏览并上载&#x200B;**资产要求文档**。

   ![](assets/upload.png)

1. 在&#x200B;**[!UICONTROL 添加用户]**&#x200B;字段中，添加要与其共享贡献文件夹的Brand Portal用户。 这些用户可以使用Brand Portal界面访问内容并将其上传到贡献文件夹。
1. 单击&#x200B;**[!UICONTROL 保存]**。

   ![](assets/contribution-folder-property3.png)

>[!NOTE]
>
>搜索结果基于Experience Manager Assets中配置的Brand Portal用户列表。 确保您拥有更新的Brand Portal用户列表。

管理员可以从`user.csv`下载[!DNL Admin Console]文件，并将其用作添加Brand Portal用户的基础模板。 转到[!UICONTROL 用户]并单击[!UICONTROL 将用户列表导出到csv]选项以下载`users.csv`文件。 以下示例用户详细列出了添加用户所需的属性。 用户条目的唯一强制属性是`Email`，而所有其他属性都是可选的。

[获取文件](assets/users.csv)

## 将资产上传到贡献文件夹 {#uplad-new-assets-to-contribution-folder}

Experience Manager Assets用户将一组基线资源上传到&#x200B;**SHARED**&#x200B;文件夹，以确保Brand Portal用户获得所需的信息。

**要上载基线资源：**

1. 登录到您的Experience Manager Assets实例。

1. 导航到&#x200B;**[!UICONTROL Assets > Files]**，然后找到贡献文件夹。

1. 选择贡献文件夹并单击以将其打开。

1. 单击&#x200B;**[!UICONTROL 新建]**&#x200B;文件夹。

   ![](assets/upload-new-assets1.png)

1. 单击&#x200B;**[!UICONTROL 创建]** > **[!UICONTROL 文件]**&#x200B;以上传单个文件或包含多个资产的文件夹(.zip)。

   ![](assets/upload-new-assets2.png)

1. 浏览资源（文件或文件夹）并将其上载到&#x200B;**[!UICONTROL NEW]**&#x200B;文件夹。

   ![](assets/upload-asset4.png)

将所有资源或文件夹上传到NEW文件夹后，将贡献文件夹发布到Experience Manager Assets。


## 将贡献文件夹发布到Brand Portal {#publish-contribution-folder-to-brand-portal}

配置贡献文件夹后，Experience Manager Assets用户（管理员/非管理员用户）可以将贡献文件夹从Experience Manager Assets发布到Brand Portal。 有权访问contribution文件夹的Brand Portal用户，会在发布操作完成后收到电子邮件或脉冲通知。


**要发布贡献文件夹：**

1. 登录到您的Experience Manager Assets实例。

1. 导航到&#x200B;**[!UICONTROL Assets > “文件”]**，然后找到要在其中发布到Brand Portal的贡献文件夹。
1. 选择一个贡献文件夹，然后单击&#x200B;**[!UICONTROL 快速发布]** > **[!UICONTROL 发布到Brand Portal]**。

   ![](assets/publish-contribution-folder-to-bp.png)

   在将contribution文件夹发布到Brand Portal后，您将收到一条成功消息。

会向分配给contribution文件夹的Brand Portal用户发送电子邮件/脉冲通知。 Brand Portal用户可以访问贡献文件夹并开始贡献。 查看[将资源上传到贡献文件夹并发布到Experience Manager Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)。
