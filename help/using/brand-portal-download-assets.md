---
title: 下载资产
seo-title: Download assets
description: 所有用户都可以同时下载可供他们访问的多个资产和文件夹。 这样，就可以安全地分发已批准的品牌资产，以便离线使用。
seo-description: All users can simultaneously download multiple assets and folders accessible to them. This way, approved brand assets can be securely distributed for offline use.
uuid: 4b57118e-a76e-4d8a-992a-cb3c3097bc03
content-type: reference
contentOwner: Vishabh Gupta
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: download-install
discoiquuid: f90c2214-beea-4695-9102-8b952bc9fd17
exl-id: be264b1c-38d9-4075-b56a-113f34a2c6bf
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '1924'
ht-degree: 3%

---

# 从  Brand Portal 下载资产 {#download-assets-from-bp}

<!-- Before update in Download experience - 26th Aug 2020 comment by Vishabh.
 All users can simultaneously download multiple assets and folders accessible to them from Brand Portal. This way, approved brand assets can be securely distributed for offline use. Read on to know how to download approved assets from Brand Portal, and what to expect from the [download performance](../using/brand-portal-download-assets.md#main-pars-header).
-->

Adobe Experience Manager Assets Brand Portal允许用户同时从Brand Portal下载可供他们访问的多个资产和文件夹，从而增强了下载体验。 这样，就可以安全地分发已批准的品牌资产，以便离线使用。 阅读并了解如何从Brand Portal下载已批准的资产，以及从[下载性能](../using/brand-portal-download-assets.md#expected-download-performance)中预期获得什么。


>[!NOTE]
>
>在Brand Portal 2020.10.0（及更高版本）中，默认启用&#x200B;**[!UICONTROL Fast Download]**&#x200B;设置，该设置使用IBM Aspera Connect来加速资产下载。 在从Brand Portal下载资产之前，在浏览器的扩展中安装IBM Aspera Connect 3.9.9(`https://www.ibm.com/docs/en/aspera-connect/3.9.9`)。 有关更多详细信息，请参阅[指南以加快从Brand Portal下载的速度](../using/accelerated-download.md)。
>
>如果您不想使用IBM Aspera Connect并继续正常下载过程，请联系Brand Portal管理员以关闭&#x200B;**[!UICONTROL Fast Download]**&#x200B;设置。

## 配置资产下载 {#configure-download}

Brand Portal管理员可以为Brand Portal用户配置资产下载和用户组设置，以便他们能够从Brand Portal界面访问和下载资产演绎版。

>[!NOTE]
>
>应用于用户界面的下载设置有助于Brand Portal用户获得自助体验，从而轻松配置和下载资产演绎版。 它不会限制在应用程序层下载资产，例如，用户仍然可以访问和下载具有完整URL路径的资产演绎版。

从Brand Portal界面访问和下载资产演绎版由以下配置定义：

* 启用下载设置
* 配置用户群组设置

### 启用下载设置 {#enable-download-settings}

管理员可以启用资产&#x200B;**[!UICONTROL 下载设置]**&#x200B;来定义可供Brand Portal用户下载的演绎版集。

可用的设置包括：

* **[!UICONTROL 快速下载]**

   它使用IBM Aspera Connect提供资产的加速下载。 默认情况下，在&#x200B;**[!UICONTROL 下载设置]**&#x200B;中启用&#x200B;**[!UICONTROL 快速下载]**&#x200B;设置。

* **[!UICONTROL 自定义呈现版本]**

   允许下载资产的自定义演绎版和（或）动态演绎版。

   除原始资产和系统生成的演绎版之外的所有资产演绎版都称为自定义演绎版。 它包括可用于资产的静态和动态演绎版。 任何用户都可以在Experience Manager资产中创建自定义静态演绎版，而只有管理员才能创建自定义动态演绎版。 有关详细信息，请参阅[如何应用图像预设或动态演绎版](../using/brand-portal-image-presets.md)。

* **[!UICONTROL 系统呈现版本]**

   允许下载系统生成的资产演绎版。

   这些缩略图是根据“DAM更新资产”工作流在Experience Manager资产中自动生成的缩略图。

* **[!UICONTROL 资源下载]**

   允许将演绎版下载到每个资产的单独文件夹中。 该设置适用于文件夹、收藏集和批量下载资产（超过20个资产）。


以管理员身份登录Brand Portal租户，然后导航到&#x200B;**[!UICONTROL 工具]** > **[!UICONTROL 下载]**。

管理员可以启用Brand Portal用户访问和下载演绎版的任意设置组合。

![](assets/download-settings-new.png)


>[!NOTE]
>
>只有管理员才能下载已过期的资产。 有关已过期资产的更多信息，请参阅[管理资产的数字权限](../using/manage-digital-rights-of-assets.md)。

### 配置用户群组设置 {#configure-user-group-settings}

除了&#x200B;**[!UICONTROL 下载设置]**&#x200B;之外，Brand Portal管理员还可以进一步配置不同用户组的设置，以查看和（或）下载原始资产及其演绎版。

以管理员身份登录Brand Portal租户，然后导航到&#x200B;**[!UICONTROL 工具]** > **[!UICONTROL 用户]**。 在&#x200B;**[!UICONTROL 用户角色]**&#x200B;页面中，导航到&#x200B;**[!UICONTROL 组]**&#x200B;选项卡，以配置用户组的视图和（或）下载设置。

![view-download-permission](assets/download-permissions.png)

>[!NOTE]
>
>如果用户被添加到多个组，并且其中一个组具有限制，则该限制将适用于该用户。

根据配置，独立资产、多个资产、包含资产的文件夹、已授权或未授权的资产，以及使用共享链接下载资产时，下载工作流将保持不变。

下表根据[下载配置](#configure-download)定义用户是否有权访问演绎版：

| **下载设置：自定义演绎版** | **下载设置：系统呈现** | **用户群组设置：下载原始** | **用户群组设置：下载演绎版** | **结果** |
|---|---|---|---|---|
| 开启 | 开启 | 开启 | 开启 | 查看和下载所有演绎版 |
| 开启 | 开启 | 关闭 | 关闭 | 查看原始资产 |
| 关闭 | 关闭 | 开启 | 开启 | 查看和下载原始资产 |
| 开启 | 关闭 | 开启 | 开启 | 查看和下载原始资产和自定义演绎版 |
| 关闭 | 开启 | 开启 | 开启 | 查看和下载原始资产和系统演绎版 |
| 开启 | 关闭 | 关闭 | 关闭 | 查看原始资产 |
| 关闭 | 开启 | 关闭 | 关闭 | 查看原始资产 |
| 关闭 | 关闭 | 关闭 | 开启 | 查看原始资产 |
| 关闭 | 关闭 | 开启 | 关闭 | 查看和下载原始资产 |
| 关闭 | 关闭 | 关闭 | 关闭 | 查看原始资产 |



## 下载资产 {#download-assets}

Brand Portal用户可以从Brand Portal界面下载多个资产、包含资产的文件夹和收藏集。

>[!NOTE]
>
>如果您没有访问或下载资产演绎版的权限，请联系Brand Portal管理员。

如果用户有权访问演绎版，则会向用户提供增强的&#x200B;**[!UICONTROL 下载]**&#x200B;对话框，该对话框具有以下功能：
* 在下载列表中查看任何资产的所有可用演绎版。
* 排除下载不需要的资产演绎版。
* 只需单击一次，即可将相同的演绎版集应用于所有类似的资产类型。
* 为不同的资产类型应用一组不同的演绎版。
* 为每个资产创建一个单独的文件夹。
* 下载选定的资产及其演绎版。

![下载对话框](assets/download-dialog-box.png)

>[!NOTE]
>
>只有在&#x200B;**[!UICONTROL 下载设置]**&#x200B;中启用了&#x200B;**[!UICONTROL 自定义呈现]**&#x200B;和（或）**[!UICONTROL 系统呈现]**&#x200B;时，才会显示&#x200B;**[!UICONTROL 下载]**&#x200B;对话框。


### 下载资产的步骤 {#bulk-download}

以下是从Brand Portal界面下载包含资产的资产或文件夹的步骤：

1. 登录到您的Brand Portal租户。 默认情况下，将打开&#x200B;**[!UICONTROL 文件]**&#x200B;视图，其中包含所有已发布的资产和文件夹。

   执行下列操作之一：

   * 选择要下载的资产或文件夹。 在顶部的工具栏中，单击&#x200B;**[!UICONTROL 下载]**&#x200B;图标。

      ![选择多个资产](assets/select-assets-new.png)

   * 要下载资产的特定资产演绎版，请将指针悬停在资产上，然后单击快速操作缩略图中提供的&#x200B;**[!UICONTROL 下载]**&#x200B;图标。

      ![选择资产](assets/select-asset.png)


      >[!NOTE]
      >
      >如果您是首次下载资产，并且浏览器中未安装IBM Aspera Connect，则系统会提示您安装Aspera下载加速器(`https://www.ibm.com/docs/en/aspera-connect/3.9.9`)。


      >[!NOTE]
      >
      >如果您下载的资产也包括授权资产，则会将您重定向到&#x200B;**[!UICONTROL 版权管理]**&#x200B;页面。 在此页中，选择资产，单击&#x200B;**[!UICONTROL 同意]**，然后单击&#x200B;**[!UICONTROL 下载]**。 如果您选择不同意，则不会下载授权资产。
      > 
      >受许可证保护的资产具有附加的[许可协议](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets)，这可通过在Experience Manager资产中设置资产的[元数据属性](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets)来完成。


      ![许可资产](assets/licensed-asset-new.png)

1. 将打开列出所有选定资产的&#x200B;**[!UICONTROL 下载]**&#x200B;对话框。

   单击任何资产可查看可用的演绎版，并选中与您要下载的演绎版对应的复选框。

   您可以手动选择或排除单个资产的演绎版，或单击&#x200B;**应用**&#x200B;图标，以选择要为类似资产类型（本示例中的所有图像文件）下载的相同演绎版集。 在&#x200B;**[!UICONTROL 应用全部]**&#x200B;对话框中，单击&#x200B;**[!UICONTROL 完成]**&#x200B;以将规则应用于所有类似资产。

   ![全部应用](assets/apply.png)

   您还可以通过单击&#x200B;**删除**&#x200B;图标，从下载列表中删除资产（如果需要）。

   ![删除](assets/remove.png)

   要在下载资产时保留Brand Portal文件夹层次结构，请选中&#x200B;**[!UICONTROL 为每个资产创建单独的文件夹]**&#x200B;复选框。

   “下载”按钮反映选定项目的计数。 完成应用规则后，单击&#x200B;**[!UICONTROL 下载项目]**。

   ![下载对话框](assets/download-dialog-box-new.png)

1. 默认情况下，在&#x200B;**[!UICONTROL 下载设置]**&#x200B;中启用了&#x200B;**[!UICONTROL 快速下载]**&#x200B;设置。 因此，似乎有一个确认框允许使用IBM Aspera Connect加速下载。

   要继续使用&#x200B;**[!UICONTROL Fast Download]**，请单击&#x200B;**[!UICONTROL Allow]**。 所有选定的演绎版均使用IBM Aspera Connect下载到zip文件夹中。

   如果不想使用IBM Aspera Connect，请单击&#x200B;**[!UICONTROL 拒绝]**。 如果拒绝或失败&#x200B;**[!UICONTROL Fast Download]**，则系统会填充一条错误消息。 单击&#x200B;**[!UICONTROL Normal Download]**&#x200B;按钮以继续下载资产。

>[!NOTE]
>
>如果管理员关闭了&#x200B;**[!UICONTROL Fast Download]**&#x200B;设置，则所选演绎版将直接下载到zip文件夹中，而无需使用IBM Aspera Connect。

>[!NOTE]
>
>如果在&#x200B;**[!UICONTROL 下载设置]**&#x200B;中启用了&#x200B;**[!UICONTROL 资产下载]**&#x200B;设置，则会在zip文件夹中每个资产的单独文件夹中下载资产演绎版。
>  
>如果从共享链接下载资产，则会在zip文件夹中每个资产的单独文件夹中下载资产演绎版。
>
>如果选择了文件夹、收藏集或20个以上的资产进行下载，则会跳过&#x200B;**[!UICONTROL 下载]**&#x200B;对话框，用户可访问的所有资产演绎版（不包括动态演绎版）都将下载到zip文件夹中。

>[!NOTE]
>
>Brand Portal支持在混合模式和Scene 7模式下配置Dynamic Media。
>
>(*如果Experience Manager资产创作实例在&#x200B;**Dynamic Media混合模式***上运行)
>
>要预览或下载资产的动态演绎版，请确保已启用Dynamic Media，并且资产的Pyramid tiff演绎版存在于Experience Manager资产创作实例中，资产的创作实例已从中发布。 将资产从Experience Manager资产发布到Brand Portal时，也会发布其金字塔TIFF演绎版。



如果管理员未授权您[访问原始演绎版](../using/brand-portal-adding-users.md#main-pars-procedure-202029708)，则不会下载选定资产的原始演绎版。

![无访问消息](assets/no-access-message.png)

<!-- This issue has been resolved, check with engineering.
>[!NOTE]
>
>Once you have downloaded the asset renditions, the **[!UICONTROL Download]** button is disabled to avoid creating duplicate copies of the renditions. To download more (missing or another copy of renditions), refresh the browser to re-enable the download button.
-->

### 从资产详细信息页面下载资产 {#download-assets-from-asset-details-page}

除了下载工作流之外，还有一种方法可以直接从资产详细信息页面下载各个资产的演绎版。

用户可以预览不同的演绎版，选择特定的演绎版，并直接从资产详细信息页面的&#x200B;**[!UICONTROL 演绎版]**&#x200B;面板中下载它们，而无需打开&#x200B;**[!UICONTROL 下载]**&#x200B;对话框。


以下是从资产详细信息页面下载资产演绎版的步骤：

1. 登录到您的Brand Portal租户，然后单击资产以打开资产详细信息页面。
1. 单击左侧的叠加图标，然后单击&#x200B;**[!UICONTROL 演绎版]**。

   ![演绎版导航](assets/rendition-navigation.png)

1. **[!UICONTROL 演绎版]**&#x200B;面板会根据资产[下载配置](#configure-download)列出所有可访问的资产演绎版。

   选择要下载的特定演绎版，然后单击&#x200B;**[!UICONTROL 下载项目]**。

   ![renditions面板](assets/renditions-panel.png)

1. 默认情况下，在&#x200B;**[!UICONTROL 下载设置]**&#x200B;中启用了&#x200B;**[!UICONTROL 快速下载]**&#x200B;设置。 因此，似乎有一个确认框允许使用IBM Aspera Connect加速下载。

   要继续使用&#x200B;**[!UICONTROL Fast Download]**，请单击&#x200B;**[!UICONTROL Allow]**。 所有选定的演绎版均使用IBM Aspera Connect下载到zip文件夹中。

   如果使用&#x200B;**[!UICONTROL Fast Download]**&#x200B;拒绝，则系统会填充一条错误消息。 单击&#x200B;**[!UICONTROL Normal Download]**&#x200B;按钮以继续下载资产。

>[!NOTE]
>
>如果管理员关闭了&#x200B;**[!UICONTROL Fast Download]**&#x200B;设置，则所选演绎版将直接下载到zip文件夹中，而无需使用IBM Aspera Connect。


>[!NOTE]
>
>单独下载的资产会显示在资产下载报表中。 但是，如果下载的文件夹中包含资产，则文件夹和资产不会显示在资产下载报表中。

<!--
>[!NOTE]
>
>Assets that are individually downloaded are visible in the assets download report. However, if a folder containing assets is downloaded, the folder and assets are not displayed in the assets download report.
-->

<!-- Backup of content before updating the new feature docs.
## Configure asset download {#configure-download}

The download configuration allows the Brand Portal administrators to define the set of renditions available to the Brand Portal users for downloading the assets. The administrator can configure the asset **[!UICONTROL Download]** settings from the Brand Portal interface. 

The available configurations are:

* **[!UICONTROL Fast Download]** 

  Enables high-speed download of the assets. To know more, see [guide to accelerate downloads from Brand Portal](../using/accelerated-download.md).

* **[!UICONTROL Custom Renditions]** 
  
  Download custom and (or) dynamic renditions of the assets. 
  All the asset renditions other than the original asset and system-generated renditions are called as custom renditions. It includes static as well as dynamic renditions available for the asset. Any user can create a custom static rendition in AEM Assets, whereas, only the AEM administrator can create custom dynamic renditions. To know more, see [how to apply image presets or dynamic renditions](../using/brand-portal-image-presets.md)

* **[!UICONTROL System Renditions]** 

  Download system-generated renditions of the assets. These are the thumbnails which are automatically generated in AEM Assets based on the "DAM update asset" workflow. 

Log in to your Brand Portal tenant as an administrator and navigate to **[!UICONTROL Tools]** > **[!UICONTROL Download]**. By default, the **[!UICONTROL Fast Download]** configuration is enabled in the **[!UICONTROL Download Settings]**. 

The administrators can enable any combination to configure the asset download process.

![](assets/download-configuration.png)


Based on the configuration, the download workflow remains constant for stand-alone assets, multiple assets, folders containing assets, licensed or unlicensed assets, and downloading assets using share link. 


* If both **[!UICONTROL Custom Renditions]** and **[!UICONTROL System Renditions]** configurations are turned-off, the original renditions of the assets are downloaded without any additional dialog being presented to the users.    


* If any of the **[!UICONTROL Custom Renditions]** or **[!UICONTROL System Renditions]** configuration is enabled, an additional **[!UICONTROL Download]** dialog box appears wherein you can choose whether to download the original asset along with its renditions, or download only specific renditions. 

>[!NOTE]
>
>Only the administrators can download the expired assets. For more information about expired assets, see [manage digital rights of assets](../using/manage-digital-rights-of-assets.md).

## Steps to download assets {#steps-to-download-assets}

Following are the steps to download assets or folders containing assets from Brand Portal:

1. From the Brand Portal interface, do one of the following:

   * Select the folders or assets you want to download. From the toolbar at the top, click the **[!UICONTROL Download]** icon.

     ![](assets/downloadassets-1.png)

   * To download a specific asset or folder, hover the pointer over the asset or folder and click the **[!UICONTROL Download]** icon available in the quick action thumbnails.

     ![](assets/downloadsingleasset-1.png)


     >[!NOTE]
     >
     >If you are downloading the assets for the first time and do not have IBM Aspera Connect installed in your browser, it will prompt you to install the Aspera download accelerator. 


     >[!NOTE]
     >
     >If the assets you are downloading also include licensed assets, you are redirected to the **[!UICONTROL Copyright Management]** page. In this page, select the assets, click **[!UICONTROL Agree]**, and then click **[!UICONTROL Download]**. If you choose to disagree, licensed assets are not downloaded. 
     > 
     >License-protected assets have [license agreement attached](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) to them, which is done by setting asset's [metadata property](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) in Experience Manager Assets.


     ![](assets/licensed-asset-download-1.png)

     
     >[!NOTE]
     >
     >Ensure to select all the required asset renditions while downloading them from the asset details page, and click **[!UICONTROL Download]**. The selected renditions are downloaded to your local machine.
     > 
     >Once you download, the **[!UICONTROL Download]** button is disabled to avoid creating duplicate copies of the downloaded renditions. To download more (missing or another copy of renditions), refresh the browser to re-enable the download button.

     If any of the **[!UICONTROL Custom Renditions]** or **[!UICONTROL System Renditions]** configuration is enabled in the **[!UICONTROL Download Settings]**, the **[!UICONTROL Download]** dialog appears with the **[!UICONTROL Asset(s)]** check box selected by default. If the **[!UICONTROL Fast Download]** configuration is enabled, the **[!UICONTROL Enable download acceleration]** check box is selected by default.

     ![](assets/download-dialog.png)

     >[!NOTE]
     >
     >If the downloading assets are image files, and you select only the **[!UICONTROL Asset(s)]** check box in the **[!UICONTROL Download]** dialog but are not [authorized by the administrator to have access to the original renditions of image files](../using/brand-portal-adding-users.md#main-pars-procedure-202029708) then no image files are downloaded and a notification appears, stating that you have been restricted by the administrator to access original renditions.

     ![](assets/restrictaccess-note.png)

1. To download the renditions in addition to the original assets, select the **[!UICONTROL Rendition(s)]** check box. However, if you want to download the system-generated renditions along with the custom renditions, clear the **[!UICONTROL Exclude System Renditions]** check box.

   ![](assets/download-system-rendition.png)

   * To download only the renditions, clear the **[!UICONTROL Asset(s)]** check box.

     >[!NOTE]
     >
     >By default, only the assets are downloaded. However, original renditions of image files are not downloaded if you are not [authorized by the administrator to have access to the original renditions of image files](../using/brand-portal-adding-users.md#main-pars-procedure-202029708).

    * To share the selected assets with other users through a link, select the **[!UICONTROL Email]** check box. An email notification is sent to the users with the download link. To know how to download assets from shared links, see [downloading assets from shared links](../using/brand-portal-link-share.md#main-pars-header-1703469193).  

      ![](assets/download-link.png)

      >[!NOTE]
      >
      >The download link on email notification expires after 45 days.
      >
      >The administrators can customize email messages, that is, logo, description, and footer, using the [Branding](../using/brand-portal-branding.md) feature.


    * You can select a predefined image preset or create a custom dynamic rendition from the **[!UICONTROL Download]** dialog box. 

      To apply a [custom image preset to the asset and its renditions](../using/brand-portal-image-presets.md#applyimagepresetswhendownloadingimages), select the **[!UICONTROL Dynamic Rendition(s)]** check box. Specify the image preset properties (such as size, format, color space, resolution, and image modifier) to apply the custom image preset while downloading the asset and its renditions. To download only the dynamic renditions, clear the **[!UICONTROL Asset(s)]** check box.

      ![](assets/dynamic-rendition.png)

      >[!NOTE]
      >
      >Brand Portal supports configuring Dynamic Media in both - Hybird and Scene 7 mode. 
      >
      >(*If AEM author instance is running on **Dynamic Media Hybrid mode***)
      >
      >To preview or download dynamic renditions of an asset, ensure that the dynamic media is enabled and the asset's Pyramid tiff rendition exists at the AEM Assets author instance from where the assets have been published. When an asset is published to Brand Portal, its Pyramid tiff rendition is also published.
      
  
    * To preserve the Brand Portal folder hierarchy while downloading assets, select the **[!UICONTROL Create separate folder for each asset]** check box. By default, the Brand Portal folder hierarchy is ignored and all the assets are downloaded in one folder in your local system.

1. Click **[!UICONTROL Download]**.

   The assets (and renditions if selected) are downloaded as a zip file to your local folder. However, no zip file is created if a single asset is downloaded without any of the renditions. 

   If you are not [authorized by the administrator to have access to the original renditions](../using/brand-portal-adding-users.md#main-pars-procedure-202029708), the original renditions of the selected assets are not downloaded. 

   >[!NOTE]
   >
   >Assets that are individually downloaded are visible in the assets download report. However, if a folder containing assets is downloaded, the folder and assets are not displayed in the assets download report.
-->

## 预期下载性能 {#expected-download-performance}

不同客户端位置的用户的文件下载体验可能会有所不同，具体取决于本地Internet连接和服务器延迟等因素。 在不同客户端位置观察到的2-GB文件的预期下载性能如下所示，其中Brand Portal服务器位于美国俄勒冈州：

| 客户端位置 | 客户端和服务器之间的延迟 | 预期下载速度 | 下载2 GB文件所花费的时间 |
|-------------------------|-----------------------------------|-------------------------|------------------------------------|
| 美国西部（北加利福利亚） | 18毫秒 | 7.68 MB/秒 | 4分钟 |
| 美国西部（俄勒冈） | 42毫秒 | 3.84 MB/秒 | 9分钟 |
| 美国东部（弗吉尼亚北） | 85毫秒 | 1.61 MB/秒 | 21分钟 |
| APAC（东京） | 124毫秒 | 1.13 MB/秒 | 30 分钟 |
| 诺伊达 | 275毫秒 | 0.5 MB/秒 | 68分钟 |
| 悉尼 | 175毫秒 | 0.49 MB/秒 | 69分钟 |
| 伦敦 | 179毫秒 | 0.32 MB/秒 | 106分钟 |
| 新加坡 | 196毫秒 | 0.5 MB/秒 | 68分钟 |


>[!NOTE]
>
>在测试条件下观察引用的数据，不同位置的用户可能看到不同的延迟和带宽。
