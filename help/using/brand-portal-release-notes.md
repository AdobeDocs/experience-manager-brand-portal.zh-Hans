---
title: 发行说明
seo-title: 发行说明
description: 深入了解Adobe Experience Manager资产品牌门户6.4.6.2版中的功能、增强功能、已修复的关键问题和已知问题。
seo-description: 深入了解Adobe Experience Manager资产品牌门户6.4.6.2版本中的增强功能、已修复的关键问题和已知问题。
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: 70640f9fa605d56160f01fde577ee699cfaac08d
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 7%

---


# 发行说明 {#release-notes}

深入了解Adobe Experience Manager资产品牌门户6.4.6.2版本中的新增功能、增强功能、已修复的关键问题和已知问题。

## 发行信息 {#release-information}

| 产品 | Adobe Experience Manager资产品牌门户 |
|---|---|
| 版本 | 6.4.6.2 |
| 日期 | 2020年6月 |

## 概述 {#overview}

Adobe Experience Manager(AEM)资产品牌门户可帮助您轻松获取、控制获准的创意资产并跨设备安全地将其分发给外部方和内部业务用户。 它有助于提高资产共享的效率，加快资产的上市时间，并降低不合规和未经授权访问的风险。 Brand Portal允许用户随时随地以公司批准的格式浏览、搜索、预览、下载和导出资产。

## 6.4.6.2 的新增功能 {#what-s-new-in-6462}

### 已修复严重问题 {#critical-issues-fixed-6462}

此版本包括对以下关键问题的修复：

* 从Brand Portal中删除已发布的元数据模式会导致错误。

* 如果管理员通过Adobe开发人员控制台使用Brand Portal配置Experience Manager资产6.5.4，则Brand Portal用户将无法将贡献文件夹的资产从Brand Portal发布到Experience Manager。

* 重复复制父文件夹会导致冲突。

* 用户无法生成链接共享报告。

* 用户可以使用copyPage命令复制Brand Portal端点的MAC机密。

* 导致在VA5克隆上重新建立索引的cq标记。


### 已知问题 {#known-issues-6462}

此版本包含以下已知问题：

* 查看器用户不得共享集合的链接，但产品界面中会显示共享选项。

* 如果层次结构中的文件夹是从AEM Assets重命名的，并且包含资产的嵌套文件夹已发布到Brand Portal，则只有在根文件夹再次发布后，该文件夹的标题才会在Brand Portal中更新。


## 6.4.6 的新增功能 {#what-s-new-in-646}

### New Features {#new-feature}

此版本包含以下新增功能：

* 客人登录Brand Portal时使用的Captcha。 See, [Brand Portal guest access](../using/guest-access.md) for more information.

* AEM Assets云服务现在支持Brand Portal。 您可以配置AEM Assets可以通过Brand Portal服务，以便与Brand Portal用户共享和分发资产。
有关详细信息，请参 [阅使用Brand Portal配置AEM Assets云服务](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html)。

### 增强功能 {#enhancements-646}

此版本的Brand Portal包含以下增强功能：

* 在AEM 6.3及更高版本中，AEM Assets与Brand Portal之间的授权渠道已更改。 AEM Assets现在通过Adobe开发人员控制台配置了品牌门户，该控制台为您的品牌门户租户购买IMS令牌以进行授权。

>[!NOTE]
>
>从2020年4月6日起，不再支持通过旧版OAuth进行配置，并且已更改为通过Adobe开发人员控制台进行配置。

>[!TIP]
>
>***仅限现有客户***
>
>旧版OAuth网关配置将继续为现有客户工作。
>
>如果您在旧版OAuth网关配置中遇到问题，请删除现有配置并通过Adobe开发人员控制台创建新配置。

For more information, see [Configure AEM Assets with Brand Portal](configure-aem-assets-with-brand-portal.md)

### 已修复严重问题 {#critical-issues-fixed}

此版本包括对以下关键问题的修复：

* 元数据模式下拉值在资产属性中不可见。

* 元数据子架构不显示基于资产属性中的mimetype的选项卡。

* 取消发布元数据模式会填充错误消息，尽管在后端删除了模式。

* 预览图像不显示已发布的资产。

* 用户无法发布或取消发布名称中包含单一报价的资产。

* 下载多个资产时不显示条款和条件。

* 已解决次要安全漏洞。

### 已知问题 {#known-issues}

此版本包含以下已知问题：

* 在升级到AEM 6.5.4上的Adobe开发人员控制台时，Brand Portal用户无法将贡献文件夹资产发布到AEM Assets。

   此问题将在下一个Service Pack 6.5.5中修复。

   要立即修复AEM 6.5.4，建议下载 [修补程序](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) ，并在创作实例上安装。

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

要确定哪些平台经认证可随此版本的Brand Portal一起运行，请参阅“技术 **要求”的“支持的创作用户界面浏览器** ”一节中 **的“触屏优化UI支持** ”一 [列](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/technical-requirements.html)。

## 链接 {#links}

* [adobe.com 上的 Adobe Experience Manager 产品页面](http://www.adobe.com/in/marketing-cloud/experience-manager.html)
* [Assets Brand Portal文档](https://helpx.adobe.com/cn/experience-manager/brand-portal/user-guide.html)

## Product Access and Support (Restricted Sites) {#product-access-and-support-restricted-sites}

这些网站仅适用于客户。如果您是客户并需要访问，请与您的Adobe客户经理联系。

* [https://daycare.day.com](https://daycare.day.com)

* [产品访问](https://login.marketing.adobe.com)

* [Adobe客户关怀](https://helpx.adobe.com/contact.html)
