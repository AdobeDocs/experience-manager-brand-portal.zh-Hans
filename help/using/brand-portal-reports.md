---
title: 使用报告
seo-title: Work with reports
description: Experience Manager Assets Brand Portal管理員可檢視Brand Portal使用情況報表，以及建立、管理和檢視有關已下載、過期、已發佈和透過Brand Portal共用之連結的資產報表。
seo-description: Experience Manager Assets Brand Portal Administrators can view report about Brand Portal usage, and create, manage, and view reports around assets downloaded, expired, published, and link shared through Brand Portal.
uuid: dc4e5275-a614-4b95-8c70-2b7e470c50a7
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 7683074f-b6ea-42e0-a411-3b13eb88d1f2
role: Admin
exl-id: 03d0292c-23c2-4ea0-9781-eb27768e6c33
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '996'
ht-degree: 2%

---

# 使用报告 {#work-with-reports}

報告功能有助於評估Brand Portal的使用情況，並瞭解內部和外部使用者如何與已核准的資產互動。 管理員可以檢視Brand Portal使用情況報表，該報表一律可在資產報表頁面上使用。 不過，使用者登入的報告和透過連結共用的資產已下載、過期、發佈和共用的資產報告，可以從「資產報告」頁面產生和檢視。 這些報表有助於分析資產部署，讓您獲得關鍵成功量度，以衡量組織內外對已核准資產的採用程度。

報表管理介面直覺化，並包含存取已儲存報表的精細選項和控制項。 您可以從「資產報告」頁面檢視、下載或刪除報告，該頁面中列出了所有先前產生的報告。

## 檢視報告 {#view-reports}

若要檢視報表，請遵循下列步驟：

1. 從頂端的工具列中，點選/按一下Experience Manager標誌以存取管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，按一下 **[!UICONTROL 建立/管理報表]** 以開啟 **[!UICONTROL 資產報表]** 頁面。

   ![](assets/access-asset-reports.png)

1. 存取 **[!UICONTROL 使用狀況]** 報告和其他產生的報告。

   >[!NOTE]
   >
   >使用情況報告是在Brand Portal中產生的預設報告。 無法建立或刪除。 不過，您可以建立、下載和刪除「下載」、「過期」、「發佈」、「連結共用」和「使用者登入」報告。

   若要檢視報表，請按一下報表連結。 或者，選取報表，然後點選/按一下工具列中的「檢視」圖示。

   **[!UICONTROL 使用情況報表]** 顯示Brand Portal中作用中Brand Portal使用者人數、所有資產佔用的儲存空間，以及資產總數的相關資訊。 未指派給Admin Console中任何產品設定檔的Brand Portal使用者會被視為非作用中使用者，而不會反映在 **[!UICONTROL 使用情況報表]**.
報表也會顯示每個資訊量度的允許容量。

   ![](assets/usage-report.png)

   **[!UICONTROL 使用者登入]** 報表會提供登入Brand Portal之使用者的相關資訊。 報表會顯示從Brand Portal 6.4.2部署到產生報表時的每個使用者的顯示名稱、電子郵件ID、角色（管理員、檢視者、編輯者、來賓）、群組、上次登入、活動狀態和登入計數。

   ![](assets/user-logins.png)

   **[!UICONTROL 下載]** 報表會列出在特定日期和時間範圍內下載的所有資產的相關細節。

   ![](assets/download-report.png)

   >[!NOTE]
   >
   >資產 **[!UICONTROL 下載]** 報表只會顯示個別選取並從Brand Portal下載的資產。 如果使用者下載了包含資產的資料夾，報表不會顯示該資料夾或資料夾內的資產。

   **[!UICONTROL 有效期]** 報告會列出在特定時間範圍內過期的所有資產並加以詳細資訊。

   ![](assets/expiration-report.png)

   **[!UICONTROL 發佈]** 報表會列出在指定時間範圍內從Experience Manager Assets發佈至Brand Portal的所有資產，並提供相關資訊。

   ![](assets/publish-report.png)

   >[!NOTE]
   >
   >發佈報表不會顯示內容片段的相關資訊，因為內容片段無法發佈至Brand Portal。

   **[!UICONTROL 連結共用報表]** 列出特定時間範圍內透過Brand Portal介面的連結共用的所有資產。 報表也會通知透過連結共用的資產時間、使用者、連結過期時間，以及租使用者（和共用資產連結的使用者）的共用連結數量。 無法自訂連結共用報表的欄。

   ![](assets/link-share-report.png)

   >[!NOTE]
   >
   >「連結共用報表」不會顯示透過連結存取共用資產或已透過連結下載資產的使用者。
   >
   >若要透過共用連結追蹤下載，您需要在選取後產生下載報告 **[!UICONTROL 僅限連結共用下載]** 選項於 **[!UICONTROL 建立報告]** 頁面。 不過，在此情況下，使用者（下載者）是匿名的。

## 產生報表 {#generate-reports}

管理員可以產生和管理以下標準報告，產生後，就會將它們儲存為 [已存取](../using/brand-portal-reports.md#main-pars-header) 稍後：

* 用户登录
* 下载
* 到期时间
* 发布
* 链接共享

可以自訂下載、到期和發佈報告中的欄以供檢視。 若要產生報表，請遵循下列步驟：

1. 從頂端的工具列中，點選/按一下Experience Manager標誌以存取管理工具。

1. 從管理工具面板，點選/按一下 **[!UICONTROL 建立/管理報表]** 以開啟 **[!UICONTROL 資產報表]** 頁面。

   ![](assets/asset-reports.png)

1. 在资产报表页面中，点按/单击&#x200B;**[!UICONTROL 创建]**。
1. 從 **[!UICONTROL 建立報告]** 頁面，選取要建立的報表，然後點選/按一下 **[!UICONTROL 下一個]**.

   ![](assets/crete-report.png)

1. 設定報告詳細資訊。 指定下列專案的標題、說明、資料夾結構（需要執行並產生統計資料的位置）和日期範圍 **[!UICONTROL 下載]**， **[!UICONTROL 有效期]**、和 **[!UICONTROL 發佈]** 報表。

   ![](assets/create-report-page.png)

   然而， **[!UICONTROL 連結共用報表]** 只需要標題、說明和日期範圍引數。

   ![](assets/create-link-share-report.png)

   >[!NOTE]
   >
   >報告標題中的特殊字元#和%在報告產生時會被連字型大小(-)取代。

1. 點選/按一下 **[!UICONTROL 下一個]**，以設定下載、到期和發佈報告的欄。
1. 視需要選取或取消選取適當的核取方塊。 例如，若要檢視使用者（已下載資產）的名稱，請 **[!UICONTROL 下載]** 報表，選取 **[!UICONTROL 下載者]**. 下圖說明如何在「下載」報表中選取預設欄。

   ![](assets/createdownloadreport.png)

   您也可以新增自訂欄到這些報表，以顯示更多符合自訂需求的資料。

   若要新增自訂欄至下載、發佈或到期報告，請遵循下列步驟：

   1. 若要顯示自訂欄，請點選/按一下 **[!UICONTROL 新增]** 範圍 [!UICONTROL 自訂欄].
   1. 在中指定資料行名稱 **[!UICONTROL 欄名稱]** 欄位。
   1. 使用屬性選擇器，選取欄需要對應的屬性。

      ![](assets/property-picker.png)
或者，在屬性路徑欄位中輸入路徑。

      ![](assets/property-path.png)

      若要新增更多自訂欄，請點選/按一下 **新增** 並重複步驟2和3。

1. 点按/单击&#x200B;**[!UICONTROL 创建]**。訊息會通知已開始產生報表。

## 下載報表 {#download-reports}

若要將報表儲存並下載為.csv檔案，請執行下列任一項作業：

* 在「資產報表」頁面上選取報表，然後點選/按一下 **[!UICONTROL 下載]** 從頂端的工具列開啟。

![](assets/download-asset-report.png)

* 從「資產報表」頁面，開啟報表。 選取 **[!UICONTROL 下載]** 報表頁面頂端的選項。

![](assets/download-report-fromwithin.png)

## 刪除報告 {#delete-reports}

若要刪除現有報表，請從下列位置選取報表： **[!UICONTROL 資產報表]** 頁面並點選/按一下 **[!UICONTROL 刪除]** 從頂端的工具列開啟。

>[!NOTE]
>
>**[!UICONTROL 使用狀況]** 無法刪除報告。
