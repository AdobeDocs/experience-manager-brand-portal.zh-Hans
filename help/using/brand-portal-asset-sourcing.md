---
title: Brand Portal 中的资产源
seo-title: Asset Sourcing in Brand Portal
description: 深入瞭解Adobe Experience Manager Assets Brand Portal中發行的資產來源功能。
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

# 資產來源概觀 {#overview-asset-sourcing-in-bp}

**資產來源** 可讓Experience Manager Assets使用者（管理員/非管理員使用者）使用額外的 **資產貢獻** 屬性，確保Brand Portal使用者可提交所建立的新資料夾。 這會自動觸發建立兩個額外子資料夾的工作流程，稱為 **已共用** 和 **新增**，在新建立的 **貢獻** 資料夾。 然後，管理員透過上傳應新增到貢獻資料夾的資產型別的簡短資訊以及一組基線資產來定義需求 **已共用** 資料夾，以確保BP使用者擁有他們所需的參考資訊。 之後，管理員便可在發佈新建立的貢獻資料夾之前，授予作用中Brand Portal使用者對貢獻資料夾的存取權 **貢獻** 資料夾移至Brand Portal。 一旦使用者完成在中新增內容 **新增** 資料夾中，他們可以將「貢獻」資料夾發佈回Experience Manager作者環境。 請注意，可能需要幾分鐘的時間來完成匯入，並反映Experience Manager Assets中新發佈的內容。

此外，所有現有功能均維持不變。 Brand Portal使用者可以從貢獻資料夾以及其他允許的資料夾中檢視、搜尋和下載資產。 管理員可以進一步共用貢獻資料夾、修改屬性，以及將資產新增至收藏集。

![Brand Portal資產來源](assets/asset-sourcing.png)

>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

## 前提条件 {#prerequisites}

* Experience Manager Assetsas a Cloud Service執行個體、Experience Manager Assets 6.5.2或更高版本。
* 確保您的Experience Manager Assets執行個體已使用Brand Portal進行設定。 請參閱， [使用Brand Portal設定Experience Manager Assets](../using/configure-aem-assets-with-brand-portal.md).

<!--
* Ensure that your Brand Portal tenant is configured with one AEM Assets author instance.
-->

>[!NOTE]
>
>Experience Manager Assetsas a Cloud Service、Experience Manager Assets 6.5.9及更高版本預設會啟用「資產來源」功能。
>
>現有設定將繼續在舊版上運作。

>[!NOTE]
>
>Experience Manager Assets 6.5.4有一個已知問題。Brand Portal使用者升級至Experience Manager Assets主控台後，無法將貢獻資料夾的資產發佈至Adobe Developer。
>
>Experience Manager Assets 6.5.5已修正此問題。您可以將Experience Manager Assets執行個體升級至最新的Service Pack，並且 [升級您的設定](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) 在Adobe Developer Console上。

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


### 上傳Brand Portal使用者清單 {#upload-bp-user-list}

Experience Manager Assets管理員可以上傳包含Experience Manager Assets中有效Brand Portal使用者清單的Brand Portal使用者設定(.csv)檔案，以允許他們存取Asset Sourcing功能。

貢獻資料夾只能與使用者清單中定義的作用中Brand Portal使用者共用。 管理員也可以在設定檔案中新增使用者，並上傳修改過的使用者清單。

>[!NOTE]
>
>確保您的Experience Manager Assets執行個體已使用Brand Portal進行設定。 請參閱， [使用Brand Portal設定Experience Manager Assets](../using/configure-aem-assets-with-brand-portal.md).

>[!NOTE]
>
>CSV檔案的格式與Admin Console支援的大量使用者匯入格式相同。 電子郵件、名字和姓氏為必填欄位。

管理員可以在Admin Console中新增使用者，請參閱 [管理使用者](brand-portal-adding-users.md) 詳細資訊。 在Admin Console中新增使用者後，這些使用者可以新增到Brand Portal使用者設定檔，然後指派許可權以存取貢獻資料夾。

**若要上傳Brand Portal使用者清單：**

1. 登入您的Experience Manager Assets執行個體。
1. 從 **工具**  面板，導覽至 **[!UICONTROL 資產]** > **[!UICONTROL Brand Portal使用者]**.

1. Brand Portal上傳貢獻者視窗隨即開啟。
從本機電腦瀏覽並上傳 **設定(.csv)檔案** 包含作用中Brand Portal使用者清單。
1. 单击“**[!UICONTROL 保存]**”。

   ![](assets/upload-user-list2.png)


管理員可在設定貢獻資料夾時，從此使用者清單提供特定使用者的存取權。 只有指派給貢獻資料夾的使用者才能存取貢獻資料夾，並從Brand Portal將資產發佈到Experience Manager Assets。

## 另请参阅 {#reference-articles}

* [設定貢獻資料夾並發佈至Brand Portal](brand-portal-publish-contribution-folder-to-brand-portal.md)

* [將貢獻資料夾發佈至Experience Manager Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)
