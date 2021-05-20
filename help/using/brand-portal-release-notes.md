---
title: 发行说明
seo-title: 发行说明
description: 深入了解Adobe Experience Manager Assets Brand Portal 2021.02.0版本中的功能、增强功能、已修复的关键问题和已知问题。
seo-description: 深入了解Adobe Experience Manager Assets Brand Portal 2021.02.0版本中的增强功能、已修复的关键问题和已知问题。
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
exl-id: e4e89080-9863-4857-8f3a-fcd516ef3271
source-git-commit: d2bfd06f8cd8a9e78efbc8dd92880e0faae39176
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 8%

---

# 发行说明 {#release-notes}

深入了解Adobe Experience Manager Assets Brand Portal 2021.02.0版本中的新增功能、增强功能、已修复的关键问题和已知问题。

## 发行信息 {#release-information}

| 产品 | Adobe Experience Manager Assets Brand Portal |
|---|---|
| 版本号 | 2021.02.0 |
| 日期 | 2021年2月 |

## 概述 {#overview}

Adobe Experience Manager(AEM)Assets Brand Portal可帮助您跨设备轻松获取、控制和安全地将已批准的创意资产分发给外部各方和内部业务用户。 它有助于提高资产共享的效率，加快资产的上市时间，并降低不合规和未经授权访问的风险。 Brand Portal允许用户随时随地以公司批准的格式浏览、搜索、预览、下载和导出资产。

## 2021.02.0 的新增功能 {#whats-new-in-2021.02.0}

### 新增功能{#new-features}

此版本包括以下新增功能：

* AEM Assets as aCloud Service现在有权使用预配置的Brand Portal实例。 Cloud Manager用户可以在AEM Assets上作为Cloud Service实例激活Brand Portal。

* 资产源功能现在在AEM Assets上作为Cloud Service提供。 它允许Brand Portal用户将资产上传到允许的贡献文件夹，并将贡献文件夹从Brand Portal作为Cloud Service实例发布到AEM Assets。

* 在&#x200B;**[!UICONTROL 下载设置]**&#x200B;下，引入了额外的&#x200B;**[!UICONTROL 资产下载]**&#x200B;设置。 下载文件夹、收藏集或批量下载资产时，它会为每个资产创建一个单独的文件夹。

<!-- 
* The **[!UICONTROL Download]** dialog is revamped in a list view with additional options to exclude the renditions which are not required, apply the same set of rules for similar asset types, and download the selected asset renditions. See [steps to download assets from Brand Portal](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets).
-->

<!--
* The new **[!UICONTROL Download]** dialog now appears with all the renditions of the selected assets or folders containing assets in a list view, wherein the Brand Portal users can apply same set of renditions for similar asset types and download the selected asset renditions. 
-->

<!-- 
* Navigation to the **[!UICONTROL Files]**, **[!UICONTROL Collections]**, and **[!UICONTROL Shared Links]** is now possible from all the Brand Portal pages in one-click.  

* The **[!UICONTROL Renditions]** panel in the asset details page now allows the Brand Portal users to select the original asset and (or) specific asset renditions, and directly download them from the **[!UICONTROL Renditions]** panel without having to open the **[!UICONTROL Download]** dialog. See [download assets from asset details page](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets-from-asset-details-page).
-->

<!--
Brand Portal users can exclude specific renditions which are not required and directly download the original asset and its renditions from the **[!UICONTROL Renditions]** panel on the asset details page. 
-->

<!-- 
* In addition to the existing **[!UICONTROL Download]** configurations, the Brand Portal administrators can also [configure permissions for different group of users](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#configure-download-permissions) to view and (or) download the original asset and its renditions from the asset details page. These configurations will define who can access and (or) download the asset renditions.
-->

### 增强功能 {#enhancements}

此版本包括以下增强功能：

* 对于文件夹下载，使用共享链接为每个资产创建一个单独的文件夹，而与&#x200B;**[!UICONTROL 下载设置]**&#x200B;无关。
* 已修改Brand Portal **[!UICONTROL 使用情况报表]**，以仅反映活动的Brand Portal用户。

<!--
* The threshold of session timeout for the guest users has been reduced from 2 hours to 15 minutes.
* The additional **[!UICONTROL View pages]** option has been removed for multi-page PDFs as the user can now view the PDF pages from the Adobe Document Cloud Viewer.
-->


### 已修复{#critical-issues-fixed}的关键问题

此版本包括对以下关键问题的修复：

* 如果仅下载原始资产，资产将反映其自身的扩展，并且在将扩展手动更改为zip之前不会打开资产。
* 单击导航箭头时，收藏集文件夹的用户界面未做出响应。
* **** 即使文件夹为空，列 **** 视图中也会显示创建按钮。
* **[!UICONTROL 如果]** 在访问Brand Portal实例时绕过调度程序，则Omni search会失败，并显示414错误消息（请求URI过长）。
* 如果资产的文件名中包含逗号(`,`)，则会下载空的zip文件夹。
* 查看器用户可以选择将用户添加到他们创建的集合。
* 使用共享链接下载资产（缩略图或Web演绎版）时，会出现不一致的行为。

请参阅[Brand Portal 2021.02.0的新增功能](whats-new.md)。


### 已知问题 {#known-issues}

此版本包括以下已知问题：

* 用户不会收到有关资产源发布工作流的电子邮件通知。

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
* 韩语

## 经过认证的平台 {#certified-platforms}

要确定哪些平台经认证可以随此版本的Brand Portal一起运行，请参阅[技术要求](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/technical-requirements.html)的“创作用户界面支持的浏览器”部分&#x200B;**中的表格中的**&#x200B;触屏优化UI **支持列。**

## 链接 {#links}

* [adobe.com 上的 Adobe Experience Manager 产品页面](http://www.adobe.com/in/marketing-cloud/experience-manager.html)
* [Assets Brand Portal文档](https://helpx.adobe.com/cn/experience-manager/brand-portal/user-guide.html)

## 产品访问和支持（受限站点）{#product-access-and-support-restricted-sites}

这些网站仅适用于客户。如果您是客户并需要访问，请联系您的Adobe客户经理。

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

* [产品访问](https://login.marketing.adobe.com)

* [Adobe客户关怀](https://helpx.adobe.com/contact.html)
