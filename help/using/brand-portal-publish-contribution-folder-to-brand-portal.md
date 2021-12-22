---
title: '配置贡献文件夹并将其从Experience Manager Assets发布到Brand Portal '
seo-title: Configure and publish contribution folder from Experience Manager Assets to Brand Portal
description: 深入了解如何配置和发布从Experience Manager Assets到Brand Portal的贡献文件夹。
seo-description: Get an insight into configuring and publishing a contribution folder from Experience Manager Assets to Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 9acad588-977a-45de-b544-f2cc8874ba12
source-git-commit: 3845d9fa17e75d59493383303ca0978349ca0401
workflow-type: tm+mt
source-wordcount: '1037'
ht-degree: 0%

---

# 在Experience Manager Assets中配置Contribution文件夹 {#configure-contribution-folder}

对于协作资产源，Experience Manager Assets用户（具有权限的管理员和非管理员用户）可以创建新类型的文件夹 **资产贡献**，以确保创建的新文件夹对Brand Portal用户提交资产的操作是打开的。  这会自动触发一个创建另外两个子文件夹(称为 **共享** 和 **新建**，在新创建的 **贡献** 文件夹。

然后，Experience Manager Assets用户通过将关于应添加到贡献文件夹的资产类型以及一组基线资产的简报上传到 **共享** 文件夹，以确保Brand Portal用户拥有所需的信息。 然后，管理员可以在将新创建的Contribution文件夹发布到Brand Portal之前，向活动的Brand Portal用户授予对Contribution文件夹的访问权限。

以下视频演示了如何在Experience Manager Assets中配置Contribution文件夹：

>[!VIDEO](https://video.tv.adobe.com/v/30547)

Experience Manager Assets用户在配置贡献文件夹时，会执行以下活动：

* [创建贡献文件夹](#create-contribution-folder)
* [上传资产要求并分配参与者](#configure-contribution-folder-properties)
* [上传基准资产](#uplad-new-assets-to-contribution-folder)
* [将贡献文件夹从Experience Manager Assets发布到Brand Portal](#publish-contribution-folder-to-brand-portal)

## 创建贡献文件夹 {#create-contribution-folder}


Experience Manager Assets管理员和有权创建新文件夹的非管理员用户可以在Experience Manager Assets中创建贡献文件夹。
要创建贡献文件夹，请创建一个类型为“资产贡献”的新文件夹，并确保创建的新文件夹已打开，可供Brand Portal用户提交资产。  这会自动触发一个工作流，该工作流会在贡献文件夹内创建另外两个子文件夹，称为SHARED和NEW。


>[!NOTE]
>
>管理员可以在一个文件夹中创建多个资产贡献文件夹。
>
>资产贡献文件夹包含用于资产分发和贡献的新文件夹和共享文件夹。 请勿在贡献文件夹中创建资产、文件夹或贡献文件夹。


您可以在创建贡献文件夹时，分别配置贡献文件夹属性。 在本例中，我们将分别配置这些属性。

**要创建贡献文件夹，请执行以下操作：**

1. 登录到Experience Manager Assets实例。

1. 导航到 **[!UICONTROL 资产]** > **[!UICONTROL 文件]**. 它列出了Experience Manager Assets存储库中的所有现有文件夹。

1. 单击 **[!UICONTROL 创建]** 创建新文件夹。 **[!UICONTROL 创建文件夹]** 对话框。

1. 输入 **[!UICONTROL 标题]** 和 **[!UICONTROL 名称]** ，然后选择 **[!UICONTROL 资产贡献]** 复选框。
建议使用不带任何空格的小写字母来命名文件夹。

1. 单击&#x200B;**[!UICONTROL 创建]**。您可以在Experience Manager Assets存储库中看到列出的贡献文件夹。

   >[!NOTE]
   >
   >非管理员用户可以创建和共享资产贡献文件夹，但无法对其进行修改或删除。


   ![](assets/create-contribution-folder.png)

1. 单击以打开贡献文件夹，您可以看到两个子文件夹 — **[!UICONTROL 共享]** 和 **[!UICONTROL 新建]** 将在贡献文件夹中自动创建。

   ![](assets/contribution-folder.png)


## 配置贡献文件夹属性 {#configure-contribution-folder-properties}

Experience Manager Assets管理员在配置贡献文件夹的属性时，会执行以下活动。

* **添加描述**:提供贡献文件夹的高级描述。
* **上传摘要**:上传包含资产相关信息的资产需求文档。
* **添加参与者**:添加Brand Portal用户以授予他们访问贡献文件夹的权限。

资产要求是指管理员为帮助参与者(Brand Portal用户)了解贡献文件夹的需要和要求而提供的详细信息。 管理员上传资产要求文档，其中包含应添加到贡献文件夹的资产类型以及与资产相关的信息（例如用途、图像类型、最大大小等）的简短说明。

**要配置贡献文件夹属性，请执行以下操作：**

1. 登录到Experience Manager Assets实例。

1. 导航到 **[!UICONTROL 资产>文件]** 并找到贡献文件夹。
1. 选择贡献文件夹并单击 **[!UICONTROL 属性]** 打开“文件夹属性”窗口。

   ![](assets/properties.png)

   ![](assets/contribution-folder-property1.png)

1. 导航到 **[!UICONTROL 资产贡献]** 选项卡。
1. 进入高级 **[!UICONTROL 描述]** 的子目录访问Advertising Cloud帮助。
1. 单击 **[!UICONTROL 上传摘要]** 从本地计算机浏览并上传 **资产需求文档**.

   ![](assets/upload.png)

1. 在 **[!UICONTROL 添加用户]** 字段中，添加要与其共享贡献文件夹的Brand Portal用户。 这些用户可以使用Brand Portal界面访问内容并将内容上传到Contribution文件夹。
1. 单击&#x200B;**[!UICONTROL 保存]**。

   ![](assets/contribution-folder-property3.png)

>[!NOTE]
>
>搜索结果基于在Experience Manager Assets中配置的Brand Portal用户列表。 确保您已更新Brand Portal用户列表。

管理员可以下载 `user.csv` 文件来源 [!DNL Admin Console] 并将其用作添加Brand Portal用户的基本模板。 转到 [!UICONTROL 用户] 并单击 [!UICONTROL 将用户列表导出到csv] 下载选项 `users.csv` 文件。 以下示例用户列表详细介绍了添加用户所需的属性。 用户条目的唯一必需属性是 `Email` 而所有其他属性都是可选的。

[获取文件](assets/users.csv)

## 将资产上传到贡献文件夹 {#uplad-new-assets-to-contribution-folder}

Experience Manager Assets用户将一组基准资产上传到 **共享** 文件夹，以确保Brand Portal用户拥有所需的信息。

**要上传基线资产，请执行以下操作：**

1. 登录到Experience Manager Assets实例。

1. 导航到 **[!UICONTROL 资产>文件]** 并找到贡献文件夹。

1. 选择贡献文件夹，然后单击以将其打开。

1. 单击 **[!UICONTROL 新建]** 文件夹。

   ![](assets/upload-new-assets1.png)

1. 单击 **[!UICONTROL 创建]** > **[!UICONTROL 文件]** 上传包含多个资产的单个文件或文件夹(.zip)。

   ![](assets/upload-new-assets2.png)

1. 浏览资产（文件或文件夹）并将其上传到 **[!UICONTROL 新建]** 文件夹。

   ![](assets/upload-asset4.png)

将所有资产或文件夹上传到NEW文件夹后，将Contribution文件夹发布到Experience Manager Assets。


## 将贡献文件夹发布到Brand Portal {#publish-contribution-folder-to-brand-portal}

配置贡献文件夹后，Experience Manager Assets用户（管理员/非管理员用户）可以将贡献文件夹从Experience Manager Assets发布到Brand Portal。 具有访问贡献文件夹权限的Brand Portal用户将在发布操作完成时收到电子邮件/脉冲通知。


**要发布贡献文件夹，请执行以下操作：**

1. 登录到Experience Manager Assets实例。

1. 导航到 **[!UICONTROL 资产>文件]** 并找到要在其中发布到Brand Portal的贡献文件夹。
1. 选择贡献文件夹并单击 **[!UICONTROL 快速发布]** > **[!UICONTROL 发布到Brand Portal]**.

   ![](assets/publish-contribution-folder-to-bp.png)

   将贡献文件夹发布到Brand Portal后，您将收到一条成功消息。

电子邮件/脉冲通知会发送给分配到贡献文件夹的Brand Portal用户。 Brand Portal用户可以访问贡献文件夹并开始贡献。 看， [将资产上传到Contribution文件夹并发布到Experience Manager Assets](brand-portal-publish-contribution-folder-to-aem-assets.md).
