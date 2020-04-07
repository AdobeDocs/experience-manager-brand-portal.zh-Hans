---
title: 使用Brand Portal配置AEM资产
seo-title: 使用Brand Portal配置AEM资产
description: 了解如何通过Brand Portal配置AEM资产。
seo-description: 了解如何通过Brand Portal配置AEM资产。
uuid: null
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 6b03229b72a1912be57c2bc1b7e47a017d3dca7e

---


# 使用Brand Portal配置AEM资产 {#configure-integration}

Adobe Experience Manager(AEM)资产通过Adobe I/O配置了Brand Portal,Adobe I/O可获取IMS令牌以授权您的Brand Portal租户。 该配置为Brand Portal用户启用了资产发布、资产分发和资产贡献功能。

>[!NOTE]
>
>以前，Brand Portal是通过旧版OAuth网关在经典UI中配置的，该网关使用JWT令牌交换获得IMS访问令牌进行授权。
>
>从2020年4月6日起，不再支持通过旧版OAuth进行配置，并已更改为通过Adobe I/O进行配置。


>[!TIP]
>
>***仅适用于现有客户***
>
>建议继续使用现有的传统OAuth网关配置。 如果您遇到旧版OAuth网关配置问题，请删除现有配置并通过Adobe I/O创建新配置。


根据您的AEM版本以及您是首次配置还是升级现有配置，配置带有Brand Portal的AEM资产的步骤有所不同：

| **AEM 版本** | **新配置** | **升级配置** |
|---|---|---|
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