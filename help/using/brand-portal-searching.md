---
title: 在 Brand Portal 上搜索资产
seo-title: Asset searching and saved search on Experience Manager Assets Brand Portal
description: Brand Portal搜尋功能可讓您使用omnisearch快速搜尋相關資產，而搜尋篩選器可協助您進一步縮小搜尋範圍。 將搜尋儲存為智慧型系列，以供日後使用。
seo-description: Brand Portal search capability lets you quickly search for relevant assets using omnisearch, and search filters help you further narrow down your search. Save your searches as smart collections for future.
uuid: c2955198-bdc0-4853-a13a-661e6a9ec61f
contentOwner: bdhar
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: SearchandPromote
discoiquuid: dc751cd7-f663-46d2-84c4-5bb12a4fe1ba
exl-id: 7297bbe5-df8c-4d0b-8204-218a9fdc2292
source-git-commit: cbdd943b904882cc9a455bab24c3cf732d5966ca
workflow-type: tm+mt
source-wordcount: '1358'
ht-degree: 5%

---

# 在 Brand Portal 上搜索资产 {#search-assets-on-brand-portal}

Brand Portal搜尋功能可讓您使用omnisearch快速搜尋相關資產，以及使用篩選器的多面向搜尋，以協助您進一步縮小搜尋範圍。 您可以在檔案或資料夾層級搜尋資產，並將搜尋結果儲存為智慧型集合。

>[!NOTE]
>
>Brand Portal不支援使用omnisearch進行集合搜尋。
>
>不過，您可以使用 [搜尋篩選器以取得相關集合的清單](#search-collection).

## 使用Omnisearch搜尋資產 {#search-assets-using-omnisearch}

若要在Brand Portal上搜尋資產：

1. 在工具列中，按一下 **[!UICONTROL 搜尋]** 圖示，或按下「**[!UICONTROL /]**」啟動Omnisearch的索引鍵。

   ![](assets/omnisearchicon-1.png)

1. 在搜尋方塊中，輸入您要搜尋之資產的關鍵字。

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >* omnisearch中至少需要3個字元，才會顯示搜尋建議。
   >* 當您搜尋 `mountain biking`，omnisearch會傳回搜尋結果中所有同時具備的資產 `mountain` 和 `biking` 在中繼資料欄位中提供。 例如， `mountain` 在 `Title` 欄位和 `biking` 在 `Description` 欄位。 這兩個字詞都必須在中繼資料欄位中可用，才能顯示在搜尋結果中。 不過，即使「智慧標籤」中繼資料欄位中只有兩個辭彙其中之一可用，Omnisearch仍會在搜尋結果中傳回資產。 例如，如果資產包含 `mountain` 作為其中一個智慧標籤，不包含 `biking` 在任何其他中繼資料欄位中搜尋 `mountain biking`，omnisearch仍會在搜尋結果中傳回資產。


1. 從下拉式清單中顯示的相關建議中選取，以快速存取相關資產。

   ![](assets/assets-search-result.png)

   *使用Omnisearch搜尋資產*

若要瞭解使用智慧標籤資產的搜尋行為，請參閱 [瞭解搜尋結果和行為](https://experienceleague.adobe.com/docs/experience-manager-65/assets/using/search-assets.html).

## 在「篩選器」面板中使用Facet進行搜尋 {#search-using-facets-in-filters-panel}

「篩選器」面板中的搜尋Facet可為您的搜尋體驗增加精細度，並讓搜尋功能有效率。 搜尋Facet會使用多個維度（述詞），讓您執行複雜的搜尋。 您可以輕鬆向下鑽研至所需的詳細資訊層級，以更集中地搜尋。

例如，如果您要尋找影像，您可以選擇想要點陣圖或向量影像。 您可以在「檔案型別」搜尋面向中指定影像的MIME型別，進一步縮小搜尋範圍。 同樣地，在搜尋檔案時，您可以指定格式，例如PDF或MS® Word格式。

![Brand Portal中的篩選器面板](assets/file-type-search.png "Brand Portal中的篩選器面板")

此 **[!UICONTROL 篩選器]** 面板包含幾個標準面向，例如 —  **[!UICONTROL 路徑瀏覽器]**， **[!UICONTROL 檔案型別]**， **[!UICONTROL 檔案大小]**， **[!UICONTROL 狀態]**、和 **[!UICONTROL 方向]**. 不過，您可以 [新增自訂搜尋Facet](../using/brand-portal-search-facets.md) 或從中移除特定搜尋Facet **[!UICONTROL 篩選器]** 面板，方法是在基礎搜尋表單中新增或移除述詞。 檢視可用和可用的 [Brand Portal上的搜尋述詞](../using/brand-portal-search-facets.md#list-of-search-predicates).

若要將篩選器套用至您的搜尋，請使用可用的 [搜尋Facet](../using/brand-portal-search-facets.md)：

1. 按一下覆蓋圖示並選取 **[!UICONTROL 篩選]**.

   ![](assets/selectorrail.png)

1. 從 **[!UICONTROL 篩選器]** 面板中，選取適當的選項以套用相關的篩選器。
例如，使用下列標準篩選器：

   * **[!UICONTROL 路徑瀏覽器]** 以搜尋特定目錄中的資產。 路徑瀏覽器的述詞預設搜尋路徑為 `/content/dam/mac/<tenant-id>/`，可透過編輯預設搜尋表單進行設定。
   >[!NOTE]
   >
   >對於非管理員使用者， [!UICONTROL 路徑瀏覽器] 在 [!UICONTROL 篩選] 面板僅顯示與其共用的資料夾（及其上級資料夾）的內容結構。\
   >路徑瀏覽器可讓管理員使用者導覽至Brand Portal中的任何資料夾。

   * **[!UICONTROL 檔案型別]** 以指定您要尋找的資產檔案型別（影像、檔案、多媒體、封存）。 此外，您可以縮小搜尋範圍，例如，為影像或檔案格式(PDF或MS® Word)指定MIME型別（Tiff、點陣圖、GIMP影像）。
   * **[!UICONTROL 檔案大小]** 以根據資產的大小來搜尋資產。 您可以指定大小範圍的下限和上限來縮小搜尋範圍，並指定要搜尋的度量單位。
   * **[!UICONTROL 狀態]** 以根據資產狀態(例如，核准（已核准、已要求變更、已拒絕、待處理）和到期)搜尋資產。
   * **[!UICONTROL 平均評分]** 以根據資產的評等搜尋資產。
   * **[!UICONTROL 方向]** 以根據資產的方向（水準、垂直、正方形）搜尋資產。
   * **[!UICONTROL 樣式]** 以根據資產的樣式（彩色、單色）搜尋資產。
   * **[!UICONTROL 視訊格式]** 根據格式(DVI、Flash、MPEG4、MPEG、OGG Theora、QuickTime、Windows Media、WebM)搜尋視訊資產。

   您可以使用 [自訂搜尋Facet](../using/brand-portal-search-facets.md) 編輯基礎的「搜尋表單」，即可在「篩選器」面板中選取。

   * **[!UICONTROL 屬性述詞]** 若用於搜尋表單，可讓您搜尋符合述詞對應之中繼資料屬性的資產。\
      例如，如果屬性述詞對應到 [!UICONTROL `jcr:content /metadata/dc:title`]，您可以根據資產的標題來搜尋資產。\
      此 [!UICONTROL 屬性述詞] 支援下列文字搜尋：

      **部分短语**&#x200B;要允许使用属性谓词中的部分短语进行资产搜索，请在“搜索表单”中启用&#x200B;**[!UICONTROL 部分搜索]**&#x200B;复选框。该功能允许您搜索所需的资产，即使您没有指定资产元数据中使用的确切字词/短语。

      >[!NOTE]
      >
      > Brand Portal支援下列「部分搜尋」欄位：
      >* jcr：content/metadata/dc：title
      >* jcr：content/jcr：title
      >* jcr：content/metadata/dam：search_promote
      >* jcr:content/metadata/dc:format


      您可以：
      * 在「篩選器」面板的Facet中，指定搜尋片語中的單字。 例如，如果您搜尋字詞 **爬升** (屬性述詞對應至 [!UICONTROL `dc:title`] 屬性)，然後所有含有單字的資產 **爬升** 會傳回標題片語。
      * 指定搜尋片語中單字的一部分，以及萬用字元(&#42;)填滿間隙。
例如，搜索：
         * **爬升&#42;** 傳回標題片語中字元開頭為「climb」的所有資產。
         * **&#42;爬升** 傳回標題片語中字詞結尾為「climb」的所有資產。
         * **&#42;爬升&#42;** 傳回其標題片語中包含「climb」字元的所有資產。

若要允許在屬性述詞中進行不區分大小寫的搜尋，請啟用       **不區分大小寫的文字**
若要允許在屬性述詞中進行不區分大小寫的搜尋，請啟用 **[!UICONTROL 忽略大小寫]** 「搜尋表單」中的核取方塊。 依預設，屬性述詞的文字搜尋會區分大小寫。
   >[!NOTE]
   >
   >選取時 **[!UICONTROL 部分搜尋]** 核取方塊、 **[!UICONTROL 忽略大小寫]** 預設為選取。

   ![](assets/wildcard-prop-1.png)

   搜尋結果會根據套用的篩選以及搜尋結果計數顯示。

   ![](assets/omnisearch-with-filters.png)

   具有搜尋結果計數的資產搜尋結果。

1. 您可以從搜尋結果輕鬆導覽至某個專案，然後使用瀏覽器中的「上一步」按鈕返回相同的搜尋結果，而不必重新執行搜尋查詢。

## 將搜尋儲存為智慧型集合 {#save-your-searches-as-smart-collection}

您可以將搜尋設定儲存為智慧型集合，以便快速重複相同的搜尋，而不必稍後重做相同的設定。 不過，您無法在集合中套用搜尋篩選器。

若要將搜尋設定儲存為智慧型集合：

1. 點選/按一下 **[!UICONTROL 儲存智慧型集合]** 並提供智慧型集合的名稱。

   若要讓所有使用者都能存取智慧型集合，請選取 **[!UICONTROL 公用]**. 系統會顯示一則訊息，確認智慧型系列已建立，並已新增至已儲存搜尋的清單中。

   >[!NOTE]
   >
   >可限制非管理員使用者將智慧型集合設為公開，以避免非管理員使用者在組織的Brand Portal上建立大量公開的智慧型集合。 組織可以停用 **[!UICONTROL 允許建立公開的智慧型集合]** 設定來源 **[!UICONTROL 一般]** 「管理工具」面板中可用的設定。

   ![](assets/save_smartcollectionui.png)

1. 若要以不同名稱儲存智慧型集合，請選取或清除 **[!UICONTROL 公用]** 核取方塊，按一下 **[!UICONTROL 編輯智慧型集合]**.

   ![](assets/edit_smartcollection.png)

1. 於 **[!UICONTROL 編輯智慧型集合]** 對話方塊，選取 **[!UICONTROL 另存為]** 並輸入智慧型集合的名稱。 单击“**[!UICONTROL 保存]**”。

   ![](assets/saveas_smartsearch.png)


## 搜尋集合 {#search-collection}

集合不支援Omnisearch。 不過，您可以套用搜尋篩選條件，以從 [!UICONTROL 集合] 介面。

從 [!UICONTROL 集合] 介面，按一下覆蓋圖示以開啟左側欄中的篩選面板。 從可用的篩選器套用單一或多個搜尋篩選器(`modified date`， `access type`、和 `tags`)。 它會根據套用的篩選器列出最相關的集合集。

![](assets/collection-search.png)
