---
title: Brand Portal 中的资产源
seo-title: Asset Sourcing in Brand Portal
description: 深入了解Adobe Experience Manager Assets Brand Portal中发布的资产源功能。
seo-description: Get an insight into the asset sourcing feature released in the Adobe Experience Manager Assets Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
sub-product: assets
topics: collaboration, content-velocity, sharing
doc-type: feature-video
activity: use
audience: author, marketer
version: 6.5
kt: 3838
exl-id: 2c132a7a-ed10-4856-8378-67939167ea60
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 1%

---

# 资产源概述 {#overview-asset-sourcing-in-bp}

**资产** 源允许Experience Manager资产用户（管理员/非管理员用户）使用额外的资产贡献属性创建新文 **件** 夹，以确保Brand Portal用户可以打开新文件夹来提交资产。这会自动触发一个工作流，该工作流会在新创建的&#x200B;**Contribution**&#x200B;文件夹中创建另外两个子文件夹，分别称为&#x200B;**SHARED**&#x200B;和&#x200B;**NEW**。 然后，管理员将应添加到贡献文件夹的资产类型以及一组基线资产的简报上传到&#x200B;**SHARED**&#x200B;文件夹，以确保BP用户获得所需的参考信息，从而定义要求。 然后，管理员可以在将新创建的&#x200B;**Contribution**&#x200B;文件夹发布到Brand Portal之前，向活动的Brand Portal用户授予对贡献文件夹的访问权限。 用户完成在&#x200B;**NEW**&#x200B;文件夹中添加内容后，即可将Contribution文件夹发布回Experience Manager创作环境。 请注意，完成导入并反映Experience Manager资产中新发布的内容可能需要几分钟的时间。

此外，所有现有功能都保持不变。 Brand Portal用户可以从贡献文件夹以及其他允许的文件夹查看、搜索和下载资产。 此外，管理员还可以进一步共享贡献文件夹、修改属性并将资产添加到收藏集。

![Brand Portal资产源](assets/asset-sourcing.png)

>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

## 前提条件 {#prerequisites}

* Experience Manager资产作为Cloud Service实例，Experience Manager资产6.5.2或更高版本。
* 确保您的Experience Manager资产实例已配置Brand Portal。 请参阅[使用Brand Portal配置Experience Manager资产](../using/configure-aem-assets-with-brand-portal.md)。

<!--
* Ensure that your Brand Portal tenant is configured with one AEM Assets author instance.
-->

>[!NOTE]
>
>默认情况下，Experience Manager资产会作为Cloud ServiceExperience Manager资产6.5.9及更高版本启用资产源功能。
>
>现有配置将继续在早期版本上工作。

>[!NOTE]
>
>Experience Manager资产6.5.4中存在一个已知问题。在升级到Adobe开发人员控制台时，Brand Portal用户无法将贡献文件夹的资产发布到Experience Manager资产。
>
>此问题已在Experience Manager资产6.5.5中修复。您可以将Experience Manager资产实例升级到最新的Service Pack，并在Adobe开发人员控制台中[升级您的配置](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65)。

<!--

>For immediate fix on AEM 6.5.4, it is recommended to [download the hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) and install on your author instance.
-->

<!--
## Configure Asset Sourcing {#configure-asset-sourcing}

**Asset Sourcing** is configured from within the AEM Assets author instance. The administrators can enable the Asset Sourcing feature flag configuration from the **AEM Web Console Configuration** and upload the active Brand Portal users list in **AEM Assets**.

>[!NOTE]
>
>Asset Sourcing is by default enabled on AEM Assets as a Cloud Service. The AEM administrator can directly upload the active Brand Portal users to allow them access to the Asset Sourcing feature.

>[!NOTE]
>
>Before you begin with the configuration, ensure that your AEM Assets instance is configured with Brand Portal. See, [Configure AEM Assets with Brand Portal](../using/configure-aem-assets-with-brand-portal.md). 

The following video demonstrates, how to configure Asset Sourcing on your AEM Assets author instance:

>[!VIDEO](https://video.tv.adobe.com/v/29771)
-->

<!--
### Enable Asset Sourcing {#enable-asset-sourcing}

AEM administrators can enable the Asset Sourcing feature flag from within the AEM Web Console Configuration (a.k.a Configuration Manager).

>[!NOTE]
>
>This step is not applicable for AEM Assets as a Cloud Service.


**To enable Asset Sourcing:**
1. Log in to your AEM Assets author instance and open Configuration Manager. 
Default URL: http:// localhost:4502/system/console/configMgr.
1. Search using the keyword **Asset Sourcing** to locate **[!UICONTROL Asset Sourcing Feature Flag Config]**.
1. Click **[!UICONTROL Asset Sourcing Feature Flag Config]** to open the configuration window.
1. Select the **[!UICONTROL feature.flag.active.status]** check box.
1. Click **[!UICONTROL Save]**.

![](assets/enable-asset-sourcing.png)
-->


### 上传Brand Portal用户列表 {#upload-bp-user-list}

Experience Manager资产管理员可以上传Brand Portal用户配置(.csv)文件，其中包含Experience Manager资产中的活动Brand Portal用户列表，以便他们能够访问资产源功能。

只能与用户列表中定义的活动Brand Portal用户共享贡献文件夹。 管理员还可以在配置文件中添加新用户，并上传修改后的用户列表。

>[!NOTE]
>
>确保您的Experience Manager资产实例已配置Brand Portal。 请参阅[使用Brand Portal配置Experience Manager资产](../using/configure-aem-assets-with-brand-portal.md)。

>[!NOTE]
>
>CSV文件的格式与批量用户导入Admin Console支持的格式相同。 电子邮件、名字和姓氏是必填项。

管理员可以在Admin Console中添加新用户，有关详细信息，请参阅[管理用户](brand-portal-adding-users.md) 。 在Admin Console中添加用户后，可以将这些用户添加到Brand Portal用户配置文件，然后为其分配访问贡献文件夹的权限。

**要上传Brand Portal用户列表，请执行以下操作：**

1. 登录到Experience Manager资产实例。
1. 从&#x200B;**工具**&#x200B;面板中，导航到&#x200B;**[!UICONTROL Assets]** > **[!UICONTROL Brand Portal用户]**。

1. Brand Portal上传参与者窗口将打开。
从本地计算机中浏览并上载**配置(.csv)文件**(包含活动的Brand Portal用户列表)。
1. 单击&#x200B;**[!UICONTROL 保存]**。

   ![](assets/upload-user-list2.png)


管理员在配置贡献文件夹时，可以从此用户列表访问特定用户。 只有分配到贡献文件夹的用户才有权访问贡献文件夹，并将资产从Brand Portal发布到Experience Manager资产。

## 另请参阅 {#reference-articles}

* [配置贡献文件夹并将其发布到Brand Portal](brand-portal-publish-contribution-folder-to-brand-portal.md)

* [将贡献文件夹发布到Experience Manager资产](brand-portal-publish-contribution-folder-to-aem-assets.md)
