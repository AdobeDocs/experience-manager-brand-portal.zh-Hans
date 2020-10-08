---
title: 品牌门户中的资产来源补充
seo-title: 品牌门户中的资产来源补充
description: 深入了解Adobe Experience Manager资产品牌门户中发布的资产来源补充功能。
seo-description: 深入了解Adobe Experience Manager资产品牌门户中发布的资产来源补充功能。
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
product: experience-manager
sub-product: 资产
feature: brand-portal
topics: collaboration, content-velocity, sharing
doc-type: feature-video
activity: use
audience: author, marketer
version: 6.5
kt: 3838
translation-type: tm+mt
source-git-commit: ecd53a7d92dd020e6a3527793ff11efadcb531ee
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 0%

---


# 资产来源补充概述 {#overview-asset-sourcing-in-bp}

**资产来源** -AEM用户（管理员／非管理员用户）可以使用其他“资产贡献”属性创建新文 **件夹** ，从而确保创建的新文件夹可以由Brand Portal用户通过资产提交方式打开。 这会自动触发一个工作流，该工作流会在新创建的Contribution **文件夹内** ，创建另外两个名 **为** SHARED和NEW **** 的子文件夹。 AEM管理员随后会定义此要求，方法是将应添加到贡献文件夹的资产类型以及一组基准资产的简报上传到 **SHARED** 文件夹，以确保BP用户获得所需的参考信息。 然后，管理员可以在将新创建的Contribution文件夹发布到Brand Portal之前，向活动的Brand Portal用户授 **予对** 贡献文件夹的访问权限。 用户在NEW文件夹中添加完内 **容后** ，即可将贡献文件夹发布回AEM作者环境。 请注意，完成导入并反映AEM Assets内新发布的内容可能需要几分钟时间。

此外，所有现有功能都保持不变。 Brand Portal用户可以从贡献文件夹以及其他允许的文件夹中视图、搜索和下载资产。 此外，管理员还可以进一步共享贡献文件夹、修改属性以及向收藏集添加资产。

## 前提条件 {#prerequisites}

* AEM 6.5.2或更高版本。
* 确保您的AEM Assets实例已配置Brand Portal。 See, [Configure AEM Assets with Brand Portal](../using/configure-aem-assets-with-brand-portal.md).
* 确保您的Brand Portal租户配置了一个AEM Assets作者实例。

>[!NOTE]
>
>AEM Assets作为Cloud Service不支持资产来源补充。

>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

![品牌门户资产来源补充](assets/asset-sourcing.png)


>[!NOTE]
>
>AEM 6.5.4中存在已知问题。在升级到Adobe开发人员控制台时，Brand Portal用户无法将贡献文件夹的资产发布到AEM Assets。
>
>此问题在AEM 6.5.5中已解决。您可以将AEM Assets实例升级到最新的服务包AEM 6.5.5，并在Adobe开发 [人员控制台上](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) 升级您的配置。
>
>要立即修复AEM 6.5.4，建议下载 [修补程序](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) ，并在创作实例上安装。

## 另请参阅 {#reference-articles}

**适用于管理员**

* [在AEM中配置资产来源补充](brand-portal-configure-asset-sourcing.md)
* [上传Brand Portal用户列表](brand-portal-configure-asset-sourcing.md)
* [配置贡献文件夹](brand-portal-contribution-folder.md)
* [将基准资产上传到贡献文件夹](brand-portal-upload-baseline-assets.md)
* [将贡献文件夹发布到Brand Portal](brand-portal-publish-contribution-folder-to-brand-portal.md)

**对于Brand Portal用户**

* [下载资产要求](brand-portal-download-asset-requirements.md)
* [将新资产上传到贡献文件夹](brand-portal-upload-assets-to-contribution-folder.md)
* [将贡献文件夹发布到AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)
