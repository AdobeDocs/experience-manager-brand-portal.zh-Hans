---
title: 使用 Brand Portal 配置 AEM Assets
seo-title: 使用 Brand Portal 配置 AEM Assets
description: 深入了解如何使用Brand Portal配置AEM Assets。
seo-description: 深入了解如何使用Brand Portal配置AEM Assets。
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: ba8a1f09573766643f6a5013a8d181f0f0dbb4f2
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 10%

---


# 使用 Brand Portal 配置 AEM Assets {#configure-integration}

Adobe Experience Manager(AEM)资产通过Adobe开发人员控制台配置为品牌门户，该控制台为您的品牌门户租户购买IMS令牌以进行授权。 AEM Assets云服务、AEM Assets6.3及更高版本现在支持Brand Portal。

通过配置AEM Assets可以通过Brand Portal提供服务，您可以发布资产并将其分发给Brand Portal用户。 然而，在AEM 6.3（及更高版本）上配置Brand Portal可为Brand Portal用户启用资产发布、资产分发和资产贡献功能。

>[!NOTE]
>
>***适用于AEM Assets6.3及更高版本***
>
>以前，品牌门户通过旧版OAuth网关在经典UI中配置，该网关使用JWT令牌交换获得IMS访问令牌进行授权。
>
>从2020年4月6日起，不再支持通过旧版OAuth进行配置，并且已更改为通过Adobe开发人员控制台进行配置。


>[!TIP]
>
>***仅限现有客户***
>
>旧版OAuth网关配置将继续为现有客户工作。
>
>如果您在旧版OAuth网关配置中遇到问题，请删除现有配置并通过Adobe开发人员控制台创建新配置。


使用Brand Portal配置AEM Assets的步骤因AEM版本、您是首次配置还是升级现有配置而异：

| **AEM 版本** | **新配置** | **升级配置** |
|---|---|---|
| **AEM Assets 云服务** | [创建配置](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5（6.5.4.0及更高版本）** | [创建配置](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [升级配置](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4（6.4.8.0及更高版本）** | [创建配置](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [升级配置](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3（6.3.3.8及更高版本）** | [创建配置](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [升级配置](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | 联系支持 | 联系支持 |


