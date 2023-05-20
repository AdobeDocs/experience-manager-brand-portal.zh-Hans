---
title: 将预设、架构和 Facet 发布到 Brand Portal
seo-title: Publish presets, schema, and facets to Brand Portal
description: 瞭解如何將預設集、結構和Facet發佈到Brand Portal。
seo-description: Learn how to publish presets, schema, and facets to Brand Portal.
uuid: c836d9bb-074a-4113-9c91-b2bf7658b88d
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: bc305abc-9373-4d33-9179-0a5f3904b352
exl-id: 9b585606-6538-459b-87a9-2e68df0087b3
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '1141'
ht-degree: 2%

---

# 将预设、架构和 Facet 发布到 Brand Portal {#publish-presets-schema-and-facets-to-brand-portal}

本文深入探討如何從AEM製作例項將影像預設集、中繼資料結構描述和自訂搜尋Facet發佈至Brand Portal。 發佈功能可讓組織重複使用在AEM Author例項中建立/修改的影像預設集、中繼資料結構描述和搜尋Facet，藉此減少重複工作。

>[!NOTE]
>
>從AEM 6.2 SP1-CFP7和AEM 6.3 SP 1-CFP 1 (6.3.1.1)起，您可以將影像預設集、中繼資料結構描述和搜尋Facet從AEM製作例項發佈至Brand Portal。

## 將影像預設集發佈至Brand Portal {#publish-image-presets-to-brand-portal}

影像預設集是在影像傳送時套用至影像的一組大小調整和格式命令。 影像預設集可在Brand Portal中建立和修改。 或者，如果AEM Author例項以Dynamic Media模式執行，則使用者可以在AEM Author中建立預設集並發佈至AEM Assets Brand Portal，並避免在Brand Portal中重新建立相同的預設集。\
預設集建立後，會在資產詳細資料轉譯邊欄和下載對話方塊上列為動態轉譯。

>[!NOTE]
>
>如果AEM Author執行個體未在中執行 **[!UICONTROL Dynamic Media模式]** (客戶尚未購買Dynamic Media)，則 **[!UICONTROL 金字塔TIFF]**  上傳時不會建立資產的轉譯。 影像預設集或動態轉譯可用於 **[!UICONTROL 金字塔TIFF]** ，因此如果 **[!UICONTROL 金字塔TIFF]** 無法在AEM Author執行個體上使用，因此也無法在Brand Portal上使用。 因此，資產詳細資訊頁面和下載對話方塊的轉譯邊欄中不會出現動態轉譯。

若要將影像預設集發佈至Brand Portal：

1. 在AEM作者執行個體中，點選/按一下AEM標誌以存取全域導覽主控台，然後點選/按一下「工具」圖示並導覽至 **[!UICONTROL 「資產」>「影像預設集」]**.
1. 從影像預設集清單中選取影像預設集或多個影像預設集，然後按一下/點選 **[!UICONTROL 發佈至Brand Portal]**.

![](assets/publishpreset.png)

>[!NOTE]
>
>當使用者按一下 **[!UICONTROL 發佈至Brand Portal]** 影像預設集已排入發佈佇列。 建議使用者監控復寫代理程式的記錄，以確認發佈是否成功。

若要從Brand Portal取消發佈影像預設集：

1. 在AEM Author例項中，點選/按一下AEM標誌以存取全域導覽主控台，然後點選/按一下 **[!UICONTROL 工具]** 圖示並導覽至 **[!UICONTROL 「資產」>「影像預設集」]**.
1. 選取影像預設集，然後選取 **[!UICONTROL 從Brand Portal移除]** 從上方的可用選項取得。

## 將中繼資料結構描述發佈至Brand Portal  {#publish-metadata-schema-to-brand-portal}

中繼資料結構描述在資產/集合的屬性頁面上顯示的版面和屬性。

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

如果使用者已編輯AEM Author例項上的預設結構描述，並願意使用與Brand Portal上的預設結構描述相同的結構描述，他們只需將中繼資料結構描述表單發佈到Brand Portal即可。 在這種情況下，Brand Portal的預設結構會由從AEM Author例項發佈的預設結構描述取代。

如果使用者已在AEM Author例項上建立自訂結構描述，他們可以將該自訂結構描述發佈到Brand Portal，而不是在那裡重新建立相同的自訂結構描述。 之後，使用者可以將此自訂結構描述套用至Brand Portal中的任何資料夾/集合。

>[!NOTE]
>
>如果預設結構描述在AEM執行個體上鎖定（即未編輯），則無法發佈到Brand Portal。

![](assets/default-schema-form.png)

>[!NOTE]
>
>如果資料夾在AEM Author例項上套用了結構描述，則Brand Portal上也必須存在相同的結構描述，以保持AEM Author和Brand Portal上資產屬性頁面的一致性。

若要將中繼資料結構從AEM Author例項發佈至Brand Portal：

1. 在AEM作者執行個體中，點選/按一下AEM標誌以存取全域導覽主控台，然後點選/按一下「工具」圖示並導覽至 **[!UICONTROL 資產>中繼資料結構]**.
1. 選取中繼資料結構，然後選取 **[!UICONTROL 發佈至Brand Portal]** 從上方的可用選項取得。

>[!NOTE]
>
>當使用者按一下 **[!UICONTROL 發佈至Brand Portal]**，中繼資料結構會排入發佈佇列。 建議使用者監控復寫代理程式的記錄，以確認發佈是否成功。

若要從Brand Portal取消發佈中繼資料結構：

1. 在AEM作者執行個體中，點選/按一下AEM標誌以存取全域導覽主控台，然後點選/按一下「工具」圖示並導覽至 **[!UICONTROL 資產>中繼資料結構]**.
1. 選取中繼資料結構，然後選取 **[!UICONTROL 從Brand Portal移除]** 從上方的可用選項取得。

## 將搜尋Facet發佈至Brand Portal {#publish-search-facets-to-brand-portal}

搜尋表單可提供 [多面向搜尋](../using/brand-portal-search-facets.md) 傳送給使用Brand Portal的使用者。 搜尋Facet可為Brand Portal上的搜尋提供更精細的粒度。 所有 [述詞已新增](https://experienceleague.adobe.com/docs/experience-manager-65/assets/administer/search-facets.html) 使用者可在搜尋篩選器中以搜尋Facet的形式使用搜尋表單中的。

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

如果您願意使用自訂搜尋表單 **[!UICONTROL 資產管理搜尋邊欄]** 從AEM Author例項，您可以將自訂搜尋表單從AEM Author例項發佈到Brand Portal，而不是在Brand Portal上重新建立相同的表單。

>[!NOTE]
>
>鎖定的搜尋表單 **[!UICONTROL 資產管理搜尋邊欄]** 除非經過編輯，否則無法將on AEM Assets發佈至Brand Portal。 編輯並發佈至Brand Portal後，此搜尋表單會覆寫Brand Portal上的搜尋表單。

若要將編輯後的搜尋Facet從AEM作者執行個體發佈至Brand Portal：

1. 点按/单击 AEM 徽标，然后转到&#x200B;**[!UICONTROL 工具 > 常规 > 搜索表单]**。
1. 選取已編輯的搜尋表單，然後選取 **[!UICONTROL 發佈至Brand Portal]**.

   >[!NOTE]
   >
   >當使用者按一下 **[!UICONTROL 發佈至Brand Portal]**，搜尋Facet會排入發佈佇列。 建議使用者監控復寫代理程式的記錄，以確認發佈是否成功。

若要從Brand Portal取消發佈搜尋表單：

1. 在AEM作者執行個體中，點選/按一下AEM標誌以存取全域導覽主控台，然後點選/按一下「工具」圖示並導覽至 **[!UICONTROL 「一般>搜尋Forms」]**.
1. 選取搜尋表單，然後選取 **[!UICONTROL 從Brand Portal移除]** 從上方的可用選項取得。

>[!NOTE]
>
>此 **[!UICONTROL 從Brand Portal取消發佈]** 動作會保留Brand Portal上的預設搜尋表單，不會還原為發佈前使用的最後一個搜尋表單。

### 限制 {#limitations}

1. 少數搜尋述詞不適用於Brand Portal上的搜尋篩選器。 當這些搜尋述詞作為搜尋表單的一部分從AEM Author執行個體發佈到Brand Portal時，它們會被篩選掉。 因此，使用者在Brand Portal看到的已發佈表單述詞數量較少。 另請參閱 [適用於Brand Portal上篩選器的搜尋述詞](../using/brand-portal-search-facets.md#list-of-search-predicates).

1. 對象 [!UICONTROL 選項述詞]，如果使用者在AEM Author例項使用任何自訂路徑來讀取選項，它將無法在Brand Portal運作。 這些額外的路徑和選項不會以搜尋表單發佈至Brand Portal。 在此情況下，使用者可以選取 **[!UICONTROL 手動]** 中的選項 **[!UICONTROL 新增選項]** 範圍 **[!UICONTROL 選項述詞]** 以在Brand Portal手動新增這些選項。

![](assets/options-predicate-manual.png)
