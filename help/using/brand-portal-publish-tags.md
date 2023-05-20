---
title: 将标记发布到 Brand Portal
seo-title: Publish tags to Brand Portal
description: 瞭解如何從Experience Manager Assets發佈標籤至Brand Portal。
seo-description: Learn how to publish tags from Experience Manager Assets to Brand Portal.
uuid: 4167367e-1af8-476b-97a5-730c43bd0816
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: 3c8e9251-195d-4c56-a9a9-27bc8b2a82a4
exl-id: 842656a6-1a2b-4b64-954d-1e663923a1a1
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 4%

---

# 将标记发布到 Brand Portal {#publish-tags-to-brand-portal}

瞭解如何從Experience Manager Assets發佈標籤至Brand Portal。

標籤對於組織資產以及增強與其相關聯之資產的可搜尋性很有用。 標籤可視為附加資產的關鍵字或標籤（中繼資料），並可在搜尋結果中快速找到資產。 若要瞭解如何在Experience Manager Assets中指派標籤至資產，請參閱 [使用標籤來組織資產](https://experienceleague.adobe.com/docs/experience-manager-65/assets/managing/organize-assets.html).

將具有關聯標籤的Assets （和集合）發佈至Brand Portal時，標籤(與AEM中的資產和集合相關聯)會自動發佈至Brand Portal。 已發佈的標籤有助於讓搜尋找到相關資產。

>[!NOTE]
>
>不過，建議先將標籤僅發佈至Brand Portal，再發佈與標籤相關聯的資產（和集合）。 這可確保更快地將資產（和集合）發佈到Brand Portal。

## 管理標籤 {#manage-tags}

您可以使用預先存在的標籤來附加至資產，或從AEM Tags主控台建立新標籤(**[!UICONTROL 工具 |標籤 | AEM標籤]**)。 在這兩種情況下，您必須先將標籤發佈至Brand Portal，然後將其與適當的資產建立關聯。

若要在AEM上建立標籤、在Brand Portal上發佈標籤，並將標籤與適當的資產（或集合）相關聯，請按照以下步驟操作：

1. **建立標籤**
以管理許可權和存取權登入AEM作者執行個體 **[!UICONTROL AEM標籤]** 來自全域導覽的控制檯：

   1. 選取 **[!UICONTROL 工具]**

   1. 選取 **[!UICONTROL 一般]**

   1. 選取 **[!UICONTROL 標籤]**

1. 選取 **[!UICONTROL 建立]** 然後選取 **[!UICONTROL 建立標籤]** 選項。
1. 指定：

   * **[!UICONTROL 标题]**

      *（必要）* 標籤的顯示標題。
   * **[!UICONTROL 名称]**
      *（必要）* 標籤的名稱。 如果未指定，則會從「標題」建立有效的節點名稱。 另請參閱 [標籤ID](https://experienceleague.adobe.com/docs/experience-manager-65/developing/platform/tagging/framework.html).
   * **描述**

      *（選擇性）* 標籤的說明。
   * **標籤路徑**
標籤的JCR路徑。

1. 選取 **[!UICONTROL 提交]** 以建立標籤。

   在AEM例項上建立標籤後，即可將標籤附加至資產（使用該資產的「屬性」區段或「管理標籤」區段）。

1. **將標籤發佈至Brand Portal**.

   前往 **[!UICONTROL AEM標籤]** 主控台([!UICONTROL 工具 |標籤 | AEM標籤])，選取所需的標籤並發佈至Brand Portal。

1. **將標籤附加至資產（或集合）**.

   選取資產（或集合），然後使用該資產的「屬性」區段或「管理標籤」區段附加所需的標籤。 若要進一步瞭解如何在AEM Assets中指派標籤至資產，請參閱 [使用標籤來組織資產](https://experienceleague.adobe.com/docs/experience-manager-65/assets/managing/organize-assets.html).

1. **將資產（或集合）發佈至Brand Portal**.\
   將資產（或集合）發佈至Brand Portal時，附加的標籤也可在Brand Portal上使用。

   若要在Brand Portal中檢視個別資產（或集合）上的附加標籤，請登入Brand Portal並選取資產，在「屬性」區段下方，您會看到附加標籤。

## 搜索提升 {#search-promote}

AEM Assets Brand Portal可讓您將特定資產設為根據關鍵字標籤進行搜尋的排名最前結果。

若要提升搜尋關鍵字的資產，請遵循下列步驟：

1. 開啟 **[!UICONTROL 屬性]** AEM編寫執行個體上的資產頁面。
1. 前往 **[!UICONTROL 進階]** 標籤。
1. 在 **[!UICONTROL 搜尋提升]** 範圍 **[!UICONTROL 提升搜尋關鍵字]** 區段，選取 **[!UICONTROL 新增]** 以新增搜尋關鍵字或標籤。

   ![](assets/search-promote.png)

1. 保存更改。
1. 将资产发布到 Brand Portal.
1. 登入Brand Portal。 檢視 **[!UICONTROL 進階]** 定位於 **[!UICONTROL 屬性]** 區段。
請注意 **[!UICONTROL 搜尋提升]** 關鍵字也會顯示在該資產的屬性中。
