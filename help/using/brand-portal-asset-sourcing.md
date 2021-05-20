---
title: Brand Portal 中的资产源
seo-title: Brand Portal 中的资产源
description: 深入了解Adobe Experience Manager Assets Brand Portal中发布的资产源功能。
seo-description: 深入了解Adobe Experience Manager Assets Brand Portal中发布的资产源功能。
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
sub-product: 资产
topics: collaboration, content-velocity, sharing
doc-type: feature-video
activity: use
audience: author, marketer
version: 6.5
kt: 3838
exl-id: 2c132a7a-ed10-4856-8378-67939167ea60
source-git-commit: e8bb1149582329f5304bda7e5e67e8dcc27cfc7b
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 4%

---

# 资产源概述{#overview-asset-sourcing-in-bp}

**资产** 源允许AEM用户（管理员/非管理员用户）使用额外的资产贡献属性创建新文 **件** 夹，以确保Brand Portal用户能够打开所创建的新文件夹来提交资产。这会自动触发一个工作流，该工作流会在新创建的&#x200B;**Contribution**&#x200B;文件夹中创建另外两个子文件夹，分别称为&#x200B;**SHARED**&#x200B;和&#x200B;**NEW**。 然后，AEM管理员将应添加到贡献文件夹的资产类型以及一组基线资产的简介上传到&#x200B;**SHARED**&#x200B;文件夹，以确保BP用户获得所需的参考信息，从而定义此要求。 然后，管理员可以在将新创建的&#x200B;**Contribution**&#x200B;文件夹发布到Brand Portal之前，向活动的Brand Portal用户授予对贡献文件夹的访问权限。 用户完成在&#x200B;**NEW**&#x200B;文件夹中添加内容后，便可以将Contribution文件夹发布回AEM创作环境。 请注意，完成导入并反映AEM Assets中新发布的内容可能需要几分钟的时间。

此外，所有现有功能都保持不变。 Brand Portal用户可以从贡献文件夹以及其他允许的文件夹查看、搜索和下载资产。 此外，管理员还可以进一步共享贡献文件夹、修改属性并将资产添加到收藏集。

## 前提条件 {#prerequisites}

* AEM Assets作为Cloud Service实例，AEM Assets 6.5.2或更高版本。
* 确保您的AEM Assets实例已配置Brand Portal。 请参阅[使用Brand Portal配置AEM Assets](../using/configure-aem-assets-with-brand-portal.md)。
* 确保为Brand Portal租户配置了一个AEM Assets创作实例。

>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

![Brand Portal资产源](assets/asset-sourcing.png)


>[!NOTE]
>
>AEM Assets 6.5.4中存在一个已知问题。在升级到Adobe开发人员控制台时，Brand Portal用户无法将贡献文件夹的资产发布到AEM Assets。
>
>此问题已在AEM 6.5.5中修复。您可以将AEM Assets实例升级到最新的Service Pack AEM 6.5.5，并在Adobe开发人员控制台上[升级您的配置。](https://docs.adobe.com/content/help/zh-Hans/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65)
>
>要在AEM 6.5.4上立即修复，建议[下载修补程序](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041)并在创作实例上安装。

## 配置资产源{#configure-asset-sourcing}

**资产** 源是从AEM Assets创作实例中配置的。管理员可以从&#x200B;**AEM Web控制台配置**&#x200B;中启用资产源功能标志配置，并在&#x200B;**AEM Assets**&#x200B;中上传活动的Brand Portal用户列表。

>[!NOTE]
>
>默认情况下，AEM Assets as a Cloud Service上会启用“资产源”。 AEM管理员可以直接上传活动的Brand Portal用户，以便他们访问资产源功能。

>[!NOTE]
>
>在开始配置之前，请确保已使用AEM Assets配置了Brand Portal实例。 请参阅[使用Brand Portal配置AEM Assets](../using/configure-aem-assets-with-brand-portal.md)。

以下视频演示了如何在AEM Assets创作实例上配置资产源：

>[!VIDEO](https://video.tv.adobe.com/v/29771)

### 启用资产源{#enable-asset-sourcing}

AEM管理员可以从AEM Web控制台配置（即配置管理器）中启用资产源功能标记。

>[!NOTE]
>
>此步骤不适用于AEM Assets作为Cloud Service。


**要启用资产来源补充，请执行以下操作：**
1. 登录到AEM Assets创作实例，然后打开配置管理器。
默认URL:http:// localhost:4502/system/console/configMgr。
1. 使用关键字&#x200B;**资产源**&#x200B;进行搜索，以找到&#x200B;**[!UICONTROL 资产源功能标志配置]**。
1. 单击&#x200B;**[!UICONTROL 资产源功能标志配置]**&#x200B;以打开配置窗口。
1. 选中&#x200B;**[!UICONTROL feature.flag.active.status]**&#x200B;复选框。
1. 单击&#x200B;**[!UICONTROL 保存]**。

![](assets/enable-asset-sourcing.png)

### 上载Brand Portal用户列表{#upload-bp-user-list}

AEM管理员可以在AEM Assets中上传包含活动Brand Portal用户列表的Brand Portal用户配置(.csv)文件。 只能与用户列表中定义的活动Brand Portal用户共享贡献文件夹。 管理员还可以在配置文件中添加新用户，并上传修改后的用户列表。

>[!NOTE]
>
>CSV文件的格式与批量用户导入Admin Console支持的格式相同。 电子邮件、名字和姓氏是必填项。

管理员可以在AEMAdmin Console中添加新用户，有关详细信息，请参阅[管理用户](brand-portal-adding-users.md) 。 在Admin Console中添加用户后，可以将这些用户添加到Brand Portal用户配置文件，然后为其分配访问贡献文件夹的权限。

**要上传Brand Portal用户列表，请执行以下操作：**
1. 登录到AEM Assets实例。
1. 从&#x200B;**工具**&#x200B;面板中，导航到&#x200B;**[!UICONTROL Assets]** > **[!UICONTROL Brand Portal用户]**。

1. Brand Portal上传参与者窗口将打开。
从本地计算机中浏览并上载**配置(.csv)文件**(包含活动的Brand Portal用户列表)。
1. 单击&#x200B;**[!UICONTROL 保存]**。

   ![](assets/upload-user-list2.png)


管理员在配置贡献文件夹时，可以从此用户列表访问特定用户。 只有分配到贡献文件夹的用户才有权访问贡献文件夹，并将资产从Brand Portal发布到AEM Assets。

## 另请参阅 {#reference-articles}

* [配置贡献文件夹并将其发布到Brand Portal](brand-portal-publish-contribution-folder-to-brand-portal.md)

* [将贡献文件夹发布到AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)
