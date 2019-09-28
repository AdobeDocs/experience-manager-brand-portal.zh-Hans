---
title: 下载资源
seo-title: 下载资源
description: 所有用户可以同时下载可供他们访问的多个资产和文件夹。 这样，获准的品牌资产便可以安全地分发以供脱机使用。
seo-description: 所有用户可以同时下载可供他们访问的多个资产和文件夹。 这样，获准的品牌资产便可以安全地分发以供脱机使用。
uuid: 4b57118e-a76e-4d8a-992a-cb3c3097bc03
content-type: 引用
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: 下载安装
discoiquuid: f90c2214-beea-4695-9102-8b952bc9fd17
translation-type: tm+mt
source-git-commit: 86d4d5c358ea795e35db2dce8c9529ed14e9ee2d

---


# 下载资源 {#download-assets}

所有用户都可以同时从Brand Portal下载可供他们访问的多个资产和文件夹。 这样，获准的品牌资产便可以安全地分发以供脱机使用。 继续阅读，了解如何从Brand Portal下载获准的资产，以及下载性能将带来 [的期待](../using/brand-portal-download-users.md#main-pars-header)。

>[!NOTE]
>
>只有管理员才能下载过期的资产。 有关过期资产的详细信息，请参 [阅管理资产的数字权限](../using/manage-digital-rights-of-assets.md)。

## 下载资产的步骤 {#steps-to-download-assets}

要下载Brand Portal中包含资产的资产或文件夹，请执行以下步骤：

1. 从Brand Portal界面中，执行以下操作之一：

   * 选择要下载的文件夹或资产。 在顶部的工具栏中，单击“下载 **[!UICONTROL ”图]** 标。
   ![](assets/downloadassets-1.png)

   * 要下载单个文件夹或资产，请将指针悬停在该文件夹或资产上。 从可用的快速操作缩略图中，单击“下 **[!UICONTROL 载]** ”图标。
   ![](assets/downloadsingleasset-1.png)

   >[!NOTE]
   >
   >如果您正在下载的资产也包括许可的资产，您会被重定向到“版权 **[!UICONTROL 管理]** ”页面。 在此页中，选择资产，单击“ **[!UICONTROL 同意]**”，然后单击“ **[!UICONTROL 下载]**”。 如果您选择不同意，则不会下载许可的资产。\
   >受许可证保护的资 [产附加了许可协议](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) ，可通过在AEM资产中设置资产的元数据属 [性](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) 来完成此操作。

   ![](assets/licensed-asset-download-1.png)

   随后 **[!UICONTROL 将出现]** “下载 **[!UICONTROL ”对话框，默]** 认情况下会选中“资产”选项。

   ![](assets/donload-assets-dialog-1.png)

   >[!NOTE]
   >
   >如果您下载的资产是图像文件，并且您在“下载”对话框中仅选择“资产”选项，但管理员未授权其访问图像文件的原始演绎版 ****[](../using/brand-portal-adding-users.md#main-pars-procedure-202029708) ，则不会下载任何图像文件，并会显示“声明”提示，指出您已被管理员限制访问原始演绎版。

   ![](assets/restrictaccess-note.png)

1. 要下载资产的演绎版以及资产，请选择“ **[!UICONTROL 演绎版”]**。 However, to allow auto-generated renditions to download along with custom renditions, deselect Exclude Auto Generated Renditions, which is selected by default.****

   ![](assets/exclude-auto-renditions.png)

   To download only the renditions, deselect **[!UICONTROL Asset(s)]**.

   >[!NOTE]
   >
   >By default, only the assets are downloaded. However, original renditions of image files are not downloaded if you are not authorized by the administrator to have access to the original renditions of image files.[](../using/brand-portal-adding-users.md#main-pars-procedure-202029708)

   * To speed up the download of asset files from Brand Portal, select Enable download acceleration option and follow the wizard. ****[](../using/accelerated-download.md#main-pars-header-405749062)To know more about faster download of assets refer guide to accelerate downloads from Brand Portal.[](../using/accelerated-download.md)

   * To apply a custom image preset to the asset and its renditions, select Dynamic Rendition(s). [](../using/brand-portal-image-presets.md#applyimagepresetswhendownloadingimages)**** Specify custom image preset properties (size, format, color space, resolution, and image modifier) to apply the custom image preset while downloading the asset and its renditions. To download only the dynamic renditions, delesect Asset(s).****
   ![](assets/dynamic-renditions.png)

   >[!NOTE]
   >
   >To preview (or download) dynamic renditions of any asset, ensure that the dynamic media is enabled and the asset's Pyramid tiff rendition exists at the AEM author instance, from where the assets have been published. When an asset is published to Brand Portal, its Pyramid tiff rendition is also published. 无法从Brand Portal生成金字塔tiff再现。

   * To preserve the Brand Portal folder hierarchy while downloading assets, select Create separate folder for each asset. **** By default, Brand Portal folder hierarchy is ignored and all assets are downloaded in one folder in your local system.

   * To send an email notification to users with a link for downloading the assets, select Email.****
   ![](assets/download-link.png)

   >[!NOTE]
   >
   >Download link on email notification expires after 45 days.
   >
   >管理员可以使用品牌功能自定义电子邮件，即徽标、说明和页 [脚](../using/brand-portal-branding.md) 。

1. 单击“ **[!UICONTROL 下载]**”。

   资产（如果已选择，则会将演绎版）作为ZIP文件下载到您的本地文件夹。 但是，如果下载单个资产而不下载任何演绎版，则不会创建zip文件，从而确保快速下载。

   如果管理员未授权您访问原始演绎版，则不 [会下载选定资产的原始演绎版](../using/brand-portal-adding-users.md#main-pars-procedure-202029708)。

   >[!NOTE]
   >
   >单独选择和下载的资产会显示在已下载的资产报告中。 但是，如果下载了包含资产的文件夹，则下载的资产报告中既不显示该文件夹，也不显示资产。

   要了解如何从共享链接下载资产，请参阅从 [共享链接下载资产](../using/brand-portal-link-share.md#main-pars-header-1703469193)。

## 预期下载性能 {#expected-download-performance}

文件下载体验可能因不同客户端位置的用户而异，具体取决于诸如本地Internet连接和服务器延迟等因素。 在不同客户端位置观察到的2 GB文件的预期下载性能如下： Brand Portal服务器位于美国俄勒冈州：

| 客户端位置 | 客户端与服务器之间的延迟 | 预期下载速度 | 下载2 GB文件所花费的时间 |
|-------------------------|-----------------------------------|-------------------------|------------------------------------|
| 美国西部（北美）加利福尼亚) | 18毫秒 | 7.68 MB/秒 | 4分钟 |
| 美国西部（俄勒冈） | 42毫秒 | 3.84 MB/秒 | 9分钟 |
| 美国东部（北美）维吉尼亚) | 85毫秒 | 1.61 MB/秒 | 21分钟 |
| APAC（东京） | 124毫秒 | 1.13 MB/秒 | 30 分钟 |
| 诺伊达 | 275毫秒 | 0.5 MB/s | 68分钟 |
| 悉尼 | 175毫秒 | 0.49 MB/秒 | 69分钟 |
| 伦敦 | 179毫秒 | 0.32 MB/秒 | 106 minutes |
| 新加坡 | 196 milliseconds | 0.5 MB/s | 68分钟 |

**Note: Cited data are observed under test conditions, which may vary for users at different locations witnessing varied latency and bandwidth.**
