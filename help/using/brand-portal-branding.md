---
title: 自定义壁纸、标题和电子邮件消息
description: Brand Portal管理员可以对向用户显示的界面进行有限的自定义。 您可以为Brand Portal登录页面选择特定的背景图像（墙纸）。 您还可以添加页眉图像并自定义资产共享电子邮件以匹配客户的品牌。
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: administration
role: Admin
exl-id: 9f5c2a6a-8844-4ca4-b0d9-8f50b6164219
source-git-commit: 32a67abf466dd3bf635b851b02377ed23591915e
workflow-type: tm+mt
source-wordcount: '761'
ht-degree: 0%

---

# 自定义壁纸、标题和电子邮件消息 {#customize-wallpaper-header-and-email-message}

Brand Portal管理员可以对向用户显示的界面进行有限的自定义。 您可以为Brand Portal登录页面选择特定的背景图像（墙纸）。 您还可以添加页眉图像并自定义资产共享电子邮件以匹配客户的品牌。

## 自定义登录屏幕壁纸 {#customize-the-login-screen-wallpaper}

如果缺少自定义品牌壁纸图像，则登录页面上将显示默认壁纸。

1. 在顶部的工具栏中，单击Experience Manager徽标以访问管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，单击&#x200B;**[!UICONTROL 品牌]**。

   ![](assets/admin-tools-panel-10.png)

1. 在&#x200B;**[!UICONTROL 配置品牌]**&#x200B;页面的左边栏上，默认选中&#x200B;**[!UICONTROL 壁纸]**。 将显示登录页面上显示的默认背景图像。

   ![](assets/default_wallpaper.png)

1. 要添加新背景图像，请单击顶部工具栏中的&#x200B;**[!UICONTROL 选择图像]**&#x200B;图标。

   ![](assets/choose_wallpaperimage.png)

   执行下列操作之一：

   * 若要从计算机上传图像，请单击&#x200B;**[!UICONTROL 上传]**。 导航到所需的图像并将其上传。
   * 要使用现有Brand Portal映像，请单击&#x200B;**[!UICONTROL 从现有中选择]**。 使用资产选取器选择图像。

   ![](assets/asset-picker.png)

1. 指定背景图像的标题文本和描述。 要保存更改，请单击顶部工具栏中的&#x200B;**[!UICONTROL 保存]**。

1. 在顶部的工具栏中，单击&#x200B;**[!UICONTROL 预览]**&#x200B;图标以生成包含图像的Brand Portal界面预览。

   ![](assets/chlimage_1.png)

   ![](assets/custom-wallpaper-preview.png)

1. 要激活或取消激活默认壁纸，请在&#x200B;**[!UICONTROL 配置品牌>壁纸]**&#x200B;页面中执行以下操作：

   * 要在Brand Portal登录页面上显示默认壁纸图像，请单击顶部工具栏中的&#x200B;**[!UICONTROL 停用壁纸]**。 将显示一条消息，确认自定义图像已停用。

   ![](assets/chlimage_1-1.png)

   * 若要在Brand Portal登录页面上还原自定义图像，请单击工具栏中的&#x200B;**[!UICONTROL 激活壁纸]**。 将显示一条消息，确认图像已恢复。

   ![](assets/chlimage_1-2.png)

   * 单击&#x200B;**[!UICONTROL 保存]**&#x200B;以保存更改。

## 自定义标题 {#customize-the-header}

登录Brand Portal后，标题会显示在各种Brand Portal页面上。

1. 在顶部的工具栏中，单击Experience Manager徽标以访问管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，单击&#x200B;**[!UICONTROL 品牌]**。

   ![](assets/admin-tools-panel-11.png)

1. 要自定义Brand Portal界面的页眉，请在&#x200B;**[!UICONTROL 配置品牌]**&#x200B;页面上从左边栏选择&#x200B;**[!UICONTROL 页眉图像]**。 将显示默认页眉图像。

   ![](assets/default-header.png)

1. 要上传页眉图像，请单击&#x200B;**[!UICONTROL 选择图像]**&#x200B;图标并选择&#x200B;**[!UICONTROL 上传]**。

   要使用现有Brand Portal映像，请选择&#x200B;**[!UICONTROL 选择现有]**。

   ![](assets/choose_wallpaperimage-1.png)

   使用资产选取器选择图像。

   ![](assets/asset-picker-header.png)

1. 要在标题图像中包含某个URL，请在&#x200B;**[!UICONTROL 图像URL]**&#x200B;框中指定该项。 您可以指定外部或内部URL。 内部链接也可以是相对链接，例如，
   [!UICONTROL `/mediaportal.html/content/dam/mac/tenant_id/tags`]。
此链接会将用户定向到tags文件夹。
要保存更改，请单击顶部工具栏中的&#x200B;**[!UICONTROL 保存]**。

   ![](assets/configure_brandingheaderimageurl.png)

1. 在顶部的工具栏中，单击&#x200B;**[!UICONTROL 预览]**&#x200B;图标以生成包含标题图像的Brand Portal界面预览。

   ![](assets/chlimage_1-3.png)
   ![](assets/custom_header_preview.png)

1. 要激活或停用页眉图像，请在&#x200B;**[!UICONTROL 配置品牌>页眉图像]**&#x200B;页面中执行以下操作：

   * 要阻止在Brand Portal页面上显示标题图像，请单击顶部工具栏中的&#x200B;**[!UICONTROL 停用标题]**。 将显示一条消息，确认图像已停用。

   ![](assets/chlimage_1-4.png)

   * 要使标题图像重新出现在Brand Portal页面上，请单击顶部工具栏中的&#x200B;**[!UICONTROL 激活标题]**。 将显示一条消息，确认图像已激活。

   ![](assets/chlimage_1-5.png)

   * 单击&#x200B;**[!UICONTROL 保存]**&#x200B;以保存更改。

## 自定义电子邮件消息 {#customize-the-email-messaging}

在将资产作为链接共享时，用户会收到一封包含该链接的电子邮件。 管理员可以自定义这些电子邮件的消息，即徽标、描述和页脚。

1. 在顶部的工具栏中，单击Experience Manager徽标以访问管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，单击&#x200B;**[!UICONTROL 品牌]**。

   ![](assets/admin-tools-panel-12.png)

1. 当资产作为链接共享或通过电子邮件下载时，以及当共享&#x200B;**[!UICONTROL 收藏集]**&#x200B;时，会向用户发送电子邮件通知。 要自定义电子邮件，请在&#x200B;**[!UICONTROL 配置品牌]**&#x200B;页面上，从左边栏选择&#x200B;**[!UICONTROL 电子邮件]**。

   ![](assets/configure-branding-page-email.png)

1. 若要向传出电子邮件添加徽标，请单击顶部工具栏中的&#x200B;**[!UICONTROL 上传]**。

1. 在&#x200B;**[!UICONTROL 描述]**&#x200B;部分中，指定电子邮件页眉和页脚文本。 要保存更改，请单击顶部工具栏中的&#x200B;**[!UICONTROL 保存]**。

   >[!NOTE]
   >
   >如果您未使用推荐的徽标大小，或者页眉和页脚文本超过了推荐的字数，则电子邮件中的内容可能会出现乱码。
