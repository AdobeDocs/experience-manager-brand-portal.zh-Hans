---
title: Brand Portal中的资产来源补充
seo-title: Brand Portal中的资产来源补充
description: 深入了解Adobe Experience Manager资产品牌门户中发布的资产来源补充功能。
seo-description: 深入了解Adobe Experience Manager资产品牌门户中发布的资产来源补充功能。
uuid: null
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
product: experience-manager
sub-product: assets
feature: brand-portal
topics: collaboration, content-velocity, sharing
doc-type: feature-video
activity: use
audience: author, marketer
version: 6.5
kt: 3838
translation-type: tm+mt
source-git-commit: 1aa8892cd51e262ccc16f955655fa644fec230e7

---


# 资产来源补充概述 {#overview-asset-sourcing-in-bp}

**资产来源补充****** (Asset Sourcing)允许AEM用户（管理员／非管理员用户）使用其他“资产贡献”属性创建新文件夹，从而确保创建的新文件夹可由Brand Portal用户打开以提交资产。 这会自动触发一个工作流，该工作流在新创建的 **Contribution** （贡献）文件夹内创建另外两个子文件夹，名 **为** SHARED **（共享）和NEW（新建）** 。 然后，AEM管理员将应添加到贡献文件夹的资产类型以及一组基准资产的简介上传到 **SHARED** 文件夹，以确保BP用户拥有他们需要的参考信息，从而定义了要求。 然后，管理员可以在将新创建的Contribution文件夹发布到Brand Portal之前，向活动的Brand Portal用户授予对贡献文件 **夹的访问权** 。 用户完成在 **NEW** 文件夹中添加内容后，他们可以将贡献文件夹发布回AEM创作环境。 请注意，完成导入并反映AEM资产中新发布的内容可能需要几分钟时间。

此外，所有现有功能都保持不变。 Brand Portal用户可以从贡献文件夹以及其他允许的文件夹查看、搜索和下载资产。 管理员还可以进一步共享贡献文件夹、修改属性以及向集合添加资产。

>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

>[!NOTE]
>
>AEM 6.5.2.0及更高版本支持品牌门户中的资产来源补充。
>
>早期版本（AEM 6.3和AEM 6.4）不支持此功能。
>
>联系Adobe支持部门，将您的AEM实例升级到最新支持的AEM版本。

![Brand Portal资产来源补充](assets/asset-sourcing.png)

## 前提条件 {#prerequisites}

* AEM 6.5.0.2或更高版本。
* 确保您的AEM资产实例已配置Brand Portal。 请参阅， [配置AEM资产与Brand Portal](../using/configure-aem-assets-with-brand-portal.md)。

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
* [将贡献文件夹发布到AEM资产](brand-portal-publish-contribution-folder-to-aem-assets.md)
