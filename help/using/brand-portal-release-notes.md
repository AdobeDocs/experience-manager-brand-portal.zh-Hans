---
title: 发行说明
description: 洞察 Adobe Experience Manager Assets Brand Portal 2026.01.01 版本中的功能、增强功能、已修复的关键问题以及已知问题。
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
exl-id: e4e89080-9863-4857-8f3a-fcd516ef3271
source-git-commit: ff2dc92ea112a95c90724f06f141221ffdef33a1
workflow-type: tm+mt
source-wordcount: '1595'
ht-degree: 96%

---

# 发行说明 {#release-notes}

洞察 Adobe Experience Manager Assets Brand Portal 2026.01.01 版本中的新功能、增强功能、已修复的关键问题以及已知问题。

## 版本信息 {#release-information}

| 产品 | Adobe Experience Manager Assets Brand Portal |
|---|---|
| 版本 | 2026.01.01 |
| 日期 | 2026年1月 |

## 概述 {#overview}

Adobe Experience Manager (AEM) Assets Brand Portal 可帮助您轻松获取、控制已批准的创意资产，并在各类设备上安全地向外部各方和内部商务用户分发这些资产。它有助于提高资产共享的效率，加快资产的上市时间，降低违规和未经授权访问的风险。 Brand Portal 允许用户随时随地以公司认可的格式浏览、搜索、预览、下载和导出资产。

## 2026.01.01 版本中的新增功能 {#whats-new-in-2026.01.01}

### 修复了关键问题 {#critical-issues-fixed}

#### 增强功能 {#enhancements}

此版本包括以下增强功能：

* 在“管理工具”面板>“Dynamic Media配置”中，您现在可以使用&#x200B;**[!UICONTROL 重置]**&#x200B;按钮来清除任何更改、重置密码并将配置恢复为默认状态。

* Brand Portal在发布到AEM之前，会验证源文件夹以确保其中至少包含一个资源，从而帮助防止发布不完整。

## 以前的版本

### 2024 年 10 月版本 {#oct-2024}

**错误修复和增强功能** 

此版本包含以下错误修复：

* 与搜寻导入事件相关的电子邮件通知未被发送。
* 在使用搜索筛选条件时，[!DNL Brand Portal] 在搜索筛选条件窗口中显示重复的文件夹。
* 下载包含未许可资产且名称中包含特殊字符的收藏集时，无法正常下载。
* 在导航至[!UICONTROL 搜索表单编辑器]时，标签未进行本地化。
* 链接分享窗口中的标签未进行本地化。
* 无法下载名称中带有特殊字符的视频。
* 从 [!DNL Adobe Experience Manager Assets] 向 Brand Portal 发布和取消发布资产的操作无法正常进行。
* 无法播放从 Brand Portal 下载的视频。

### 2024 年 2 月版本 {#feb-2024}

**错误修复和增强功能** 

此版本包含以下错误修复：

* 在土耳其地区，无法下载受 DRM 保护的数字资产。
* 无法打开和下载包含多行标题资产的现有报告。
* 当您使用操作栏中的[!UICONTROL 下载]按钮下载资产时，最多可下载 1000 个资产。
* 在内容树中查看时，PSD 类型资产的名称不正确。
* 资产详情页面上的[!UICONTROL 删除演绎版]选项无法使用。
* 下载弹出窗口中资产标题和大小不一致。
* 在创建报告时，标签未进行本地化。
* 在 Brand Portal 中，支持管理员被称作管理员。

### 2023 年 10 月版本 {#oct-2023}

**错误修复与增强功能**
此版本包含以下增强功能：

* 在浏览[!UICONTROL 收藏夹]时，性能得到了提升。

* 在使用 OmniSearch 字段进行部分搜索时，搜索结果有所改进。

此版本包含以下错误修复：

* 无法将[!UICONTROL 日期]和[!UICONTROL 选项]谓词保存到[!UICONTROL 智能收藏集]中。

* 在非英语区域设置下工作时，[!UICONTROL 日期和时间]格式不一致。

* 在搜索资产时，缺少[!UICONTROL 删除]按钮。

* 如果[!UICONTROL 标题]字段在[!UICONTROL 链接共享]中包含多字节符号，则无法下载报告。

* 查看 PDF 类型的文档时，标签和工具提示未本地化。

### 2023 年 8 月版本 {#aug-2023}

**错误修复与增强功能**
此版本包含以下增强功能：

* 在[!UICONTROL 下载]弹出窗口中加载资产时的性能改进。
* 当您下载资产或资产的演绎版时，现在会以原始文件类型格式下载，而不是以 zip 文件格式下载。

此版本包含以下错误修复：

* 长标签或标记在搜索筛选条件中显示不当。
* 无法在“下载”对话框中显示长演绎版名称。
* 无法在卡片视图中预览视频资产。

### 2023 年 5 月版本 {#may-2023}

**错误修复**
此版本包含对以下关键问题的修复：

* 如果从共享链接下载资产时发生错误，错误提示中的 `Notice` 和 `Close` 标签未进行本地化。
* 在使用 `Filter` 窗格访问搜索筛选条件时，Brand Portal 显示&#x200B;**请求标头字段过大**&#x200B;错误。

**已知问题**
此版本包括以下已知问题：

* 资产搜寻报告内容中的部分本地化。
* 用户轮廓中的大部分字段都是可编辑的。

### 2023 年 2 月版本 {#feb-2023}

**错误修复**

此版本包含对以下关键问题的修复：

* 无法在 Brand Portal 上更新轮廓图片。
* 内容树窗格不可调整大小。如果文件名长度超过了内容树的默认宽度，则无法水平和垂直拖动内容树。因此，较长的文件名不可读。
* 在搜索表单中两次使用的同一属性谓词，其搜索结果不一致。
* 中间登录页面上的文本未针对所有语言进行本地化。

**增强功能**

此版本包括以下增强功能：

* 现已推出全新的现代 PDF 查看器，可提供更佳的 PDF 资产预览体验。
* 您现在可以选择为管理员启用或禁用资产搜寻通知。导航至[!UICONTROL 常规设置]，然后启用或禁用 [!UICONTROL `Notify Administrator of asset contribution`]。

  ![通知管理员进行资产贡献](assets/notify-admin.png)

* 如果访问请求被禁用，则未经授权的用户无法请求访问 Brand Portal 。
* 只有为 Brand Portal 配置的组织才会在轮廓选择器列表中可见。

**已知问题**

此版本包括以下已知问题：

* 资产搜寻报告内容中的部分本地化。
* 用户轮廓中的大部分字段都是可编辑的。

### 2022 年 10 月版本 {#oct-2022}

**修复了关键问题**

此版本包含对以下关键问题的修复：

* 从 Brand Portal 向第三方工具复制大文件时，响应速度较慢。
* 当您选中演绎版复选框时，用于选择单个演绎版的复选框被禁用。
* 搜索响应时间慢。

>[!IMPORTANT]
>
>AEM Assets Brand Portal 中的 Pulse 通知将于 2022 年 12 月 1 日起停止。您将继续收到以下事件的电子邮件通知，而不是 Pulse 通知：
>
>* 通过链接共享资产
>* 请求访问工作流
>* 共享贡献文件夹
>* 开始导出至 AEM
>* 已完成导出至 AEM
>

### 2022 年 8 月版本 {#aug-2022}

**已修复关键问题**

此版本包含对以下关键问题的修复：

* 当 NUI 无法在 Experience Manager 中处理资产时，Brand Portal 显示不准确的资产导入状态。
* 预览操作失败时，没有告知失败情况的通知。
* 修正了每项资产的 `totalUploadedSize` 属性的不准确值。
* 当您点击&#x200B;**下载所有项目**，并且资产有大量可用的演绎版本时，Brand Portal 下载无效的 .ZIP 文件。
* Brand Portal 用户界面上的一些字符串翻译被截断。

### 2022 年 5 月版本 {#may-2022}

**新增功能**

Brand Portal 现在每十二小时执行一次自动任务，以删除所有已发布到 AEM 的 Brand Portal 资产。因此，您无需手动删除“贡献”文件夹中的资产，即可将文件夹大小保持在阈值限制以下。

**修复了关键问题**

此版本包含对以下关键问题的修复：

* 当您下载包含带有颜色标记的资产的文件夹或收藏集时，也会同时下载一个 XML 文件。
* 当您下载包含演绎版的视频时，Brand Portal 会创建一个无效的 .ZIP 文件。
* 当您在 AEM Author 环境上创建预设和资产，并将其发布到 Brand Portal 时，您可以在下载资产时选择动态演绎版。但是，您无法提取下载的 .ZIP 文件。此问题导致无法访问下载的内容。
* 从 Brand Portal 上的某些文件夹下载视频资产时出现问题。
* 当您使用电子邮件共享贡献文件夹的 URL 时，查看者和编辑者角色在使用痕迹导航访问其父文件夹时会遇到问题。
* 搜寻发布的报告显示错误的任务开始时间。

### 2022 年 2 月版本 {#feb-2022}

**新增功能**

* 访客用户的会话超时阈值从 2 小时缩短至 15 分钟。
* 移除了多页 PDF 中额外的&#x200B;**[!UICONTROL 查看页面]**&#x200B;选项，因为用户现在可以通过 Adobe Document Cloud 查看器查看 PDF 页面。
* 用户无法搜索、导航或打开文件夹。用户界面反映错误消息：`Failed to load data`。
* **[!UICONTROL 演绎版]**&#x200B;面板未列出发布到 Brand Portal 的资产的所有静态演绎版。
* **[!UICONTROL 演绎版]**&#x200B;面板列出了资产的智能裁剪演绎版，但用户无法预览或下载这些智能裁剪演绎版。
* 下载对话框列出了所选资产的智能裁剪演绎版，但用户无法下载这些智能裁剪演绎版。
* 非管理员用户在下载资产时，仅能获取原始资产演绎版。系统和自定义演绎版不下载。
* 在应用搜索筛选条件下载资产时，下载对话框中的 `Download` 按钮被禁用，用户无法下载资产。
* 如果启用 `Smart Tags` 和（或）`Color Tags`，下载对话框将 `json` 文件列为演绎版，并在存档的 zip 文件夹中下载这些 `json` 文件。
* 匿名用户无法使用共享链接下载资产，因为该链接会重定向至 Brand Portal 登录页面。
* 系统没有正确反映当前并发用户的数量。

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

Brand Portal 用户界面提供以下语言版本：

* 英语
* 德语
* 法语
* 西班牙语
* 意大利语
* 巴西葡萄牙语
* 日语
* 简体中文
* 韩语

## 认证平台 {#certified-platforms}

要查看哪些平台已获得此 Brand Portal 版本的认证，请查看[技术要求](https://experienceleague.adobe.com/zh-hans/docs/experience-manager-65/content/implementing/deploying/introduction/technical-requirements)中&#x200B;**支持创作用户界面的浏览器**&#x200B;部分的&#x200B;**支持触控优化的 UI**&#x200B;列。

## 链接 {#links}

* [adobe.com 上的 Adobe Experience Manager 产品页面](https://business.adobe.com/in/products/experience-manager/adobe-experience-manager.html)
* [Assets Brand Portal 文档](https://experienceleague.adobe.com/zh-hans/docs/experience-manager-brand-portal/using/home)

## 产品访问和支持（受限网站） {#product-access-and-support-restricted-sites}

这些网站仅对客户开放。如果您是客户且需要访问权限，请联系您的 Adobe 客户经理。

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

<!--
* [Customer Support]()
-->
