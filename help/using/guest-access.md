---
title: 来宾访问 Brand Portal
seo-title: Guest Access to Brand Portal
description: 允許訪客存取，並省下在未驗證的情況下載入許多使用者的工作。
seo-description: Allow guest access and save the effort to onboard numerous users without authentication.
uuid: edb4378d-1710-44a2-97a6-594d99f62fff
contentOwner: VG
topic-tags: introduction
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: b9e9fe7b-0373-42d1-851b-7c76b47657c2
exl-id: ecce0a45-abae-41c4-9ea7-5dfdcf19e5ea
source-git-commit: 51dc6f9c3b3a59751d7910513279e52906d97b88
workflow-type: tm+mt
source-wordcount: '1026'
ht-degree: 0%

---

# 来宾访问 Brand Portal {#guest-access-to-brand-portal}

Experience Manager Assets Brand Portal可讓訪客存取入口網站。 訪客使用者不需要認證即可進入入口網站，且可以存取入口網站的公開資產（和集合）。 來賓工作階段中的使用者可以將資產新增至Lightbox （私人集合）並下載相同的資產，直到其工作階段持續為止，也就是從工作階段開始算起2小時，除非來賓使用者選擇這樣做 [[!UICONTROL 結束工作階段]](#exit-guest-session).

訪客存取功能可讓組織執行下列動作 [快速共用核准的資產](../using/brand-portal-sharing-folders.md#how-to-share-folders) 可大規模提供目標對象，而不需將其加入。 Brand Portal 6.4.2之後已可同時為多位訪客使用者提供服務，佔每個組織使用者配額總數的10%。 允許訪客存取，可節省在Brand Portal上管理功能有限的使用者並上線分數的時間。\
組織可以使用對組織的Brand Portal帳戶啟用（或停用）訪客存取 **[!UICONTROL 允許訪客存取]** 選項來源 **[!UICONTROL 存取]** 「管理工具」面板中的設定。

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## 開始來賓工作階段 {#begin-guest-session}

若要以匿名方式進入Brand Portal，請選取 **[!UICONTROL 按一下這裡]** 對應至 **[!UICONTROL 訪客存取？]** 在Brand Portal歡迎畫面上。 輸入驗證碼安全性檢查以授予使用Brand Portal的存取權。

![](assets/bp-login-screen.png)

## 來賓工作階段持續時間 {#guest-session-duration}


訪客使用者工作階段會維持15分鐘的有效狀態。
這表示 **[!UICONTROL Lightbox]** 會從工作階段開始時間保留15分鐘，之後目前的來賓工作階段會重新啟動，因此Lightbox狀態會遺失。

例如，某個訪客使用者在1500小時登入Brand Portal，並將資產新增至 **[!UICONTROL Lightbox]** 於15:05下載。 如果使用者不下載 **[!UICONTROL Lightbox]** 集合（或其資產）在15:15小時（登入後15分鐘內）之前，使用者必須重新啟動工作階段。 此 **[!UICONTROL Lightbox]** 空白，這表示如果工作階段遺失，上傳的資產就不再可用。

## 允許並行來賓工作階段 {#concurrent-guest-sessions-allowed}

每個組織的同時來賓工作階段數限製為使用者配額總數的10%。 這表示對於使用者配額為200個的組織來說，最多可同時工作20個訪客使用者。 第21位使用者被拒絕存取，而且只有在20位使用中來賓使用者的工作階段結束時，才能以來賓身分存取。

>[!NOTE]
>
>如果授權使用者人數超過合約值（配額），Brand Portal不會傳送通知。 此外，它不會限制授權使用者的任何活動。

## 訪客使用者與Brand Portal的互動 {#guest-user-interaction-with-brand-portal}

### 來賓UI導覽

以訪客身分進入Brand Portal時，使用者可看到 [資產和資料夾已共用](../using/brand-portal-sharing-folders.md#sharefolders) 公開或只與訪客使用者合作。 此檢視是僅內容檢視，以卡片、清單或欄配置顯示資產。

![](assets/disabled-folder-hierarchy1.png)

但如果管理員已啟用，訪客使用者在登入Brand Portal時，將會看到資料夾樹狀結構（從根資料夾開始）和共用資料夾在各自的父資料夾中排列 [啟用資料夾階層](../using/brand-portal-general-configuration.md#main-pars-header-1621071021) 設定。

這些父資料夾是虛擬資料夾，無法對它們執行任何動作。 您可以使用鎖定圖示來識別這些虛擬資料夾。

暫留或選取動作任務時未顯示任何動作任務 **[!UICONTROL 卡片檢視]**，不同於共用資料夾。 **[!UICONTROL 概觀]** 選擇中的虛擬資料夾時顯示按鈕 **[!UICONTROL 欄檢視]** 和 **[!UICONTROL 清單檢視]**.

>[!NOTE]
>
>虛擬資料夾的預設縮圖為第一個共用資料夾的縮圖影像。

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

**[!UICONTROL 檢視設定]** 選項可讓訪客使用者調整卡片大小 **[!UICONTROL 卡片檢視]** 或欄顯示 **[!UICONTROL 清單檢視]**.

![](assets/nav-guest-user.png)

此 **[!UICONTROL 內容樹狀結構]** 可讓您移動資產階層。

![](assets/guest-login-ui.png)

Brand Portal提供 **[!UICONTROL 概觀]** 訪客使用者可檢視的選項 **[!UICONTROL 資產屬性]** 個資產/資料夾的位置。 此 **[!UICONTROL 概觀]** 選項可見：

* 在頂端的工具列中選取資產/資料夾。
* 在下拉式清單中選取「邊欄選取器」。

選取 **[!UICONTROL 概觀]** 選項選取資產/資料夾時，使用者可檢視資產建立的標題、路徑和時間。 而在資產詳細資訊頁面上選取 **[!UICONTROL 概觀]** 選項可讓使用者檢視資產的中繼資料。

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)

**[!UICONTROL 導覽]** 左側邊欄中的選項可讓您從檔案導覽至收藏集，然後返回guest工作階段，以便使用者可以瀏覽檔案或收藏集中的資產。

**[!UICONTROL 篩選]** 選項可讓訪客使用者使用管理員設定的搜尋述詞來篩選資產檔案和資料夾。

### 訪客使用者功能

訪客使用者可以存取Brand Portal上的公開資產，且幾乎沒有限制，詳細內容將詳加討論。

**訪客使用者可以**：

* 存取適用於所有Brand Portal使用者的所有公用資料夾和集合。
* 瀏覽成員、詳細資訊頁面，並擁有所有公用資料夾和集合成員的完整資產檢視。
* 在公用資料夾和集合中搜尋資產。
* 將資產新增至Lightbox集合。 這些對集合的變更會在工作階段期間持續存在。
* 直接或透過Lightbox集合下載資產。

**訪客使用者無法**：

* 建立收藏集和已儲存的搜尋，或進一步共用它們。
* 存取資料夾和集合設定。
* 以連結形式共用資產。

### 下載來賓工作階段中的資產

訪客使用者可以直接下載在Brand Portal上公開或專門與訪客使用者共用的資產。 訪客使用者也可以將資產新增至 **[!UICONTROL Lightbox]** （公開收集），並下載 **[!UICONTROL Lightbox]** 在工作階段過期之前的集合。

若要下載資產和收藏集，請使用下列位置的下載圖示：

* 快速動作縮圖，當游標停留在資產或集合上時便會顯示
* 頂端的工具列，會在選取資產或集合時顯示

![](assets/download-on-guest.png)

選取 **[!UICONTROL 啟用加速下載]** 於 [!UICONTROL 下載] 對話方塊可讓您 [提升下載效能](../using/accelerated-download.md).

## 退出來賓工作階段 {#exit-guest-session}

若要結束來賓工作階段，請使用 **[!UICONTROL 結束工作階段]** 從標題中可用的選項中選取。 不過，如果用於來賓工作階段的瀏覽器索引標籤非使用中，則工作階段會在兩小時非使用後自動過期。

![](assets/end-guest-session.png)

## 監視來賓使用者活動 {#monitoring-guest-user-activities}

管理員可以透過Brand Portal監控訪客使用者互動。 在Brand Portal中產生的報表可提供訪客使用者活動的關鍵深入分析。 例如， **[!UICONTROL 下載]** 報表可用來追蹤訪客使用者下載的資產計數。 **[!UICONTROL 使用者登入]** 報告可告知訪客使用者上次登入入口網站的時間，以及指定期間內的登入頻率。
