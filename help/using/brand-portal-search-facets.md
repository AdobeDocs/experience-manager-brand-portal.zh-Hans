---
title: 使用自定义搜索 Facet
seo-title: Use custom search facets
description: 管理員可以將搜尋述詞新增至篩選器面板，以自訂搜尋並使搜尋功能通用。
seo-description: Administrators can add search predicates to the Filters panel to customize search and make the search functionality versatile.
uuid: 986fba5a-fac5-4128-ac75-d04da5b52d45
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 19faa028-246b-42c7-869f-97c95c7a1349
role: Admin
exl-id: c07e1268-2c83-40ba-8dcd-5dade3a10141
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '1279'
ht-degree: 9%

---

# 使用自定义搜索 Facet {#use-custom-search-facets}

管理員可以將搜尋述詞新增至 [!UICONTROL 篩選器] 面板，可自訂搜尋並使搜尋功能通用。

Brand Portal支援 [多面向搜尋](../using/brand-portal-searching.md#search-using-facets-in-filters-panel) 針對已核准品牌資產的細微搜尋，可能原因如下： [**篩選器** 面板](../using/brand-portal-searching.md#search-using-facets-in-filters-panel). 透過以下方式，可在「篩選器」面板上使用搜尋Facet： **[!UICONTROL 搜尋表單]** （在管理工具中）。 名為「資產管理搜尋邊欄」的預設搜尋表單存在於管理工具的「搜尋Forms」頁面中。 不過，管理員可以透過新增、修改或移除搜尋述詞來編輯預設搜尋表單（資產管理員搜尋邊欄），進而自訂預設篩選面板，從而使搜尋功能具有通用性。

您可以使用各種搜尋述詞來自訂 **[!UICONTROL 篩選器]** 面板。 例如，新增屬性述詞，以搜尋符合您在此述詞中指定的單一屬性的資產。 新增選項述詞，以搜尋符合您為特定屬性指定的一或多個值的資產。 新增日期範圍述詞，以搜尋在指定日期範圍內建立的資產。

>[!NOTE]
>
>Experience Manager Assets可讓組織 [從AEM Author發佈自訂搜尋表單](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal) Brand Portal，而不要在Brand Portal上重新建立相同的表單。

## 新增搜尋述詞 {#add-a-search-predicate}

將搜尋述詞新增至 **[!UICONTROL 篩選器]** 面板：

1. 若要存取管理工具，請按一下頂端工具列中的Experience Manager標誌。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，按一下 **[!UICONTROL 搜尋Forms]**.

   ![](assets/navigation-panel-1.png)

1. 在 **[!UICONTROL 搜尋Forms]** 頁面，選取 **[!UICONTROL 資產管理搜尋邊欄]**.

   ![](assets/search-forms-page.png)

1. 在頂端出現的工具列上，按一下 **[!UICONTROL 編輯]** 以開啟「編輯搜尋」表單。

   ![](assets/edit-search-form-1.png)

1. 在 [!UICONTROL 編輯搜尋表單] 頁面，從拖曳述詞 [!UICONTROL 選取述詞] 標籤移至主窗格。 例如，拖曳 **[!UICONTROL 屬性述詞]**.

   此 **[!UICONTROL 屬性]** 欄位會顯示在主窗格中，而 **[!UICONTROL 設定]** 索引標籤在右側顯示屬性述詞。

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >中的標題標籤 **[!UICONTROL 設定]** tab會識別您選取的述詞型別。

1. 在 **[!UICONTROL 設定]** 標籤，輸入屬性述詞的標籤、預留位置文字和說明。

   * 選取 **[!UICONTROL 部分搜尋]**，如果您想要根據指定的屬性值允許資產的部分片語搜尋（和萬用字元搜尋）。 依預設，述詞支援全文檢索搜尋。
   * 選取 **[!UICONTROL 忽略大小寫]**，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，，， 依預設，搜尋篩選條件中的搜尋屬性值會區分大小寫。

   >[!NOTE]
   >
   >選取時 **[!UICONTROL 部分搜尋]** 核取方塊、 **[!UICONTROL 忽略大小寫]** 預設為選取。

1. 在 **[!UICONTROL 屬性名稱]** 欄位，開啟屬性選擇器，然後選取執行搜尋所依據的屬性。 或者，輸入屬性的名稱。 例如，输入 `  jcr :content/metadata/dc:title` 或 `./jcr:content/metadata/dc:title`。

   >[!NOTE]
   >
   >在Brand Portal中，所有屬性(開頭為 `xmp`)，在 `jcrcontent/metadata` 之 `dam:asset` 預設會編制索引。
   >
   >建立屬性述詞時，可以使用任何已編制索引的屬性。 如果設定了任何非索引屬性，則未索引屬性上的搜尋查詢可能不會提供任何搜尋結果。

   ![](assets/title-prop.png)

1. 按一下 **[!UICONTROL 完成]** 以儲存設定。
1. 從 [!UICONTROL 資產] 使用者介面，按一下覆蓋圖示並選擇 **[!UICONTROL 篩選]** 導覽至 **[!UICONTROL 篩選器]** 面板。 此 **[!UICONTROL 屬性]** 述詞會新增至面板。

   ![](assets/property-filter-panel.png)

1. 在中輸入要搜尋的資產的標題 **[!UICONTROL 屬性]** 文字方塊。 例如，「Adobe」。 執行搜尋時，標題符合「Adobe」的資產會顯示在搜尋結果中。

## 搜尋述詞清單 {#list-of-search-predicates}

類似於新增 **[!UICONTROL 屬性]** 述詞，您可以將下列述詞新增至 **[!UICONTROL 篩選器]** 面板：

| **述詞名稱** | **描述** | **属性** |
|-------|-------|----------|
| **[!UICONTROL 路径浏览器]** | 搜尋述詞，可搜尋特定位置的資產。 **注意：** *對於登入的使用者，篩選器上的路徑瀏覽器僅顯示與該使用者共用的資料夾（及其祖先）的內容結構。* <br> 管理員使用者可使用路徑瀏覽器導覽至任何資料夾，以搜尋該資料夾中的資產。 <br> 反之，非管理員使用者可在路徑瀏覽器中導覽至資料夾（可由他們存取），在該資料夾中搜尋資產。 | <ul><li>字段标签</li><li>路径</li><li>描述</li></ul> |
| **[!UICONTROL 属性]** | 根據特定中繼資料屬性搜尋資產。 **注意：** *選取「部分搜尋」時，預設會選取「忽略大小寫」*. | <ul><li>字段标签</li><li>占位符</li><li>属性名称</li><li>部分搜索</li><li>忽略大小写</li><li> 描述</li></ul> |
| **[!UICONTROL 多值屬性]** | 類似於屬性述詞，但允許多個輸入值，以分隔字元（預設為COMMA）分隔[，])結果中會傳回符合任何輸入值的資產。 | <ul><li>字段标签</li><li>占位符</li><li>属性名称</li><li>分隔符支持</li><li>忽略大小写</li><li>描述</li></ul> |
| **[!UICONTROL 标记]** | 搜尋述詞，以根據標籤搜尋資產。 您可以設定Path屬性以填入Tags清單中的各種標籤。 *注意：管理員可能需要變更路徑值，例如 [!UICONTROL `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`]，如果他們從AEM發佈搜尋表單，其中路徑不包含租使用者資訊，例如 [!UICONTROL `/etc/tags/<custom_tag_namespace>`]. | <ul><li>字段标签</li><li>属性名称</li><li>路径</li><li>描述</li></ul> |
| **[!UICONTROL 路径]** | 搜尋述詞，可搜尋特定位置的資產。 | <ul><li>字段标签</li><li>路径</li><li>描述</li></ul> |  |
| **[!UICONTROL 相对日期]** | 搜尋述詞，以根據資產的相對建立日期來搜尋資產。 | <ul><li>字段标签</li><li>属性名称</li><li>相對日期</li></ul> |
| **[!UICONTROL 范围]** | 搜尋述詞，可搜尋位於指定屬性值範圍內的資產。 在「篩選器」面板中，您可以指定範圍的最小和最大屬性值。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 日期范围]** | 搜尋述詞，以搜尋在指定範圍內建立的資產，以取得日期屬性。 在「篩選器」面板中，您可以指定「開始」和「結束」日期。 | <ul><li>字段标签</li><li>占位符</li><li>属性名称</li><li>範圍文字（從）</li><li>範圍文字（至）</li><li>描述</li></ul> |
| **[!UICONTROL 日期]** | 根據日期屬性的資產滑桿式搜尋的搜尋述詞。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 檔案大小]** | 搜尋述詞，以根據資產的大小進行搜尋。 | <ul><li>字段标签</li><li>属性名称</li><li>路径</li><li>描述</li></ul> |
| **[!UICONTROL 上次修改的资源]** | 搜尋述詞，以根據上次修改日期搜尋資產。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 核准狀態]** | 搜尋述詞，以根據核准中繼資料屬性搜尋資產。 預設屬性名稱為 **dam：status**. | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 签出状态]** | 搜尋述詞，以在資產從AEM Assets發佈時根據資產的簽出狀態搜尋資產。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 签出方]** | 搜尋述詞，以根據已取出資產的使用者來搜尋資產。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 到期状态]** | 搜尋述詞，以根據到期狀態搜尋資產。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 集合成員]** | 根據資產是否為集合的一部分來搜尋資產的搜尋述詞。 | 描述 |
| **[!UICONTROL 隐藏]** | 一般使用者無法明確看見此述詞，且此述詞用於任何隱藏的限制，通常用於將搜尋結果型別限製為 **dam：Asset**. | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |

>[!NOTE]
>
>不要使用 **[!UICONTROL 選項述詞]**， **[!UICONTROL 發佈狀態述詞]**、和 **[!UICONTROL 評等述詞]** 因為這些述詞在Brand Portal中無法運作。

## 刪除搜尋述詞 {#delete-a-search-predicate}

若要刪除搜尋述詞，請遵循下列步驟：

1. 按一下Adobe標誌以存取管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，按一下 **[!UICONTROL 搜尋Forms]**.

   ![](assets/navigation-panel-2.png)

1. 在 **[!UICONTROL 搜尋Forms]** 頁面，選取 **[!UICONTROL 資產管理搜尋邊欄]**.

   ![](assets/search-forms-page.png)

1. 在頂端出現的工具列上，按一下 **[!UICONTROL 編輯]** 以開啟「編輯搜尋」表單。

   ![](assets/edit-search-form-2.png)

1. 在 [!UICONTROL 編輯搜尋表單] 頁面，從主窗格中選取您要刪除的述詞。 例如，選取 **[!UICONTROL 屬性述詞]**.

   此 **[!UICONTROL 設定]** 索引標籤在右側顯示屬性述詞欄位。

1. 若要刪除屬性述詞，請按一下bin圖示。 於 **[!UICONTROL 刪除欄位]** 對話方塊中，按一下 **[!UICONTROL 刪除]** 以確認刪除動作。

   此 **[!UICONTROL 屬性述詞]** 欄位會從主窗格中移除，而 **[!UICONTROL 設定]** 索引標籤會變成空白。

   ![](assets/search-form-delete-predicate.png)

1. 若要儲存變更，請按一下 **[!UICONTROL 完成]** （在工具列中）。
1. 從 **[!UICONTROL 資產]** 使用者介面，按一下覆蓋圖示並選擇 **[!UICONTROL 篩選]** 導覽至 **[!UICONTROL 篩選器]** 面板。 此 **[!UICONTROL 屬性]** 述詞會從面板中移除。

   ![](assets/property-predicate-removed.png)
