---
title: Brand Portal 中的资产源
seo-title: Brand Portal 中的资产源
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
topics: collaboration, content-velocity, sharing
doc-type: feature-video
activity: use
audience: author, marketer
version: 6.5
kt: 3838
translation-type: tm+mt
source-git-commit: 263653916e4bc183827c197c3beb137c9e59ccb1
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 4%

---


# 资产来源补充概述{#overview-asset-sourcing-in-bp}

**资产** 源允许AEM用户（管理员/非管理员用户）使用其他Asset Contribution属性创建新 **文** 件夹，从而确保创建的新文件夹可由Brand Portal用户打开并提交资产。这会自动触发一个工作流，该工作流会在新创建的&#x200B;**Contribution**&#x200B;文件夹中创建另外两个子文件夹，名为&#x200B;**SHARED**&#x200B;和&#x200B;**NEW**。 然后，AEM管理员将应添加到贡献文件夹的资产类型以及一组基准资产的简报上传到&#x200B;**SHARED**&#x200B;文件夹，以确保BP用户获得所需的参考信息，从而定义要求。 然后，管理员可以在将新创建的&#x200B;**Contribution**&#x200B;文件夹发布到Brand Portal之前，向活动的Brand Portal用户授予对贡献文件夹的访问权限。 用户在&#x200B;**NEW**&#x200B;文件夹中添加完内容后，可以将贡献文件夹发布回AEM作者环境。 请注意，完成导入并反映AEM Assets中新发布的内容可能需要几分钟时间。

此外，所有现有功能都保持不变。 Brand Portal用户可以从贡献文件夹以及其他允许的文件夹中视图、搜索和下载资产。 此外，管理员还可以进一步共享贡献文件夹、修改属性以及向收藏集添加资产。

## 前提条件 {#prerequisites}

* AEM Assets作为Cloud Service实例，AEM Assets 6.5.2或更高版本。
* 确保您的AEM Assets实例已配置Brand Portal。 请参阅[配置AEM Assets与Brand Portal](../using/configure-aem-assets-with-brand-portal.md)。
* 确保您的Brand Portal租户已配置一个AEM Assets作者实例。

>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

![品牌门户资产来源](assets/asset-sourcing.png)


>[!NOTE]
>
>AEM Assets 6.5.4中存在已知问题。在升级到Adobe开发人员控制台时，Brand Portal用户无法将贡献文件夹的资产发布到AEM Assets。
>
>此问题在AEM 6.5.5中已解决。您可以将AEM Assets实例升级到最新的Service Pack AEM 6.5.5和[升级Adobe开发人员控制台上的配置](https://docs.adobe.com/content/help/zh-Hans/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65)。
>
>对于AEM 6.5.4上的即时修复，建议[下载修补程序](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041)并安装在创作实例上。

## 配置资产来源补充{#configure-asset-sourcing}

**资产** 源是从AEM Assets作者实例中配置的。管理员可以从&#x200B;**AEM Web Console配置**&#x200B;中启用资产来源补充功能标志配置，并上传&#x200B;**AEM Assets**&#x200B;中的活动Brand Portal用户列表。

>[!NOTE]
>
>默认情况下，AEM Assets会将资产来源补充作为Cloud Service启用。 AEM管理员可以直接上传活动的Brand Portal用户，以允许他们访问资产来源补充功能。

>[!NOTE]
>
>在开始配置之前，请确保AEM Assets实例已配置Brand Portal。 请参阅[配置AEM Assets与Brand Portal](../using/configure-aem-assets-with-brand-portal.md)。

以下视频演示了如何在AEM Assets作者实例上配置资产来源补充：

>[!VIDEO](https://video.tv.adobe.com/v/29771)

### 启用资产来源补充{#enable-asset-sourcing}

AEM管理员可以从AEM Web控制台配置（即配置管理器）中启用资产来源补充功能标志。

>[!NOTE]
>
>此步骤不适用于AEM Assets作为Cloud Service。


**要启用资产来源补充，请执行以下操作：**
1. 登录到AEM Assets作者实例，然后打开Configuration Manager。
默认URL:http:// localhost:4502/system/console/configMgr。
1. 使用关键字&#x200B;**资产来源补充**&#x200B;进行搜索以找到&#x200B;**[!UICONTROL 资产来源补充功能标志配置]**。
1. 单击&#x200B;**[!UICONTROL 资产来源补充功能标志配置]**&#x200B;以打开配置窗口。
1. 选中&#x200B;**[!UICONTROL feature.flag.active.status]**&#x200B;复选框。
1. 单击&#x200B;**[!UICONTROL 保存]**。

![](assets/enable-asset-sourcing.png)

### 上传Brand Portal用户列表{#upload-bp-user-list}

AEM管理员可以上传包含AEM Assets中活动Brand Portal用户列表的Brand Portal用户配置(.csv)文件。 贡献文件夹只能与在用户列表中定义的活动Brand Portal用户共享。 管理员还可以在配置文件中添加新用户并上传修改后的用户列表。

>[!NOTE]
>
>CSV文件的格式与批量用户导入Admin Console中支持的格式相同。 电子邮件、名和姓是必填项。

管理员可以在AEMAdmin Console中添加新用户，有关详细信息，请参阅[管理用户](brand-portal-adding-users.md)。 在Admin Console中添加用户后，可以将这些用户添加到Brand Portal用户配置文件，然后为其分配访问贡献文件夹的权限。

**要上传Brand Portal用户列表:**
1. 登录到AEM Assets实例。
1. 从&#x200B;**工具**&#x200B;面板，导航到&#x200B;**[!UICONTROL 资产]** > **[!UICONTROL 品牌门户用户]**。

1. 将打开“品牌门户上传参与者”窗口。
从您的本地计算机浏览并上传包含活动Brand Portal用户列表的**配置(.csv)文件**。
1. 单击&#x200B;**[!UICONTROL 保存]**。

   ![](assets/upload-user-list2.png)


管理员可以在配置贡献文件夹时通过此用户列表向特定用户提供访问权限。 只有分配到贡献文件夹的用户才有权访问贡献文件夹并将资产从Brand Portal发布到AEM Assets。

## 另请参阅 {#reference-articles}

* [配置贡献文件夹并将其发布到Brand Portal](brand-portal-publish-contribution-folder-to-brand-portal.md)

* [将贡献文件夹发布到AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)
