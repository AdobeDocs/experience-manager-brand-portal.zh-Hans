---
title: 使用 Brand Portal 配置 AEM Assets
seo-title: 使用 Brand Portal 配置 AEM Assets
description: 深入了解如何通过Brand Portal配置AEM Assets。
seo-description: 深入了解如何通过Brand Portal配置AEM Assets。
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: de21e84b93a657570db2024c2ceba58704ba5844
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 10%

---


# 使用 Brand Portal 配置 AEM Assets {#configure-integration}

将Adobe Experience Manager资产配置为Adobe Experience Manager资产品牌门户的Cloud Service后，您便可以通过Brand Portal用户发布和分发资产。 而使用Brand Portal配置AEM 6.3（及更高版本）则可为Brand Portal用户启用资产发布、资产分发和资产贡献功能。

Adobe Experience Manager资产通过Adobe开发者控制台配置了品牌门户，该控制台为您的品牌门户租户购买AdobeIdentity Management服务(IMS)令牌以授权。

>[!NOTE]
>
>***适用于AEM Assets6.3及更高版本***
>
>以前，Brand Portal通过旧版OAuth Gateway在经典界面中配置，该网关使用JSON Web令牌(JWT)交换获取IMS令牌进行授权。
>
>从2020年4月6日起，不再支持通过旧版OAuth进行配置，并且已通过Adobe开发人员控制台更改为进行配置。


>[!TIP]
>
>***仅限现有客户***
>
>旧版OAuth网关配置将继续为现有客户工作。
>
>如果您在旧版OAuth网关配置中遇到问题，请删除现有配置并通过Adobe开发人员控制台创建新配置。


根据AEM版本以及您是首次配置还是升级现有配置，使用Brand Portal配置AEM Assets的步骤有所不同：

| **AEM 版本** | **新配置** | **升级配置** |
|---|---|---|
| **AEM Assets 云服务** | [创建配置](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5（6.5.4.0及更高版本）** | [创建配置](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [升级配置](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4（6.4.8.0及更高版本）** | [创建配置](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [升级配置](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3（6.3.3.8及更高版本）** | [创建配置](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [升级配置](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | 联系支持 | 联系支持 |


