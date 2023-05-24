---
title: 自定义墙纸、标题和电子邮件消息
seo-title: Customize wallpaper, header, and email message
description: Brand Portal管理员可以对向用户显示的界面进行有限的自定义。 您可以为Brand Portal登录页面选择特定的背景图像（壁纸）。 您还可以添加页眉图像并自定义资产共享电子邮件以匹配客户的品牌。
seo-description: Brand Portal administrators can make limited customizations to the interface displayed to users. You can choose a specific background image (wallpaper) for the Brand Portal login page. You can also add a header image and customize asset sharing emails to match the customer’s brand.
uuid: e078d0b9-18b5-467a-ae90-7f0b9fd0d414
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: administration
discoiquuid: 7b573a4f-2d4e-48d6-b259-436d0cfbdce9
role: Admin
exl-id: 9f5c2a6a-8844-4ca4-b0d9-8f50b6164219
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 2%

---

# 自定义墙纸、标题和电子邮件消息 {#customize-wallpaper-header-and-email-message}

Brand Portal管理员可以对向用户显示的界面进行有限的自定义。 您可以为Brand Portal登录页面选择特定的背景图像（壁纸）。 您还可以添加页眉图像并自定义资产共享电子邮件以匹配客户的品牌。

## 自定义登录屏幕壁纸 {#customize-the-login-screen-wallpaper}

如果缺少自定义品牌壁纸图像，则登录页面上会显示默认壁纸。

1. 在顶部的工具栏中，单击Experience Manager徽标以访问管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，单击 **[!UICONTROL 品牌化]**.


   ![](assets/admin-tools-panel-10.png)

1. 在左侧边栏上 **[!UICONTROL 配置品牌]** 页面， **[!UICONTROL 壁纸]** 默认情况下处于选中状态。 将显示登录页面上显示的默认背景图像。

   ![](assets/default_wallpaper.png)

1. 要添加新背景图像，请单击 **[!UICONTROL 选择图像]** 图标。

   ![](assets/choose_wallpaperimage.png)

   执行下列操作之一：

   * 要从计算机上传图像，请单击 **[!UICONTROL 上传]**. 导航到所需的图像并将其上传。
   * 要使用现有Brand Portal图像，请单击 **[!UICONTROL 从现有中选择]**. 使用资产选取器选择图像。

   ![](assets/asset-picker.png)

1. 指定背景图像的标题文本和描述。 要保存更改，请单击 **[!UICONTROL 保存]** 从顶部的工具栏中。

1. 在顶部的工具栏中，单击 **[!UICONTROL 预览]** 图标以生成包含图像的Brand Portal界面预览。

   ![](assets/chlimage_1.png)

   ![](assets/custom-wallpaper-preview.png)

1. 要激活或取消激活默认壁纸，请在 **[!UICONTROL 配置品牌>壁纸]** 页面：

   * 要在Brand Portal登录页面上显示默认壁纸图像，请单击 **[!UICONTROL 停用壁纸]** 从顶部的工具栏中。 将显示一条消息，确认自定义图像已停用。

   ![](assets/chlimage_1-1.png)

   * 要在Brand Portal登录页面上还原自定义映像，请单击 **[!UICONTROL 激活壁纸]** 工具栏中。 将显示一条消息，确认图像已恢复。

   ![](assets/chlimage_1-2.png)

   * 单击 **[!UICONTROL 保存]** 以保存更改。



## 自定义标题 {#customize-the-header}

登录Brand Portal后，标题会显示在各种Brand Portal页面上。

1. 在顶部的工具栏中，单击Experience Manager徽标以访问管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，单击 **[!UICONTROL 品牌化]**.

   ![](assets/admin-tools-panel-11.png)

1. 要自定义Brand Portal界面的页眉，请在 **[!UICONTROL 配置品牌]** 页面，选择 **[!UICONTROL 页眉图像]** 从左边栏开始。 将显示默认页眉图像。

   ![](assets/default-header.png)

1. 要上传页眉图像，请单击 **[!UICONTROL 选择图像]** 图标并选择 **[!UICONTROL 上传]**.

   要使用现有Brand Portal图像，请选择 **[!UICONTROL 从现有中选择]**.

   ![](assets/choose_wallpaperimage-1.png)

   使用资产选取器选择图像。

   ![](assets/asset-picker-header.png)

1. 要在标题图像中包含某个URL，请在 **[!UICONTROL 图像URL]** 盒子。 您可以指定外部或内部URL。 内部链接也可以是相对链接，例如，
   [!UICONTROL `/mediaportal.html/content/dam/mac/tenant_id/tags`].
此链接会将用户定向到tags文件夹。
要保存更改，请单击 **[!UICONTROL 保存]** 从顶部的工具栏中。

   ![](assets/configure_brandingheaderimageurl.png)

1. 在顶部的工具栏中，单击 **[!UICONTROL 预览]** 图标以生成包含标题图像的Brand Portal界面预览。

   ![](assets/chlimage_1-3.png)
   ![](assets/custom_header_preview.png)

1. 要激活或取消激活页眉图像，请在 **[!UICONTROL 配置品牌>页眉图像]** 页面：

   * 要防止标题图像出现在Brand Portal页面上，请单击 **[!UICONTROL 停用标题]** 从顶部的工具栏中。 将显示一条消息，确认图像已停用。

   ![](assets/chlimage_1-4.png)

   * 要使标题图像重新显示在Brand Portal页面上，请单击 **[!UICONTROL 激活标题]** 从顶部的工具栏中。 将显示一条消息，确认图像已激活。

   ![](assets/chlimage_1-5.png)

   * 单击 **[!UICONTROL 保存]** 以保存更改。



## 自定义电子邮件消息 {#customize-the-email-messaging}

将资产作为链接共享时，用户会收到一封包含该链接的电子邮件。 管理员可以自定义这些电子邮件的消息，即徽标、描述和页脚。

1. 在顶部的工具栏中，单击Experience Manager徽标以访问管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，单击 **[!UICONTROL 品牌化]**.

   ![](assets/admin-tools-panel-12.png)

1. 将资产作为链接共享或通过电子邮件下载的时间，以及  **[!UICONTROL 收藏集]** 共享，则会向用户发送电子邮件通知。 要自定义电子邮件，请在 **[!UICONTROL 配置品牌]** 页面，选择 **[!UICONTROL 电子邮件]** 从左边栏开始。

   ![](assets/configure-branding-page-email.png)

1. 要将徽标添加到外发电子邮件，请单击 **[!UICONTROL 上传]** 从顶部的工具栏中。

1. 在 **[!UICONTROL 描述]** 部分，指定电子邮件页眉和页脚文本。 要保存更改，请单击 **[!UICONTROL 保存]** 从顶部的工具栏中。

   >[!NOTE]
   >
   >如果您未使用推荐的徽标大小，或者页眉和页脚文本超过推荐的字数，则电子邮件中的内容可能会出现乱码。
