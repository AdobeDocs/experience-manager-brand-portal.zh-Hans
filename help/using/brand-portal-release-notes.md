---
title: 发行说明
seo-title: 发行说明
description: 深入了解Adobe Experience Manager Assets Brand Portal 6.4.6版本中的功能、增强功能、已修复的关键问题和已知问题。
seo-description: 深入了解Adobe Experience Manager Assets Brand Portal 6.4.6版本中的增强功能、已修复的关键问题和已知问题。
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: 6b03229b72a1912be57c2bc1b7e47a017d3dca7e

---


# 发行说明 {#release-notes}

深入了解Adobe Experience Manager Assets Brand Portal 6.4.6版本中的新增功能、增强功能、已修复的关键问题和已知问题。

## 发行信息 {#release-information}

| 产品 | Adobe Experience Manager Assets Brand Portal |
|---|---|
| 版本 | 6.4.6 |
| 日期 | 2020年3月 |

## 概述 {#overview}

Adobe Experience Manager(AEM)Assets Brand Portal可帮助您轻松获取、控制获准的创意资产并跨设备安全地将其分发给外部方和内部业务用户。 它有助于提高资产共享的效率，加快资产的上市时间，并降低不合规和未授权访问的风险。 Brand Portal允许用户随时随地以公司批准的格式浏览、搜索、预览、下载和导出资产。

## 6.4.6 的新增功能 {#what-s-new-in-646}

### 新增功能 {#new-feature}

此版本包含以下新增功能：

* 客人登录Brand Portal的Captcha。 有关详细 [信息，请参阅Brand Portal客人访问](../using/guest-access.md) 。

### 增强功能 {#enhancements-646}

此版本的Brand Portal包括以下增强功能：

* AEM资产现在通过Adobe I/O配置了Brand Portal，后者为Brand Portal租户购买IMS令牌以授权。

   >[!NOTE]
   >
   >从2020年4月6日起，不再支持通过旧版OAuth进行配置，并已更改为通过Adobe I/O进行配置。


   >[!TIP]
   >
   >***仅限现有客户***
   >
   >建议继续使用现有的传统OAuth网关配置。 如果您遇到旧版OAuth网关配置问题，请删除现有配置并通过Adobe I/O创建新配置。


有关详细信息，请参 [阅配置AEM资产与Brand Portal](configure-aem-assets-with-brand-portal.md)


### 已修复的关键问题 {#critical-issues-fixed}

此版本包括对以下关键问题的修复：

* 元数据模式下拉值在资产属性中不可见。

* 元数据子架构不显示基于资产属性中的mime类型的选项卡。

* 取消发布元数据模式会填充错误消息，但模式会在后端删除。

* 预览图像不显示已发布的资产。

* 用户无法发布或取消发布名称中包含单报价的资产。

* 下载多个资产时不显示条款和条件。

* 已解决较小的安全漏洞。

### 已知问题 {#known-issues}

此版本包含以下已知问题：

* 在升级到Adobe I/O后，Brand Portal用户无法将贡献文件夹资产发布到AEM资产。

* 下载资产时，“排除系统演绎版”选项无法正常工作。

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

要确定哪些平台经认证可随此版本的Brand Portal一起运行，请参阅“技术要求”的“支持的创作用户界面浏览器 **”一节中的“触屏优化UI** 支持” **一列**[](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/technical-requirements.html)。

## 链接 {#links}

* [adobe.com 上的 Adobe Experience Manager 产品页面](http://www.adobe.com/in/marketing-cloud/experience-manager.html)
* [Assets Brand Portal文档](https://helpx.adobe.com/experience-manager/brand-portal/user-guide.html)

## Product Access and Support (Restricted Sites) {#product-access-and-support-restricted-sites}

这些网站仅适用于客户。如果您是客户并需要访问，请与您的Adobe客户经理联系。

* [](https://daycare.day.com) 产 [品访问](https://login.marketing.adobe.com)

* [Adobe客户关怀](https://helpx.adobe.com/contact.html)
