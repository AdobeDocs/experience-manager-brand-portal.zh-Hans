---
title: 发行说明
seo-title: 发行说明
description: 深入了解Adobe Experience Manager资产品牌门户2020.10.0版本中的功能、增强功能、已修复的关键问题和已知问题。
seo-description: 深入了解Adobe Experience Manager资产品牌门户2020.10.0版本中的增强功能、已修复的关键问题和已知问题。
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: 5cf924ce71433e33506449bbad608d5e57a41b8d
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 9%

---


# 发行说明 {#release-notes}

深入了解Adobe Experience Manager资产品牌门户2020.10.0版本中的新增功能、增强功能、已修复的关键问题和已知问题。

## 发行信息 {#release-information}

| 产品 | Adobe Experience Manager资产品牌门户 |
|---|---|
| 版本 | 2020.10.0 |
| 日期 | 2020年10月 |

## 概述 {#overview}

Adobe Experience Manager(AEM)Assets Brand Portal可帮助您轻松获取、控制获准的创意资产并跨设备安全地将其分发给外部方和内部业务用户。 它有助于提高资产共享的效率，加快资产的上市时间，并降低不合规和未经授权访问的风险。 Brand Portal允许用户随时随地以公司批准的格式浏览、搜索、预览、下载和导出资产。

## 2020.10.0 的新增功能 {#whats-new-in-2020.10.0}

### New Features {#new-features}

此版本包含以下新增功能：

* 在列表 **[!UICONTROL 视图中]** ,“下载”对话框进行了改头换面，增加了一些选项，可排除不需要的演绎版、对类似资产类型应用同一套规则以及下载选定的资产演绎版。 请参 [阅从Brand Portal下载资产的步骤](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets)。

<!--
* The new **[!UICONTROL Download]** dialog now appears with all the renditions of the selected assets or folders containing assets in a list view, wherein the Brand Portal users can apply same set of renditions for similar asset types and download the selected asset renditions. 
-->

* 现在，只需 **[!UICONTROL 单击一]**&#x200B;下，即可从所 **[!UICONTROL 有Brand Portal页面]****** 导航到文件、集合和共享链接。

* 现在， **[!UICONTROL 资产]** 详细信息页面中的“演绎版”面板允许Brand Portal用户选择原始资产和（或）特定资产演绎版，并直接从“演绎版”面板下载它们，而无需打开“下载 **[!UICONTROL ”对话]** 框 **** 。 请参 [阅从资产详细信息页面下载资产](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets-from-asset-details-page)。

<!--
Brand Portal users can exclude specific renditions which are not required and directly download the original asset and its renditions from the **[!UICONTROL Renditions]** panel on the asset details page. 
-->

* 除了现有的下 **[!UICONTROL 载配置]** ,Brand Portal管理员还可以将不同用户组的权 [限配置为视图](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#configure-download-permissions) ，并（或）从资产详细信息页面下载原始资产及其演绎版。 这些配置将定义哪些人员可以访问和（或）下载资产演绎版。

### 增强功能 {#enhancements}

此版本包含以下增强功能：

* 来宾用户的会话超时阈值已从2小时减少到15分钟。
* 对于多 **[!UICONTROL 页PDF]** ，已删除附加的视图页面选项，因为用户现在可以从Adobe Document Cloud查看器视图PDF页面。


<!--
### Critical Issues Fixed {#critical-issues-fixed}

This release includes fixes to the following critical issue:

* The users are not able to view the PDF pages if the PDF contains sub assets.
-->

### 已知问题 {#known-issues}

此版本包含以下已知问题：

* 在资产报 **[!UICONTROL 表上搜索]** ，会显示产品界面上的处理情况，而没有搜索结果。
* 非管理员用户在资产详细信息页面上无法看到视频DM编码。
* 在下载对话框中，单个资产演绎版的大小和总下载大小的对齐方式会失真。



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

要确定哪些平台经认证可随此版本的Brand Portal一起运行，请参阅“技术 **要求”的“支持的创作用户界面浏览器** ”一节中 **的“触屏优化UI支持** ”一 [列](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/technical-requirements.html)。

## 链接 {#links}

* [adobe.com 上的 Adobe Experience Manager 产品页面](http://www.adobe.com/in/marketing-cloud/experience-manager.html)
* [Assets Brand Portal文档](https://helpx.adobe.com/cn/experience-manager/brand-portal/user-guide.html)

## Product Access and Support (Restricted Sites) {#product-access-and-support-restricted-sites}

这些网站仅适用于客户。如果您是Adobe并需要访问，请与客户经理联系。

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

* [产品访问](https://login.marketing.adobe.com)

* [Adobe客户关怀](https://helpx.adobe.com/contact.html)
