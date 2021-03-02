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
translation-type: tm+mt
source-git-commit: 302bbf441453a760fe53d981a61b2eb014ebd1f0
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 9%

---


# 发行说明 {#release-notes}

深入了解Adobe Experience Manager Assets Brand Portal 2021.02.0版本中的新增功能、增强功能、已修复的关键问题和已知问题。

## 发行信息 {#release-information}

| 产品 | Adobe Experience Manager Assets Brand Portal |
|---|---|
| 版本号 | 2021.02.0 |
| 日期 | 2021年2月 |

## 概述 {#overview}

Adobe Experience Manager(AEM)Assets Brand Portal可帮助您轻松获取、控制获准的创意资产并将其安全地分发给外部各方和跨设备的内部业务用户。 它有助于提高资产共享的效率，加快资产的上市时间，并降低不合规和未授权访问的风险。 Brand Portal允许用户随时随地以公司批准的格式浏览、搜索、预览、下载和导出资产。

## 2021.02.0 的新增功能 {#whats-new-in-2021.02.0}

### 新增功能{#new-features}

此版本包含以下新增功能：

* 资产来源补充功能现在在AEM Assets上作为Cloud Service可用。 它允许Brand Portal用户将资产上传到允许的贡献文件夹，并将贡献文件夹从Brand Portal发布到AEM Assets作为Cloud Service实例。

* 在&#x200B;**[!UICONTROL 下载设置]**&#x200B;下增加了&#x200B;**[!UICONTROL 资产下载]**&#x200B;设置。 在下载文件夹、收藏集或批量下载资产时，系统会为每个资产创建一个单独的文件夹。 请参阅[下载设置](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#configure-download)。

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

此版本包含以下增强功能：

* 对于文件夹下载，将使用共享链接为每个资产创建一个单独的文件夹，而不管&#x200B;**[!UICONTROL 下载设置]**。
* Brand Portal **[!UICONTROL 使用情况报告]**&#x200B;已修改，仅反映活动的Brand Portal用户。

<!--
* The threshold of session timeout for the guest users has been reduced from 2 hours to 15 minutes.
* The additional **[!UICONTROL View pages]** option has been removed for multi-page PDFs as the user can now view the PDF pages from the Adobe Document Cloud Viewer.
-->


### 已修复{#critical-issues-fixed}的严重问题

此版本修复了以下关键问题：

* 如果仅下载了原始资产，资产会反映其自己的扩展，直到将扩展手动更改为zip后，才会打开。
* 单击导航箭头时，集合文件夹的用户界面不会响应。
* **[!UICONTROL 即]** 使文件夹为空，“列 **** 视图”中也会显示“创建”按钮。
* **[!UICONTROL 如果]** 在访问Brand Portal实例时绕过调度程序，则omni search将失败，并显示414错误消息(Request-URI Too Long)。
* 如果资产的文件名中包含逗号(`,`)，则会下载一个空的zip文件夹。
* 查看器用户可以选择将用户添加到他们创建的集合。
* 使用共享链接下载资产（缩略图或Web演绎版）时，会出现不一致的行为。

请参阅[Brand Portal 2021.02.0](whats-new.md)中的新增功能。

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

Brand Portal用户界面提供以下语言版本：

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

要确定哪些平台经认证可随此版本的Brand Portal一起运行，请参阅[技术要求](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/technical-requirements.html)的&#x200B;**创作用户界面支持的浏览器**&#x200B;部分中的&#x200B;**触屏优化UI支持**&#x200B;列。

## 链接 {#links}

* [adobe.com 上的 Adobe Experience Manager 产品页面](http://www.adobe.com/in/marketing-cloud/experience-manager.html)
* [Assets Brand Portal文档](https://helpx.adobe.com/cn/experience-manager/brand-portal/user-guide.html)

## 产品访问和支持（受限站点）{#product-access-and-support-restricted-sites}

这些网站仅适用于客户。如果您是Adobe并需要访问，请与您的客户经理联系。

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

* [产品访问](https://login.marketing.adobe.com)

* [Adobe客户关怀](https://helpx.adobe.com/contact.html)
