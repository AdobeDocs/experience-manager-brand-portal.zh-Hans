---
title: 使用 Brand Portal 配置 AEM Assets
seo-title: 使用 Brand Portal 配置 AEM Assets
description: 了解如何通过Brand Portal配置AEM Assets。
seo-description: 了解如何通过Brand Portal配置AEM Assets。
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
role: Administrator
translation-type: tm+mt
source-git-commit: 6b9433bd5a225a2bbaddc09980c9f7b866a75fe8
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 23%

---


# 使用 Brand Portal 配置 AEM Assets {#configure-integration}

通过Brand Portal配置Adobe Experience Manager资产，可为Brand Portal用户启用资产发布、资产分发和资产贡献功能。 它允许AEM Assets用户与Brand Portal用户一起发布和分发资产。 Brand Portal用户可以通过将新资产上传到资产贡献文件夹并将其发布回AEM Assets，来访问共享资产和贡献。

支持在以下位置配置AEM Assets与Brand Portal:
* AEM Assets as a Cloud Service
* AEM Assets（内部部署和托管服务）6.3及更高版本

通过从云管理器激活Brand Portal，AEM Assets作为Cloud Service自动配置为Brand Portal。 激活工作流在后端创建所需的配置，并将AEM Assets作为Cloud Service实例激活同一IMS组织上的品牌门户。

而AEM Assets（内部部署和托管服务）是使用Adobe Developer Console手动配置Brand Portal的，后者为Brand Portal租户购买Adobe Identity Management Services(IMS)令牌以授权。

>[!NOTE]
>
>***适用于AEM Assets 6.3及更高版本***
>
>以前，Brand Portal是通过旧版OAuth网关在经典界面中配置的，该网关使用JSON Web令牌(JWT)交换获取IMS令牌以进行授权。
>
>从2020年4月6日起，不再支持通过旧版OAuth进行配置，并且已更改为通过Adobe Developer控制台进行配置。


>[!TIP]
>
>***仅适用于现有客户（内部部署和托管服务）***
>
>旧版OAuth网关配置将继续为现有客户工作。
>
>如果您在旧版OAuth网关配置中遇到问题，请删除现有配置，并通过Adobe Developer控制台创建新配置。

配置AEM Assets与Brand Portal的步骤因AEM版本而异，具体取决于您是首次配置还是升级现有配置：

| **AEM 版本** | **新配置** | **升级配置** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [激活Brand Portal](https://docs.adobe.com/content/help/zh-Hans/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5（6.5.4.0及更高版本）** | [创建配置](https://docs.adobe.com/content/help/zh-Hans/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [升级配置](https://docs.adobe.com/content/help/zh-Hans/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4（6.4.8.0及更高版本）** | [创建配置](https://docs.adobe.com/content/help/zh-Hans/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [升级配置](https://docs.adobe.com/content/help/zh-Hans/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3（6.3.3.8及更高版本）** | [创建配置](https://helpx.adobe.com/cn/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [升级配置](https://helpx.adobe.com/cn/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | 联系支持 | 联系支持 |
