---
title: Brand Portal 中的资产源
seo-title: Asset Sourcing in Brand Portal
description: 深入了解在Adobe Experience Manager Assets Brand Portal中发布的资源获取功能。
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
source-wordcount: '647'
ht-degree: 1%

---

# 资产来源补充概览 {#overview-asset-sourcing-in-bp}

**Asset Sourcing**&#x200B;允许Experience Manager Assets用户（管理员/非管理员用户）使用额外的&#x200B;**Asset Contribution**&#x200B;属性创建新文件夹，确保所创建的新文件夹可供Brand Portal用户提交资源。 这会自动触发一个工作流，该工作流在新创建的&#x200B;**Contribution**&#x200B;文件夹中创建两个名为&#x200B;**SHARED**&#x200B;和&#x200B;**NEW**&#x200B;的子文件夹。 然后，管理员通过向&#x200B;**SHARED**&#x200B;文件夹上载有关应添加到贡献文件夹的资源类型的简短说明以及一组基线资源来定义需求，以确保BP用户拥有他们所需的参考信息。 随后，管理员可以向活动Brand Portal用户授予对贡献文件夹的访问权限，然后再将新创建的&#x200B;**贡献**&#x200B;文件夹发布到Brand Portal。 用户完成在&#x200B;**NEW**&#x200B;文件夹中添加内容后，即可将贡献文件夹发布回Experience Manager创作环境。 请注意，可能需要几分钟才能完成导入，并在Experience Manager Assets中反映新发布的内容。

此外，所有现有功能均保持不变。 Brand Portal用户可以从“贡献”文件夹以及其他允许的文件夹中查看、搜索和下载资源。 管理员可以进一步共享贡献文件夹、修改属性并将资源添加到收藏集。

![Brand Portal资源源](assets/asset-sourcing.png)

>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

## 先决条件 {#prerequisites}

* Experience Manager Assetsas a Cloud Service实例，Experience Manager Assets 6.5.2或更高版本。
* 确保已使用Brand Portal配置您的Experience Manager Assets实例。 请参阅[使用Brand Portal配置Experience Manager Assets](../using/configure-aem-assets-with-brand-portal.md)。

<!--
* Ensure that your Brand Portal tenant is configured with one AEM Assets author instance.
-->

>[!NOTE]
>
>默认情况下，Experience Manager Assets as a Cloud Service、Experience Manager Assets 6.5.9及更高版本上启用了“资源源”功能。
>
>现有配置将继续在早期版本上运行。

>[!NOTE]
>
>Experience Manager Assets 6.5.4中存在已知问题。升级到Adobe Developer Console时，Brand Portal用户无法将contribution文件夹中的资产发布到Experience Manager Assets。
>
>已在Experience Manager Assets 6.5.5中修复此问题。您可以在Adobe Developer Console上将Experience Manager Assets实例升级到最新的Service Pack并[升级配置](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65)。

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

Experience Manager Assets管理员可以上传包含Experience Manager Assets中的活动Brand Portal用户列表的Brand Portal用户配置(.csv)文件，以允许他们访问资源源功能。

贡献文件夹只能与在用户列表中定义的活动Brand Portal用户共享。 管理员还可以在配置文件中添加新用户并上传修改的用户列表。

>[!NOTE]
>
>确保已使用Brand Portal配置您的Experience Manager Assets实例。 请参阅[使用Brand Portal配置Experience Manager Assets](../using/configure-aem-assets-with-brand-portal.md)。

>[!NOTE]
>
>CSV文件的格式与Admin Console中支持批量用户导入的格式相同。 电子邮件、名字和姓氏是必填项。

管理员可以在Admin Console中添加新用户，有关详细信息，请参阅[管理用户](brand-portal-adding-users.md)。 在Admin Console中添加用户后，可以将这些用户添加到Brand Portal用户配置文件，然后为其分配访问贡献文件夹的权限。

**要上传Brand Portal用户列表：**

1. 登录到您的Experience Manager Assets实例。
1. 从&#x200B;**工具**&#x200B;面板中，导航到&#x200B;**[!UICONTROL Assets]** > **[!UICONTROL Brand Portal用户]**。

1. 将打开Brand Portal上传参与者窗口。
从本地计算机中浏览并上传包含活动Brand Portal用户列表的**配置(.csv)文件**。
1. 单击&#x200B;**[!UICONTROL 保存]**。

   ![](assets/upload-user-list2.png)


在配置贡献文件夹时，管理员可以通过此用户列表向特定用户提供访问权限。 只有分配到贡献文件夹的用户才有权访问贡献文件夹，并可以将资源从Brand Portal发布到Experience Manager Assets。

## 另请参阅 {#reference-articles}

* [配置贡献文件夹并将其发布到Brand Portal](brand-portal-publish-contribution-folder-to-brand-portal.md)

* [Publish贡献文件夹到Experience Manager Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)
