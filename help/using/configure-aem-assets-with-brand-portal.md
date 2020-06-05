---
title: 使用 Brand Portal 配置 AEM Assets
seo-title: 使用 Brand Portal 配置 AEM Assets
description: 深入了解如何通过Brand Portal配置AEM资产。
seo-description: 深入了解如何通过Brand Portal配置AEM资产。
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 0278d17cc774338b456d9c3881953f2e34ca7126
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 10%

---


# 使用 Brand Portal 配置 AEM Assets {#configure-integration}

Adobe Experience Manager(AEM)资产通过Adobe开发人员控制台配置为品牌门户，该控制台为品牌门户租户购买IMS令牌以进行授权。 AEM Assets云服务、AEM Assets 6.3及更高版本现在支持Brand Portal。

通过配置AEM资产可以通过Brand Portal提供服务，您可以通过Brand Portal用户发布和分发资产。 然而，在AEM 6.3（及更高版本）上配置Brand Portal可为Brand Portal用户启用资产发布、资产分发和资产贡献功能。

>[!NOTE]
>
>***对于AEM Assets 6.3及更高版本***
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


根据您的AEM版本以及您是首次配置还是升级现有配置，使用Brand Portal配置AEM资产的步骤会有所不同：

| **AEM 版本** | **新配置** | **升级配置** |
|---|---|---|
| **AEM Assets 云服务** | [创建配置](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5（6.5.4.0及更高版本）** | [创建配置](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [升级配置](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4（6.4.8.0及更高版本）** | [创建配置](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [升级配置](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3（6.3.3.8及更高版本）** | [创建配置](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [升级配置](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | 联系支持 | 联系支持 |


<!--
   Comment Type: draft

   <li> </li>
   -->

<!--
   Comment Type: draft

   <li>Step text</li>
   -->
