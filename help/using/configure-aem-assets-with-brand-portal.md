---
title: 使用 Brand Portal 配置 AEM Assets
seo-title: 使用 Brand Portal 配置 AEM Assets
description: 深入了解如何配置AEM Assets与Brand Portal。
seo-description: 深入了解如何配置AEM Assets与Brand Portal。
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
role: Administrator
exl-id: 261c0e84-6b3d-459c-b6b9-a9af106d6943
source-git-commit: d2bfd06f8cd8a9e78efbc8dd92880e0faae39176
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 22%

---

# 使用 Brand Portal 配置 AEM Assets {#configure-integration}

使用Brand Portal配置Adobe Experience Manager Assets可为Brand Portal用户启用资产发布、资产分发和资产贡献功能。 它允许AEM Assets用户与Brand Portal用户发布和分发资产。 Brand Portal用户可以访问共享资产并进行贡献，方法是将新资产上传到资产贡献文件夹，然后将其发布回AEM Assets。

支持在以下位置配置AEM Assets与Brand Portal:
* AEM Assets as a Cloud Service
* AEM Assets（内部部署版和Managed Service）6.3及更高版本

AEM Assets as aCloud Service通过从Cloud Manager激活Brand Portal，自动配置为Brand Portal。 激活工作流会在后端创建所需的配置，并在与AEM Assets(作为Cloud Service实例)相同的IMS组织上激活Brand Portal。

而是，AEM Assets（内部部署版和托管服务版）会使用Brand Portal开发人员控制台通过Adobe手动配置，该控制台可获取AdobeIdentity Management服务(IMS)令牌以授权Brand Portal租户。

>[!NOTE]
>
>***适用于AEM Assets 6.3及更高版本***
>
>以前，Brand Portal是通过旧版OAuth网关在经典界面中配置的，该网关使用JSON Web令牌(JWT)交换获取IMS令牌以进行授权。
>
>自2020年4月6日起，不再支持通过旧版OAuth进行配置，并且已通过Adobe开发人员控制台更改为配置。


>[!TIP]
>
>***仅适用于现有客户（内部部署版和托管服务版）***
>
>旧版OAuth网关配置将继续适用于现有客户。
>
>如果您在旧版OAuth网关配置中遇到问题，请删除现有配置，并通过Adobe开发人员控制台创建新配置。

使用Brand Portal配置AEM Assets的步骤因AEM版本以及您是首次配置还是升级现有配置而异：

| **AEM 版本** | **新配置** | **升级配置** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [激活Brand Portal](https://docs.adobe.com/content/help/zh-Hans/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5（6.5.4.0及更高版本）** | [创建配置](https://docs.adobe.com/content/help/zh-Hans/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [升级配置](https://docs.adobe.com/content/help/zh-Hans/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4（6.4.8.0及更高版本）** | [创建配置](https://docs.adobe.com/content/help/zh-Hans/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [升级配置](https://docs.adobe.com/content/help/zh-Hans/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3（6.3.3.8及更高版本）** | [创建配置](https://helpx.adobe.com/cn/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [升级配置](https://helpx.adobe.com/cn/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | 联系支持人员 | 联系支持人员 |
