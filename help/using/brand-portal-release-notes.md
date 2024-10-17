---
title: 发行说明
description: 深入了解Adobe Experience Manager Assets Brand Portal 2024.10.0版本中的功能、增强功能、修复的关键问题和已知问题。
content-type: reference
contentOwner: Kirandeep Kour
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
exl-id: e4e89080-9863-4857-8f3a-fcd516ef3271
source-git-commit: 3f3065de994f5c38e604b52848b0a538c9efd7d1
workflow-type: tm+mt
source-wordcount: '1533'
ht-degree: 4%

---

# 发行说明 {#release-notes}

深入了解Adobe Experience Manager Assets Brand Portal 2024.10.0版本中的新增功能、增强功能、修复的关键问题和已知问题。

## 版本信息 {#release-information}

| 产品 | Adobe Experience Manager Assets Brand Portal |
|---|---|
| 版本 | 2024.10.0 |
| 日期 | 2024年10 |

## 概述 {#overview}

Adobe Experience Manager (AEM) Assets Brand Portal可帮助您轻松地获取、控制经过批准的创意资产，并将这些资产安全地分发给跨设备的外部参与方和内部业务用户。 它有助于提高资产共享效率，加快资产上市速度，并降低不合规和未经授权访问的风险。 Brand Portal允许用户随时随地以公司批准的格式浏览、搜索、预览、下载和导出资源。

## 2024.10.0的新增功能{#whats-new-in-2024.10.0}

### 已修复的关键问题 {#critical-issues-fixed}

#### 错误修复 {#bug-fixes}

此版本包含以下错误修复：

* 未发送采购导入事件的电子邮件通知。
* 使用搜索筛选器时，[!DNL Brand Portal]在搜索筛选器窗口中显示重复的文件夹。
* 无法下载包含名称中包含特殊字符的非许可资产的收藏集。
* 导航到[!UICONTROL 搜索表单编辑器]时，标签未本地化。
* 标签在链接共享窗口中未本地化。
* 无法下载名称中包含特殊字符的视频。
* 将资产从[!DNL Adobe Experience Manager Assets]发布到Brand Portal并将其取消发布无法正常运行。
* 无法播放从Brand Portal下载的视频。

## 以前的版本

### 2024 年 2 月版本 {#feb-2024}

**错误修复和增强功能**

此版本包含以下错误修复：

* 无法在土耳其语言环境中下载受DRM保护的数字资产。
* 无法打开和下载现有报表，这些报表包含具有多行标题的资产。
* 使用操作栏中的[!UICONTROL 下载]按钮下载资源时，最多可下载1000个资源。
* 在PSD树中查看时，内容类型资源的名称不正确。
* 资源详细信息页面上的[!UICONTROL 删除演绎版]选项不起作用。
* 下载弹出窗口中资源的标题和大小未对齐。
* 创建报告时，标签未本地化。
* 在Brand Portal中，支持管理员称为管理员。

### 2023 年 10 月版本 {#oct-2023}

**错误修复和增强功能**
此版本包括以下增强功能：

* 浏览[!UICONTROL 收藏集]时的性能改进。

* 改进了使用OmniSearch字段执行部分搜索时的搜索结果。

此版本包含以下错误修复：

* 无法将[!UICONTROL Date]和[!UICONTROL Options]谓词保存到[!UICONTROL 智能收藏集]。

* 使用英语以外的区域设置时，[!UICONTROL 日期和时间]格式不一致。

* 执行搜索资产时，缺少[!UICONTROL 删除]按钮。

* 如果[!UICONTROL 标题]字段在[!UICONTROL 链接共享]中包含多字节符号，则无法下载报告。

* 查看PDF类型文档时，标签和工具提示未本地化。

### 2023 年 8 月版本 {#aug-2023}

**错误修复和增强功能**
此版本包括以下增强功能：

* 在[!UICONTROL 下载]弹出窗口中加载资产时的性能改进。
* 现在，当您下载资源或资源的演绎版时，将以其原始文件类型格式而不是zip文件格式下载。

此版本包含以下错误修复：

* 长标签或标记无法正确显示在搜索筛选器中。
* 无法在“下载”对话框中显示长格式副本名称。
* 无法在卡片视图中预览视频资产。

### 2023 年 5 月版本 {#may-2023}

**错误修复**
此版本包括对以下关键问题的修复：

* 如果从共享链接下载资产时出错，则错误提示的`Notice`和`Close`标签未本地化。
* 使用`Filter`窗格访问搜索筛选器时，Brand Portal显示&#x200B;**请求标头字段太大**&#x200B;错误。

**已知问题**
此版本包括以下已知问题：

* 资产源报表内容中的部分本地化。
* 用户配置文件的某些字段在用户配置文件上不可编辑。

### 2023 年 2 月版本 {#feb-2023}

**错误修复**

此版本包括对以下关键问题的修复：

* 无法在Brand Portal上更新配置文件图片。
* 内容树窗格无法调整大小。 如果文件名长于内容树的缺省宽度，则无法水平和垂直拖动内容树。 因此，较长的文件名是不可读的。
* 在搜索表单中使用两次的同一属性谓词的搜索结果不一致。
* 并非所有语言都本地化了中间登录页面上的文本。

**增强功能**

此版本包括以下增强功能：

* 现在提供了新的现代PDF查看器，以改进PDF资源的预览。
* 您现在可以选择为管理员启用或禁用资产源通知。 导航到[!UICONTROL 常规设置]，然后启用或禁用[!UICONTROL `Notify Administrator of asset contribution`]。

  ![通知管理员资源贡献](assets/notify-admin.png)

* 如果禁用了请求访问权限，则未授权用户无法请求访问Brand Portal。
* 只有为Brand Portal配置的组织才会显示在配置文件选取器列表中。

**已知问题**

此版本包括以下已知问题：

* 资产源报表内容中的部分本地化。
* 用户配置文件的某些字段在用户配置文件上不可编辑。

### 2022 年 10 月版本 {#oct-2022}

**已修复严重问题**

此版本包括对以下关键问题的修复：

* 将大型文件从Brand Portal复制到第三方工具时，响应缓慢。
* 选中呈现版本计数复选框时，用于选择单个呈现版本的复选框将被禁用。
* 搜索响应缓慢。

>[!IMPORTANT]
>
>AEM Assets Brand Portal中的Pulse通知将从2022年12月1日起停止。 您继续收到以下事件的电子邮件通知，而不是Pulse通知：
>
>* 通过链接共享资源
>* 请求访问工作流
>* 共享贡献文件夹
>* 启动导出到AEM的过程
>* 已完成导出到AEM
>

### 2022 年 8 月版本 {#aug-2022}

**已修复严重问题**

此版本包括对以下关键问题的修复：

* 当NUI无法在Experience Manager中处理资源时，Brand Portal显示不准确的资源导入状态。
* 当预览操作失败时，没有通知可传达该失败。
* 修复了每个资源的`totalUploadedSize`属性不准确的值。
* 当您单击&#x200B;**下载所有项目**&#x200B;并且某个资源具有大量可用呈现时，Brand Portal将下载无效的.ZIP文件。
* 某些字符串的翻译在Brand Portal用户界面中被截断。

### 2022 年 5 月版本 {#may-2022}

**新功能**

Brand Portal现在每十二小时执行一次自动作业，以删除发布到AEM的所有Brand Portal资源。 因此，您无需手动删除“贡献”文件夹中的资产，即可将文件夹大小保持在阈值限制以下。

**已修复严重问题**

此版本包括对以下关键问题的修复：

* 下载包含带有颜色标记的资产的文件夹或收藏集时，也会下载XML文件。
* 下载包含演绎版的视频时，Brand Portal会创建一个无效的.ZIP文件。
* 在AEM创作实例中创建预设和资源，然后将其发布到Brand Portal时，您可以在下载资源的同时选择动态演绎版。 但是，您无法解压缩下载的.ZIP文件。 此问题会阻止访问下载的内容。
* 从Brand Portal上提供的某些文件夹下载视频资源时出现问题。
* 当您使用电子邮件共享Contribution文件夹的URL时，查看者和编辑者角色在使用痕迹导航访问其父文件夹时面临问题。
* 来源补充发布报表显示的作业开始时间不正确。

### 2022 年 2 月版本 {#feb-2022}

**新功能**

* 来宾用户的会话超时阈值已从2小时减少到15分钟。
* 已为多页面PDF删除其他&#x200B;**[!UICONTROL 查看页面]**&#x200B;选项，因为用户现在可以从Adobe Document Cloud查看器查看PDF页面。
* 用户无法搜索、导航或打开文件夹。 用户界面反映错误消息： `Failed to load data`。
* **[!UICONTROL 呈现版本]**&#x200B;面板未列出发布到Brand Portal的所有资源的静态呈现版本。
* **[!UICONTROL 演绎版]**&#x200B;面板列出了资源的智能裁剪演绎版，但是，用户无法预览或下载智能裁剪演绎版。
* 下载对话框列出了所选资源的智能裁剪演绎版，但是，用户无法下载智能裁剪演绎版。
* 非管理员用户在下载资源时仅获得原始资源演绎版。 未下载系统和自定义呈现版本。
* 应用搜索筛选器下载资产时，`Download`按钮在下载对话框中处于禁用状态，不允许用户下载资产。
* 如果启用了`Smart Tags`和（或）`Color Tags`，下载对话框会将`json`文件列为演绎版，并将这些`json`文件下载到存档的zip文件夹中。
* 匿名用户无法使用共享链接下载资源，因为该链接将重定向到Brand Portal登录页面。
* 系统未反映活动并发用户数的正确值。

<!--
### New Features {#new-features}

This release includes the following new features:

* AEM Assets as a Cloud Service is now entitled to have a pre-configured Brand Portal instance. The Cloud Manager user can activate Brand Portal on the AEM Assets as a Cloud Service instance.

* Asset Sourcing feature is now available on AEM Assets as a Cloud Service. It allows the Brand Portal users to upload assets to the permitted contribution folders and publish the contribution folder from Brand Portal to AEM Assets as a Cloud Service instance. 

* An additional **[!UICONTROL Asset Download]** setting has been introduced under the **[!UICONTROL Download Settings]**. It creates a separate folder for each asset while downloading the folders, collections, or bulk download of assets. 
-->
<!-- 
* The **[!UICONTROL Download]** dialog is revamped in a list view with additional options to exclude the renditions which are not required, apply the same set of rules for similar asset types, and download the selected asset renditions.
-->

<!--
* The new **[!UICONTROL Download]** dialog now appears with all the renditions of the selected assets or folders containing assets in a list view, wherein the Brand Portal users can apply same set of renditions for similar asset types and download the selected asset renditions. 
-->

<!-- 
* Navigation to the **[!UICONTROL Files]**, **[!UICONTROL Collections]**, and **[!UICONTROL Shared Links]** is now possible from all the Brand Portal pages in one-click.  

* The **[!UICONTROL Renditions]** panel in the asset details page now allows the Brand Portal users to select the original asset and (or) specific asset renditions, and directly download them from the **[!UICONTROL Renditions]** panel without having to open the **[!UICONTROL Download]** dialog.
-->

<!--
Brand Portal users can exclude specific renditions which are not required and directly download the original asset and its renditions from the **[!UICONTROL Renditions]** panel on the asset details page. 
-->

<!-- 
* In addition to the existing **[!UICONTROL Download]** configurations, the Brand Portal administrators can also [configure permissions for different group of users]() to view and (or) download the original asset and its renditions from the asset details page. These configurations will define who can access and (or) download the asset renditions.
-->

<!--
### Enhancements {#enhancements}

Brand Portal 2021.08.0 is an internal release that introduces Business profiles for enterprise and teams customers to give organizations better control over their assets. 

This release includes the following enhancements:

* The users now have organization-specific entitlement on the new and migrated organizations. If a user is entitled to multiple organizations, the user has to select the organization at the time of login.

* The new users that are added in Admin Console must **Join Team** to get entitled to the organization. 

>[!NOTE]
>
>Business profiles are currently applicable for the new organizations that are created after August 16, 2021. 
>
>Until your organization is migrated, you can continue to use Adobe ID, Enterprise ID, or Federated ID types to access the organization.   
-->

<!-- 
* For folder download, a separate folder is created for each asset using share link irrespective of the **[!UICONTROL Download Settings]**. 
* The Brand Portal **[!UICONTROL Usage Report]** has been modified to reflect only the active Brand Portal users.
-->

<!--
* The threshold of session timeout for the guest users has been reduced from 2 hours to 15 minutes.
* The additional **[!UICONTROL View pages]** option has been removed for multi-page PDFs as the user can now view the PDF pages from the Adobe Document Cloud Viewer.

* The users are unable to search, navigate, or open folders. The user interface reflects the error message: `Failed to load data`. 
* The **[!UICONTROL Renditions]** panel does not list all the static renditions of the assets that are published to Brand Portal.
* The **[!UICONTROL Renditions]** panel lists the smart crop renditions of the asset, however, the user cannot preview or download the smart crop renditions.
* The download dialog lists the smart crop renditions of the selected asset, however, the user cannot download the smart crop renditions. 
* A non-admin user is getting only the original asset rendition when downloading an asset. The system and custom renditions are not downloaded.  
* When applying search filter to download an asset, the `Download` button is disabled in the download dialog and does not allows the user to download the asset.
* If `Smart Tags` and (or) `Color Tags` are enabled, the download dialog lists the `json` files as renditions and downloads these `json` files in the archived zip folder.
* The anonymous users are unable to download assets using a shared link because the link redirects to the Brand Portal login page. 
* The system is not reflecting the correct value for the number of active concurrent users.
-->

<!--
### New features {#new-features}

Brand Portal now executes automatic jobs every twelve hours to delete all Brand Portal assets that are published to AEM. As a result, you do not need to delete the assets in the Contribution folder manually to keep the folder size below the threshold limit. See [What's new in Experience Manager Assets Brand Portal](whats-new.md).
-->

<!--
This release includes fixes to the following critical issues:

* When you download a folder or a collection that includes assets with color tags, an XML file gets downloaded as well.

* When you download a video that includes renditions, Brand Portal creates an invalid .ZIP file.

* When you create presets and assets on AEM author and publish them to Brand Portal and then select dynamic renditions while downloading the assets, you cannot extract the downloaded .ZIP file.

* Issues while downloading video assets from certain folders available on Brand Portal.

* When you share the Contribution folder's URL using an email, Viewer and Editor roles face issues while accessing its parent folder using the breadcrumb.

* Sourcing published report displays an incorrect job start time.
>
 
<!--
* Asset Sourcing email notifications are not delivered for some organizations. 

* Video files with extension `.mov` are not running on Brand Portal. 

* In the **[!UICONTROL Smart Collections]** dropdown list, only ten saved collections are visible. 
-->
<!--
* *_deleted tenants are listed as valid tenant which fails during the execution of TenantCustomizers/TenantUpdates where tenant id is returned as /etc/tenants/`<nodename>`.
-->

<!--
In case only the original assets are downloaded, the asset reflects its own extension and does not open until the extension is manually changed to zip. 
* The user interface of the collection folder does not respond on clicking the navigation arrow. 
* **[!UICONTROL Create]** button is visible in the **[!UICONTROL Column]** view even when the folders are empty.
* **[!UICONTROL Omni search]** fails with a 414 error message (Request-URI Too Long) if the dispatcher is bypassed while accessing the Brand Portal instance.
* An empty zip folder is downloaded if the asset contains a comma (`,`) in the file name.
* The viewer users get the option to add users to the collection they have created. 
* Inconsistent behavior is experienced when an asset (thumbnail or web rendition) is downloaded using share link.

See [what's new in Brand Portal 2021.02.0](whats-new.md).
-->

<!--
### Known Issues {#known-issues}

This release includes the following known issue:

* Search on the **[!UICONTROL Asset Reports]** shows processing on the product interface with no search result.
* The video DM encodes are not visible to the non-admin users on the asset details page.
* The alignment of the size of individual asset renditions and total download size is distorted in the Download dialog.
-->


<!--
* Download Settings configuration to configure asset download from Brand Portal. Fast download, custom renditions, and system renditions are the available configurations. 
-->

<!--
* Document Viewer has been introduced to enhance the PDF viewing experience. New options are available for viewing the PDF files in Brand Portal.

* Advances in the asset download process which improves the Brand Portal user experience while [downloading assets from Brand Portal](brand-portal-download-assets.md). Brand Portal administrators can configure **[!UICONTROL Fast Download]**, **[!UICONTROL Custom Renditions]**, and **[!UICONTROL System Renditions]** from the **[!UICONTROL Download]** settings. 

For details, see [what's new in Brand Portal 6.4.7](whats-new.md). 

### Critical Issues Fixed {#critical-issues-fixed-647}

This release includes fixes to the following critical issues:

* The viewer users are not permitted to share link for collections but the option to share is visible to them on the product interface.

* The **[!UICONTROL Download]** button on the options bar does not list all the licensed assets of the selected folder.

* The search takes longer to show the results for certain keywords.

* The **[!UICONTROL Agree]** and **[!UICONTROL Disagree]** check boxes does not appear on bulk selection of licensed and unlicensed assets during download.

* Filter-based search shows processing on the product interface with no search result. 

* The assets do not download from share link if the shared folder contains numerous and large assets.


### Known Issues {#known-issues-647}

This release includes the following known issues:

* If multiple assets are selected, license text does not appear on clicking Terms and Conditions on the license agreement page during download using share link.   

-->

## 语言 {#languages}

提供了以下语言版本的Brand Portal用户界面：

* 英语
* 德语
* 法语
* 西班牙语
* 意大利语
* 巴西葡萄牙语
* 日语
* 简体中文
* 朝鲜语

## 认证平台 {#certified-platforms}

要查看哪些平台已针对此Brand Portal版本进行认证，请查看[技术要求](https://experienceleague.adobe.com/zh-hans/docs/experience-manager-65/content/implementing/deploying/introduction/technical-requirements)的&#x200B;**用于创作用户界面的受支持的浏览器**&#x200B;部分中的&#x200B;**对触控优化UI的支持**&#x200B;列。

## 链接 {#links}

* adobe.com上的[Adobe Experience Manager产品页](https://business.adobe.com/in/products/experience-manager/adobe-experience-manager.html)
* [Assets Brand Portal文档](https://experienceleague.adobe.com/en/docs/experience-manager-brand-portal/using/home)

## 产品访问和支持（受限制的站点） {#product-access-and-support-restricted-sites}

这些网站仅供客户使用。 如果您是客户并且需要访问权限，请联系您的Adobe客户经理。

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

<!--
* [Customer Support]()
-->
