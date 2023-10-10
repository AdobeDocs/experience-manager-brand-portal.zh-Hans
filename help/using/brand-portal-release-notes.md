---
title: 发行说明
seo-title: Release Notes
description: 深入了解Adobe Experience Manager Assets Brand Portal 2023.10.0版本中的功能、增强功能、修复的关键问题和已知问题。
seo-description: Get an insight into the enhancements, critical issues fixed, and known issues in the Adobe Experience Manager Assets Brand Portal 2023.08.0 release.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Kirandeep Kour
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
exl-id: e4e89080-9863-4857-8f3a-fcd516ef3271
source-git-commit: 21fc4446c2ec56a58a3dcbf8362d661c6e8d3712
workflow-type: tm+mt
source-wordcount: '1312'
ht-degree: 6%

---

# 发行说明 {#release-notes}

深入了解Adobe Experience Manager Assets Brand Portal 2023.10.0版本中的新增功能、增强功能、修复的关键问题和已知问题。

## 版本信息 {#release-information}

| 产品 | Adobe Experience Manager Assets Brand Portal |
|---|---|
| 版本 | 2023.10.0 |
| 日期 | 2023年10 |

## 概述 {#overview}

Adobe Experience Manager (AEM) Assets Brand Portal可帮助您轻松地获取、控制经过批准的创意资产，并将这些资产安全地分发给跨设备的外部参与方和内部业务用户。 它有助于提高资产共享效率，加快资产上市速度，并降低不合规和未经授权访问的风险。 Brand Portal允许用户随时随地以公司批准的格式浏览、搜索、预览、下载和导出资源。

## 2023.10.0版的新增功能 {#whats-new-in-2023.10.0}

### 已修复的关键问题 {#critical-issues-fixed}

#### 错误修复 {#bug-fixes}

此版本包含以下错误修复：

* 无法保存 [!UICONTROL 日期] 和 [!UICONTROL 选项] 谓词 [!UICONTROL 智能收藏集].

* 此 [!UICONTROL 日期和时间] 在英语以外的区域设置中工作时，格式不一致。

* 搜索资产时， [!UICONTROL 删除] 按钮缺失。

* 如果 [!UICONTROL 标题] 字段包含多字节符号 [!UICONTROL 链接共享]，则无法下载报表。

* 查看PDF类型文档时，标签和工具提示未本地化。

#### 增强 {#enhancements}

此版本包括以下增强功能：

* 浏览时的性能改进 [!UICONTROL 收藏集].

* 使用OmniSearch字段执行部分搜索时，结果不准确。

## 之前版本

### 2023年8月版 {#aug-2023}

**错误修复和增强功能**
此版本包括以下增强功能：

* 改进了在上加载资产时的性能 [!UICONTROL 下载] 弹出窗口。
* 现在，当您下载资源或资源的演绎版时，将以其原始文件类型格式而不是zip文件格式下载。

此版本包含以下错误修复：

* 长标签或标记无法正确显示在搜索筛选器中。
* 无法在“下载”对话框上显示较长的演绎版名称。
* 无法在卡片视图中预览视频资产。

### 2023年5月版 {#may-2023}

**错误修复**
此版本包括对以下关键问题的修复：

* 如果从共享链接下载资产时出错，则 `Notice` 和 `Close` 错误提示的标签未本地化。
* Brand Portal显示 **请求标头字段太大** 使用访问搜索筛选器时出错 `Filter` 窗格。

**已知问题**
此版本包括以下已知问题：

* 资产源报表内容中的部分本地化。
* 用户配置文件的某些字段在用户配置文件上不可编辑。

### 2023年2月版 {#feb-2023}

**错误修复**

此版本包括对以下关键问题的修复：

* 无法在Brand Portal上更新配置文件图片。
* 内容树窗格无法调整大小。 如果文件名长于内容树的缺省宽度，则无法水平和垂直拖动内容树。 因此，较长的文件名是不可读的。
* 在搜索表单中使用两次的同一属性谓词的搜索结果不一致。
* 并非所有语言都本地化了中间登录页面上的文本。

**增强**

此版本包括以下增强功能：

* 现在提供了新的现代PDF查看器，以改进PDF资源的预览。
* 您现在可以选择为管理员启用或禁用资产源通知。 导航到 [!UICONTROL 常规设置] 然后启用或禁用 [!UICONTROL `Notify Administrator of asset contribution`].

  ![通知管理员资源贡献](assets/notify-admin.png)

* 如果禁用了请求访问权限，则未授权用户无法请求访问Brand Portal。
* 只有为Brand Portal配置的组织才会显示在配置文件选取器列表中。

**已知问题**

此版本包括以下已知问题：

* 资产源报表内容中的部分本地化。
* 用户配置文件的某些字段在用户配置文件上不可编辑。

### 2022年10月版 {#oct-2022}

**已修复的关键问题**

此版本包括对以下关键问题的修复：

* 将大型文件从Brand Portal复制到第三方工具时，响应缓慢。
* 选中呈现版本计数复选框时，用于选择单个呈现版本的复选框将被禁用。
* 搜索响应缓慢。

>[!IMPORTANT]
>
>AEM Assets Brand Portal中的Pulse通知将从2022年12月1日起停止。 您将继续接收以下事件的电子邮件通知，而不是Pulse通知：
>* 通过链接共享资产
>* 请求访问工作流
>* 共享贡献文件夹
>* 启动导出到AEM的过程
>* 已完成导出到AEM
>

### 2022年8月版 {#aug-2022}

**已修复的关键问题**

此版本包括对以下关键问题的修复：

* 当NUI无法在Experience Manager中处理资源时，Brand Portal显示不准确的资源导入状态。
* 当预览操作失败时，没有通知可传达该失败。
* 修复了每个资源的totalUploadedSize属性的不准确值。
* 当您单击 **下载所有项目** 并且资产有大量的演绎版可用，Brand Portal会下载无效的.ZIP文件。
* 某些字符串的翻译在Brand Portal用户界面中被截断。

### 2022年5月版 {#may-2022}

**新增功能**

 Brand Portal 现在，每十二小时执行一次自动作业，以删除发布到 AEM 的所有 Brand Portal 资产。 因此，您无需手动删除“贡献”文件夹中的资产，即可将文件夹大小保持在阈值限制以下。 

**已修复的关键问题**

此版本包括对以下关键问题的修复：

* 下载包含带有颜色标记的资产的文件夹或收藏集时，也会下载XML文件。
* 下载包含演绎版的视频时，Brand Portal会创建一个无效的.ZIP文件。
* 当您在AEM创作实例中创建预设和资源，并将其发布到Brand Portal，然后在下载资源时选择动态演绎版时，无法提取下载的.ZIP文件。
* 从Brand Portal上提供的某些文件夹下载视频资源时出现问题。
* 当您使用电子邮件共享Contribution文件夹的URL时，查看者和编辑者角色在使用痕迹导航访问其父文件夹时面临问题。
* 来源补充发布报表显示的作业开始时间不正确。

### 2022年2月版 {#feb-2022}

**新增功能**

* 来宾用户的会话超时阈值已从2小时减少到15分钟。
* 其他 **[!UICONTROL 查看页面]** 已为多页面PDF删除选项，因为用户现在可以从Adobe Document Cloud查看器查看PDF页面。
* 用户无法搜索、导航或打开文件夹。 用户界面反映错误消息： `Failed to load data`.
* 此 **[!UICONTROL 节目]** 面板不会列出发布到Brand Portal的资源的所有静态演绎版。
* 此 **[!UICONTROL 节目]** 面板列出了资源的智能裁剪演绎版，但是，用户无法预览或下载智能裁剪演绎版。
* 下载对话框列出了所选资源的智能裁剪演绎版，但是，用户无法下载智能裁剪演绎版。
* 非管理员用户在下载资源时仅获得原始资源演绎版。 未下载系统和自定义呈现版本。
* 应用搜索过滤器下载资源时， `Download` 下载对话框中禁用了按钮，不允许用户下载资产。
* 如果 `Smart Tags` 和（或） `Color Tags` 已启用，下载对话框会列出 `json` 文件作为演绎版并下载这些 `json` 文件，该文件位于存档的zip文件夹中。
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

要确定哪些平台经认证可以使用此版本的Brand Portal，请参阅 **支持触控优化的UI** 中的列 **支持创作用户界面的浏览器** 部分 [技术要求](https://experienceleague.adobe.com/docs/experience-manager-65/deploying/introduction/technical-requirements.html).

## 链接 {#links}

* [adobe.com上的Adobe Experience Manager产品页面](https://business.adobe.com/in/products/experience-manager/adobe-experience-manager.html)
* [Assets Brand Portal文档](https://experienceleague.adobe.com/docs/experience-manager-brand-portal/using/home.html)

## 产品访问和支持（受限制的站点） {#product-access-and-support-restricted-sites}

这些网站仅供客户使用。 如果您是客户并且需要访问权限，请联系您的Adobe客户经理。

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

<!--
* [Customer Support]()
-->
