---
title: 发行说明
seo-title: Release Notes
description: 深入了解Adobe Experience Manager Assets Brand Portal 2023.02.0版本中的功能、增强功能、已修复的关键问题和已知问题。
seo-description: Get an insight into the enhancements, critical issues fixed, and known issues in the Adobe Experience Manager Assets Brand Portal 2023.02.0 release.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Kirandeep Kour
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
exl-id: e4e89080-9863-4857-8f3a-fcd516ef3271
source-git-commit: d5284a2ad62be2a72d168358d86b473257856592
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 7%

---

# 发行说明 {#release-notes}

深入了解Adobe Experience Manager Assets Brand Portal 2023.02.0版本中的新增功能、增强功能、已修复的关键问题和已知问题。

## 版本信息 {#release-information}

| 产品 | Adobe Experience Manager Assets Brand Portal |
|---|---|
| 版本 | 2023.02.0 |
| 日期 | 2023 年 2 月 日 |

## 概述 {#overview}

Adobe Experience Manager(AEM)Assets Brand Portal可帮助您跨设备轻松获取、控制和安全地将已批准的创意资产分发给外部各方和内部业务用户。 它有助于提高资产共享的效率，加快资产的上市时间，并降低不合规和未经授权访问的风险。 Brand Portal允许用户随时随地以公司批准的格式浏览、搜索、预览、下载和导出资产。

## 2023.02.0的新增功能 {#whats-new-in-2023.02.0}

### 已修复的关键问题 {#critical-issues-fixed}

#### 错误修复 {#bug-fixes}

此版本包括对以下关键问题的修复：
* 无法在Brand Portal上更新用户档案图片。
* 内容树窗格不可调整大小。 如果文件名比内容树的默认宽度长，则不能同时水平和垂直拖动内容树。 因此，较长的文件名不可读。
* 搜索表单中使用两次的同一属性谓词的搜索结果不一致。
* 中间登录页面上的文本并非针对所有语言进行本地化。

### 增强功能 {#enhancements}

此版本包括以下增强功能：
* 现在提供了新的现代PDF查看器，以改进PDF资产的预览。
* 您现在可以选择为管理员启用或禁用资产源通知。 导航到 [!UICONTROL 常规设置] 然后启用或禁用 [!UICONTROL `Notify Administrator of asset contribution`].

   ![通知管理员进行资产贡献](assets/notify-admin.png)

* 如果请求访问被禁用，则未授权用户无法请求访问Brand Portal。
* 仅为Brand Portal配置的组织显示在配置文件选取器列表中。

### 已知问题 {#known-issues}

此版本包括以下已知问题：

* 资产源报表内容中的局部本地化。
* 用户配置文件的少数字段在用户配置文件中不可编辑。

## 以前版本

### 2022年10月版 {#oct-2022}

**已修复的关键问题**

此版本包括对以下关键问题的修复：
* 将大文件从Brand Portal复制到第三方工具时响应速度缓慢。
* 选中演绎版计数复选框时，用于选择各个演绎版的复选框将处于禁用状态。
* 搜索响应速度缓慢。

>[!IMPORTANT]
>
>AEM Assets Brand Portal的脉冲通知将从2022年12月1日起停用。 您将继续接收以下事件的电子邮件通知，而不是Pulse通知：
>* 通过链接共享资产
>* 请求访问工作流
>* 共享贡献文件夹
>* 开始导出到AEM
>* 已完成导出到AEM
>


### 2022年8月版 {#aug-2022}

**已修复的关键问题**

此版本包括对以下关键问题的修复：
* 当NUI无法在Experience Manager中处理资产时，Brand Portal会显示不准确的资产导入状态。
* 预览操作失败时，不会显示通知来告知失败。
* 修复了每个资产的totalUploadedSize属性值不准确的问题。
* 单击 **下载所有项目** 并且资产有大量的演绎版可用，因此Brand Portal会下载无效的.ZIP文件。
* 某些字符串的翻译在Brand Portal用户界面中会被截断。

### 2022年5月版 {#may-2022}

**新增功能**

 Brand Portal 现在，每十二小时执行一次自动作业，以删除发布到 AEM 的所有 Brand Portal 资产。 因此，您无需手动删除“贡献”文件夹中的资产，即可将文件夹大小保持在阈值限制以下。 

**已修复的关键问题**

此版本包括对以下关键问题的修复：

* 下载包含带有颜色标记的资产的文件夹或收藏集时，也会下载XML文件。
* 下载包含演绎版的视频时，Brand Portal会创建一个无效的.ZIP文件。
* 在AEM作者上创建预设和资产，并将它们发布到Brand Portal，然后在下载资产时选择动态演绎版，此时您将无法提取下载的.ZIP文件。
* 从Brand Portal上可用的某些文件夹下载视频资产时出现问题。
* 使用电子邮件共享Contribution文件夹的URL时，查看器和编辑器角色在使用痕迹导航访问其父文件夹时遇到问题。
* 来源补充发布报表显示错误的作业开始时间。

### 2022年2月版 {#feb-2022}

**新增功能**

* 来宾用户的会话超时阈值已从2小时减少到15分钟。
* 其他 **[!UICONTROL 查看页面]** 多页面PDF的选项已被删除，因为用户现在可以从Adobe Document Cloud查看器中查看PDF页面。
* 用户无法搜索、导航或打开文件夹。 用户界面反映错误消息： `Failed to load data`.
* 的 **[!UICONTROL 演绎版]** 面板中未列出发布到Brand Portal的资产的所有静态演绎版。
* 的 **[!UICONTROL 演绎版]** 面板会列出资产的智能裁剪演绎版，但用户无法预览或下载智能裁剪演绎版。
* 下载对话框会列出选定资产的智能裁剪演绎版，但用户无法下载智能裁剪演绎版。
* 非管理员用户在下载资产时只能获取原始资产演绎版。 不会下载系统和自定义演绎版。
* 应用搜索过滤器下载资产时， `Download` 按钮在“下载”对话框中处于禁用状态，且不允许用户下载资产。
* 如果 `Smart Tags` 和（或） `Color Tags` ，则下载对话框会列出 `json` 文件作为演绎版并下载这些文件 `json` 文件。
* 匿名用户无法使用共享链接下载资产，因为该链接重定向到Brand Portal登录页面。
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

* When you share the Contribution folder’s URL using an email, Viewer and Editor roles face issues while accessing its parent folder using the breadcrumb.

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

要确定哪些平台经认证可随此版本的Brand Portal一起运行，请参阅 **支持触屏优化UI** 列 **用于创作用户界面的支持的浏览器** 部分 [技术要求](https://experienceleague.adobe.com/docs/experience-manager-65/deploying/introduction/technical-requirements.html).

## 链接 {#links}

* [Adobe Experience Manager adobe.com上的产品页](https://business.adobe.com/in/products/experience-manager/adobe-experience-manager.html)
* [Assets Brand Portal文档](https://experienceleague.adobe.com/docs/experience-manager-brand-portal/using/home.html)

## 产品访问和支持（受限网站） {#product-access-and-support-restricted-sites}

这些网站仅供客户使用。 如果您是客户并需要访问，请联系您的Adobe客户经理。

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

<!--
* [Customer Support]()
-->
