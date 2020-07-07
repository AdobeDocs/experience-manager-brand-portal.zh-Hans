---
title: 下载资产
seo-title: 下载资产
description: 所有用户可以同时下载可供他们访问的多个资产和文件夹。 这样，可安全地分发获准的品牌资产以供离线使用。
seo-description: 所有用户可以同时下载可供他们访问的多个资产和文件夹。 这样，可安全地分发获准的品牌资产以供离线使用。
uuid: 4b57118e-a76e-4d8a-992a-cb3c3097bc03
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: download-install
discoiquuid: f90c2214-beea-4695-9102-8b952bc9fd17
translation-type: tm+mt
source-git-commit: b41f86824afd5be043c7b91035b01b71fdb69a26
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 1%

---


# 下载资产 {#download-assets}

所有用户都可以同时下载可以从Brand Portal访问的多个资产和文件夹。 这样，可安全地分发获准的品牌资产以供离线使用。 阅读相关内容，了解如何从Brand Portal下载获准的资产，以及下载性能 [的预期](../using/brand-portal-download-users.md#main-pars-header)。

>[!NOTE]
>
>只有管理员才能下载过期的资产。 有关过期资产的更多信息，请参 [阅管理资产的数字权限](../using/manage-digital-rights-of-assets.md)。

## 下载资源的步骤 {#steps-to-download-assets}

要下载包含Brand Portal资产的资产或文件夹，请执行以下步骤：

1. 从Brand Portal界面，执行下列操作之一：

   * 选择要下载的文件夹或资产。 在顶部的工具栏中，单击“下 **[!UICONTROL 载]** ”图标。
   ![](assets/downloadassets-1.png)

   * 要下载单个文件夹或资产，请将指针悬停在该文件夹或资产上方。 在可用的快速操作缩略图中，单击“下 **[!UICONTROL 载]** ”图标。
   ![](assets/downloadsingleasset-1.png)

   >[!NOTE]
   >
   >如果您正在下载的资产也包含许可的资产，则会将您重定向到版权 **[!UICONTROL 管理页]** 面。 在此页中，选择资产，单击“ **[!UICONTROL 同意]**”，然后单击“ **[!UICONTROL 下载]**”。 如果您选择不同意，则不会下载许可的资产。\
   >受许可证保护的资 [产附加了许](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) 可证协议 [，可通过在AEM Assets中设置资产的元](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) 数据属性。

   ![](assets/licensed-asset-download-1.png)

   随后 **[!UICONTROL 将出现]** “下载”对话 **[!UICONTROL 框，默认情况下会选]** 择“资产”选项。

   ![](assets/donload-assets-dialog-1.png)

   >[!NOTE]
   >
   >如果您正在下载的资产是图像文件，并且您仅在“下载”对话框中选择 **[!UICONTROL “资产]** ”选项，但管理员未授权您访问图像文件的原始演绎版 [](../using/brand-portal-adding-users.md#main-pars-procedure-202029708) ，则不会下载任何图像文件，并出现通知提示，指出管理员已限制您访问原始演绎版。

   ![](assets/restrictaccess-note.png)

1. 要下载资产的演绎版以及资产，请选 **[!UICONTROL 择演绎版]**。 但是，要允许自动生成的演绎版与自定义演绎版一起下载，请取消选 **[!UICONTROL 择“排除自动生成的演绎版]**”（默认情况下为选中状态）。

   ![](assets/exclude-auto-renditions.png)

   要仅下载演绎版，请取 **[!UICONTROL 消选择资产]**。

   >[!NOTE]
   >
   >默认情况下，仅下载资产。 但是，如果管理员未授权您访问图像文 [件的原始演绎版，则不会下载图像文件的原始演绎版](../using/brand-portal-adding-users.md#main-pars-procedure-202029708)。

   * 要加快从Brand Portal下载资产文件的速度，请选择“启 **[!UICONTROL 用下载加速]** ”选项 [，然后按向导操作](../using/accelerated-download.md#main-pars-header-405749062)。 要进一步了解如何更快地下载资产，请参 [阅指南以加速从Brand Portal下载](../using/accelerated-download.md)。

   * 要将自定 [义图像预设应用到资产及其演绎版](../using/brand-portal-image-presets.md#applyimagepresetswhendownloadingimages)，请 **[!UICONTROL 选择动态演绎版]**。 指定自定义图像预设属性（大小、格式、色彩空间、分辨率和图像修饰符），以便在下载资产及其演绎版时应用自定义图像预设。 要仅下载动态演绎版，请 **[!UICONTROL 删除资产]**。
   ![](assets/dynamic-renditions.png)

   >[!NOTE]
   >
   >要预览（或下载）任何资产的动态演绎版，请确保已启用Dynamic Media，且资产的金字塔tiff演绎版存在于AEM作者实例中（从中发布资产）。 将资产发布到Brand Portal时，也会发布其金字塔tiff再现。 无法从Brand Portal生成金字塔tiff再现。

   * 要在下载资产时保留Brand Portal文件夹层次结构，请选 **[!UICONTROL 择为每个资产创建单独的文件夹]**。 默认情况下，将忽略Brand Portal文件夹层次结构，所有资产都下载到本地系统的一个文件夹中。

   * 要向用户发送包含下载资产链接的电子邮件通知，请选择“电 **[!UICONTROL 子邮件]**”。
   ![](assets/download-link.png)

   >[!NOTE]
   >
   >电子邮件通知的下载链接在45天后过期。
   >
   >管理员可以使用品牌功能自定义电子邮件，即徽标、说明 [和页脚](../using/brand-portal-branding.md) 。

1. 单击“ **[!UICONTROL 下载]**”。

   资产（如果已选择，则会将演绎版）作为ZIP文件下载到您的本地文件夹。 但是，如果下载单个资产时不包含任何演绎版，则不会创建zip文件，从而确保快速下载。

   如果管理员未授权您访问原始演绎版，则不 [会下载选定资产的原始演绎版](../using/brand-portal-adding-users.md#main-pars-procedure-202029708)。

   >[!NOTE]
   >
   >单独选择和下载的资产会显示在下载的资产报告中。 但是，如果下载的文件夹中包含资产，则下载的资产报告中不会显示该文件夹和资产。

   要了解如何从共享链接下载资产，请参阅从 [共享链接下载资产](../using/brand-portal-link-share.md#main-pars-header-1703469193)。

## 预期下载性能 {#expected-download-performance}

不同客户端位置的用户的文件下载体验可能不同，具体取决于诸如本地Internet连接和服务器延迟等因素。 在不同客户端位置观察到的2 GB文件的预期下载性能如下：

| 客户端位置 | 客户端与服务器之间的延迟 | 预期下载速度 | 下载2 GB文件所花费的时间 |
|-------------------------|-----------------------------------|-------------------------|------------------------------------|
| 美国西部（加利福尼亚北部） | 18毫秒 | 7.68 MB/秒 | 4分钟 |
| 美国西部（俄勒冈） | 42毫秒 | 3.84 MB/秒 | 9分钟 |
| 美国东部（弗吉尼亚北部） | 85毫秒 | 1.61 MB/秒 | 21分钟 |
| APAC（东京） | 124毫秒 | 1.13 MB/秒 | 30 分钟 |
| 诺伊达 | 275毫秒 | 0.5 MB/s | 68分钟 |
| 悉尼 | 175毫秒 | 0.49 MB/秒 | 69分钟 |
| 伦敦 | 179毫秒 | 0.32 MB/秒 | 106分钟 |
| 新加坡 | 196毫秒 | 0.5 MB/s | 68分钟 |

**注意**: 在测试条件下观察引用的数据，这可能因不同位置的用户目睹不同的延迟和带宽而异。
