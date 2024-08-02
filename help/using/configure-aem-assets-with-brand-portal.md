---
title: 使用 Brand Portal 配置 Experience Manager Assets
description: 深入了解如何使用Brand Portal配置Experience Manager Assets。
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
role: Admin
exl-id: 261c0e84-6b3d-459c-b6b9-a9af106d6943
source-git-commit: 32a67abf466dd3bf635b851b02377ed23591915e
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 6%

---

# 使用 Brand Portal 配置 Experience Manager Assets {#configure-integration}

使用Brand Portal配置Adobe Experience Manager Assets可为Brand Portal用户启用资产发布、资产分配和资产贡献功能。 它允许Experience Manager Assets用户与Brand Portal用户一起发布和分发资源。 Brand Portal用户可以访问共享资源并通过将新资源上传到资源贡献文件夹并将其发布回Experience Manager Assets来贡献资源。

支持使用Brand Portal配置Experience Manager Assets：

* Experience Manager Assetsas a Cloud Service
* Experience Manager Assets（内部部署和托管服务）6.5及更高版本

通过从Cloud Manager激活Experience Manager Assets，可使用Brand Portal自动配置Brand Portalas a Cloud Service。 激活工作流会在后端创建所需的配置，并在与Experience Manager Assetsas a Cloud Service实例相同的IMS组织上激活Brand Portal。

而使用Brand Portal手动配置Experience Manager Assets（内部部署和托管服务）的Adobe Developer Console，这会获取Adobe的Identity Management Services (IMS)令牌以授权Brand Portal租户。

>[!NOTE]
>
>适用于Experience Manager Assets 6.5及更高版本的&#x200B;******
>
>以前，经典界面使用旧版OAuth网关配置Brand Portal，该网关使用JSON Web令牌(JWT)交换获取IMS令牌进行授权。
>
>从2020年4月6日起，不再支持通过旧版OAuth进行配置，而是更改为通过Adobe Developer Console进行配置。


>[!TIP]
>
>***仅针对现有客户（内部部署和托管服务）***
>
>旧版OAuth网关配置将继续适用于现有客户。
>
>如果您遇到旧版OAuth网关配置问题，请删除现有配置，并通过Adobe Developer Console创建新配置。

使用Brand Portal配置AEM Assets的步骤因您的AEM版本，以及您是首次配置还是升级现有配置而异：

| **AEM版本** | **新配置** | **升级配置** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [激活Brand Portal](https://experienceleague.adobe.com/zh-hans/docs/experience-manager-cloud-service/content/assets/brand-portal/configure-aem-assets-with-brand-portal) | - |
| **AEM 6.5 （6.5.4.0及更高版本）** | [创建配置](https://experienceleague.adobe.com/zh-hans/docs/experience-manager-65/content/assets/brandportal/configure-aem-assets-with-brand-portal) | [升级配置](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/brandportal/configure-aem-assets-with-brand-portal#upgrade-integration-65) |
