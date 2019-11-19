---
title: 配置贡献文件夹属性
seo-title: 配置贡献文件夹属性
description: '了解如何在AEM资产中配置贡献文件夹的属性。 '
seo-description: '了解如何在AEM资产中配置贡献文件夹的属性。 '
uuid: null
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: f8d95ab1e1c17ef2cf86d0206a36134996e4fe07

---


# 配置贡献文件夹属性 {#configure-contribution-folder-properties}

AEM管理员在配置贡献文件夹的属性时执行以下活动。

* **添加说明**:提供贡献文件夹的高级描述。
* **上传简介**: 上传包含资产相关信息的资产需求文档。
* **添加参与者**:添加Brand Portal用户或用户组，以授予他们对贡献文件夹的访问权限。

资产要求是指管理员为帮助参与者（Brand Portal用户）了解贡献文件夹的需要和要求而提供的详细信息。 管理员上传资产要求文档，其中包含应添加到贡献文件夹的资产类型和资产相关信息（例如用途、图像类型、最大大小等）的简要说明。

然后，管理员可以在将新创建的“贡献”文件夹发布到Brand Portal之前，向Brand Portal用户／组授予对贡献文件夹的访问权限。

**要配置贡献文件夹属性，请执行以下操作：**
1. 登录AEM作者实例默认URL:http://本地主机：4502/aem/start.html
1. 导航到“资 **[!UICONTROL 产”&gt;“文件]** ”，然后找到贡献文件夹。
1. 选择贡献文件夹，然后单击“ **[!UICONTROL 属性]** ” ![](assets/properties.png)。 “文件夹属性”(Folder properties)窗口打开。
   ![](assets/contribution-folder-property1.png)
1. 导航到“资 **[!UICONTROL 产贡献]** ”选项卡。
1. 输入贡献文 **[!UICONTROL 件夹的]** “高级说明”。
1. 单击 **[!UICONTROL 上传摘要]** ，从本地计算机浏览并上传 ![](assets/upload.png) 资产需求文档 ****。
1. 在“ **[!UICONTROL 添加用户或组]**”中，搜索和 **[!UICONTROL 添加Brand]** Portal用户或要与其共享贡献文件夹的组。
这些Brand Portal用户／组将具有访问贡献文件夹和从其Brand Portal界面上传内容的权限，无需访问AEM作者实例。
1. Click **[!UICONTROL Save]**.
   ![](assets/contribution-folder-property2.png)

>[!NOTE]
>
>搜索结果基于在AEM资产中配置的Brand Portal用户列表。 确保您有更新的Brand Portal用户列表。 请参阅， [上传Brand Portal用户列表](brand-portal-configure-asset-sourcing.md)。