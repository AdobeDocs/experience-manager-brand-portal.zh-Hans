---
title: Experience Manager Assets Brand Portal概觀
seo-title: Overview of Experience Manager Assets Brand Portal
description: Experience Manager Assets Brand Portal可協助您輕鬆取得、控制核准的創意資產，並安全地將其散佈給跨裝置的外部團體和內部業務使用者。
seo-description: Experience Manager Assets Brand Portal can help you easily acquire, control, and securely distribute approved creative assets to external parties and internal business users across devices.
uuid: b1e54d03-eb2e-488e-af4d-bae817dd135a
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: introduction
discoiquuid: 6aefa298-4728-4b8e-a85b-e419ee37f2f4
exl-id: 0f2c45e4-416e-451a-905b-06c5e42a9272
source-git-commit: fb2ce4d39fd9e7aa69ba541bd48a6b9cddd3b4c5
workflow-type: tm+mt
source-wordcount: '1576'
ht-degree: 6%

---

# Experience Manager Assets Brand Portal概觀 {#overview-of-aem-assets-brand-portal}

作為行銷人員，您有時需要與通路合作夥伴和內部業務使用者共同作業，以快速建立、管理相關數位內容並將其提供給客戶。 在整個客戶歷程中及時傳送相關內容，對於推動更多需求、轉換、參與和客戶忠誠度至關重要。

然而，開發解決方案以支援與延伸的內部團隊、合作夥伴和經銷商有效且安全地共用核准的品牌標誌、指導方針、行銷活動資產或產品快照是一項挑戰。

**Adobe Experience Manager (AEM) Assets Brand Portal** 專注於行銷人員需求，透過提供資產分配和資產貢獻功能，與分散於全球的Brand Portal使用者有效合作。

資產散佈可讓您輕鬆取得、控制核准的創意資產，並安全地將其散佈至跨裝置的外部團體和內部業務使用者。 而Asset Contribution可讓Brand Portal使用者將資產上傳到Brand Portal並發佈到Experience Manager Assets，而無需存取作者環境。 「貢獻」功能的名稱為 **Brand Portal中的資產來源**. 此外，整合可改善資產散佈的整體Brand Portal體驗，以及Brand Portal使用者（外部機構/團隊）的貢獻，加速資產的上市時間，並降低不合規和未經授權存取的風險。
請參閱， [Brand Portal中的Asset Sourcing](brand-portal-asset-sourcing.md).

瀏覽器式入口網站環境可讓您輕鬆上傳、瀏覽、搜尋、預覽和匯出已核准格式的資產。

## 使用 Brand Portal 配置 Experience Manager Assets {#configure-brand-portal}

透過Brand Portal設定Adobe Experience Manager Assets可為Brand Portal使用者啟用資產發佈、資產發佈和資產貢獻功能。

>[!NOTE]
>
>Experience Manager Assetsas a Cloud Service、Experience Manager Assets 6.3及更高版本支援使用Brand Portal設定Experience Manager Assets。

從Cloud Manager啟動Experience Manager Assets，即可使用Brand Portal自動設定Brand Portalas a Cloud Service。 啟動工作流程會在後端建立所需的設定，並在與Experience Manager Assetsas a Cloud Service執行個體相同的IMS組織上啟動Brand Portal。

然而，Experience Manager Assets （內部部署和Managed Service）是使用Brand Portal手動設定Adobe Developer主控台，這會取得AdobeIdentity Management Services (IMS) Token以授權Brand Portal租使用者。

如需詳細資訊，請參閱 [使用Brand Portal設定Experience Manager Assets](../using/configure-aem-assets-with-brand-portal.md).

## Brand Portal中的使用者角色 {#Personas}

Brand Portal支援下列使用者角色：

* 訪客使用者
* 查看者
* 编辑器
* 管理员

下表列出具有這些角色的使用者可以執行的工作：

|  | **浏览** | **搜索** | **下载** | **共享文件夹** | **共享收藏集** | **以链接方式共享资产** | **存取管理工具** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **訪客使用者** | ✓ (A)* | ✓* | ✓* | x | x | x | x |
| **查看者** | ✓ | ✓ | ✓ | x | x | x | x |
| **编辑器** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | x |
| **管理员** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |

>[!NOTE]
>
>訪客使用者只能瀏覽、存取和搜尋公用資料夾和集合中的資產。

<!--
&#42; Viewer users can access and download the public assets shared with them, and can add these assets to create their own collections.

>[!NOTE]
>
>There is a known issue that the share link for collections is currently visible to the viewer users. The viewer users does not have the privilege to add users to create a share link. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.
-->

### 訪客使用者 {#guest-user}

Experience Manager Assets Brand Portal允許 [訪客存取](#request-access-to-brand-portal) 至Brand Portal。 訪客使用者不需要認證即可進入入口網站，且可存取公用資料夾和集合。 身為來賓使用者，您可以瀏覽資產詳細資訊，並擁有公用資料夾和集合成員的完整資產檢視。 您可以搜尋、下載公開資產，並將其新增至 [!UICONTROL Lightbox] 集合。

不過，訪客工作階段會限制您建立收藏集和已儲存的搜尋，並進一步共用它們。 來賓工作階段中的使用者無法存取資料夾和集合設定，也無法以連結形式共用資產。 以下是訪客使用者可以執行的工作清單：

* [瀏覽及存取公用資產](browse-assets-brand-portal.md)

* [搜尋公用資產](brand-portal-searching.md)

* [下載公開資產](brand-portal-download-assets.md)

* [將資產新增至 [!UICONTROL Lightbox]](brand-portal-light-box.md#add-assets-to-lightbox)

如需詳細資訊，請參閱 [訪客存取Brand Portal](../using/guest-access.md).

### 查看者 {#viewer}

Brand Portal使用者定義於 [!DNL Admin Console] 以檢視器角色存取Brand Portal的使用者。 具有此角色的使用者可以登入Brand Portal並存取允許的資料夾、集合和資產。 使用者也可以瀏覽、預覽、下載和匯出資產（原始或特定轉譯）、設定帳戶設定和搜尋資產。 以下是檢視器可以執行的工作清單：

* [瀏覽資產](browse-assets-brand-portal.md)

* [搜尋資產](brand-portal-searching.md)

* [下载资源](brand-portal-download-assets.md)

### 编辑器 {#editor}

具有編輯者角色的使用者可以執行檢視器可以執行的所有工作。 此外，和Editor可以檢視管理員共用的檔案和資料夾。 具有編輯者角色的使用者也可以與其他人共用內容（檔案、資料夾、集合）。

除了檢視器可以執行的工作之外，編輯者還可以執行下列其他工作：

* [共享文件夹](brand-portal-sharing-folders.md)

* [共享收藏集](brand-portal-share-collection.md)

* [以链接方式共享资产](brand-portal-link-share.md)

### 管理员 {#administrator}

管理員包括中標籤為系統管理員或Brand Portal產品管理員的使用者 [!UICONTROL Admin Console]. 管理員可以新增和移除系統管理員和使用者、定義預設集、傳送電子郵件給使用者，以及檢視入口網站使用情況和儲存空間報告。

>[!NOTE]
>
>在Brand Portal中，在中標籤為支援管理員的使用者 [!UICONTROL Admin Console] 具有與系統管理員相同的許可權。

管理員可以執行編輯者可以執行的所有工作。 以下是管理員可以執行的其他工作：

* [管理用户、组和用户角色](brand-portal-adding-users.md)

* [自訂壁紙、頁面標題和電子郵件](brand-portal-branding.md)

* [使用自定义搜索 Facet](brand-portal-search-facets.md)

* [使用元数据架构表单](brand-portal-metadata-schemas.md)

* [应用图像预设或动态演绎版](brand-portal-image-presets.md)

* [使用报告](brand-portal-reports.md)

除了上述工作之外，AEM Assets中的作者還可以執行下列工作：

* [使用 Brand Portal 配置 AEM Assets](../using/configure-aem-assets-with-brand-portal.md)

* [将文件夹发布到 Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/brand-portal-publish-folder.html)

* [将收藏集发布到 Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/brand-portal-publish-collection.html)

## Brand Portal URL的替代別名 {#tenant-alias-for-portal-url}

Brand Portal 6.4.3以後，組織可以有一個替代（別名） URL用於其Brand Portal租使用者的現有URL。 別名URL可在URL中使用替代首碼來建立。\
請注意，您只能自訂Brand Portal URL的前置詞，而不能自訂整個URL。 例如，擁有現有網域的組織 `geomettrix.brand-portal.adobe.com` 可以取得 `geomettrixinc.brand-portal.adobe.com` 已依要求建立。

不過，AEM作者例項可以 [已設定](../using/configure-aem-assets-with-brand-portal.md) 僅使用租使用者ID URL，而不使用租使用者別名（替代） URL。

>[!NOTE]
>
>若要在現有入口網站URL中取得租使用者名稱稱的別名，組織需要透過新的租使用者別名建立請求聯絡客戶支援。 系統會先檢查別名是否可用，然後建立別名，以處理此請求。
>
>若要取代舊別名或刪除舊別名，必須遵循相同的程式。

## 要求存取Brand Portal {#request-access-to-brand-portal}

使用者可從登入畫面要求存取Brand Portal。 這些請求會傳送給Brand Portal管理員，由管理員透過Adobe授予使用者存取權 [!UICONTROL Admin Console]. 授予存取權後，使用者會收到通知電子郵件。

若要要求存取權，請執行下列動作：

1. 從Brand Portal登入頁面中，選取 **[!UICONTROL 按一下這裡]** 對應至 **[!UICONTROL 需要存取權？]**. 不過，若要進入來賓工作階段，請選取 **[!UICONTROL 按一下這裡]** 對應至 **[!UICONTROL 訪客存取？]**.

   ![Brand Portal登入畫面](assets/bp-login-requestaccess.png)

   此 [!UICONTROL 要求存取權] 頁面隨即開啟。

1. 若要請求存取組織的Brand Portal，您必須具備有效的 [!UICONTROL Adobe ID]， [!UICONTROL Enterprise ID]，或 [!UICONTROL Federated ID].

   在 [!UICONTROL 要求存取權] 頁面，使用您的ID登入（案例1）或建立 [!UICONTROL Adobe ID] （案例2）：

   ![[!UICONTROL 要求存取權]](assets/bplogin_request_access_2.png)

   **案例1**

   1. 如果您擁有 [!UICONTROL Adobe ID]， [!UICONTROL Enterprise ID]，或 [!UICONTROL Federated ID]，按一下 **[!UICONTROL 登入]**.
此 [!UICONTROL 登入] 頁面隨即開啟。

   1. 提供您的 [!UICONTROL Adobe ID] 認證，然後按一下 **[!UICONTROL 登入]**.

      ![Adobe登入](assets/bplogin_request_access_3.png)
   系統會將您重新導向至 [!UICONTROL 要求存取權] 頁面。

   **案例2**

   1. 如果您沒有 [!UICONTROL Adobe ID]，若要建立一個，請按一下 **[!UICONTROL 取得Adobe ID]** 從 [!UICONTROL 要求存取權] 頁面。
此 [!UICONTROL 登入] 頁面隨即開啟。
   1. 按一下 **[!UICONTROL 取得Adobe ID]**.
此 [!UICONTROL 註冊] 頁面隨即開啟。
   1. 輸入您的名字和姓氏、電子郵件ID和密碼。
   1. 選取 **[!UICONTROL 註冊]**.

      ![](assets/bplogin_request_access_5.png)
   系統會將您重新導向至 [!UICONTROL 要求存取權] 頁面。

1. 下一頁會顯示您用來要求存取權的名稱和電子郵件ID。 為管理員留下註解，然後按一下 **[!UICONTROL 提交]**.

   ![](assets/bplogin-request-access.png)

## 產品管理員授予存取權 {#grant-access-to-brand-portal}

Brand Portal產品管理員會在其Brand Portal通知區域及收件匣中的電子郵件接收存取要求。

![存取要求的通知](assets/bplogin_request_access_7.png)

若要授與存取權，產品管理員需要按一下Brand Portal通知區域中的相關通知，然後按一下 **[!UICONTROL 授予存取權]**.
或者，產品管理員也可以按照存取要求電子郵件中提供的連結來瀏覽Adobe [!UICONTROL Admin Console] 並將使用者新增至相關的產品設定。

系統會將您重新導向至 [Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) 首頁。 使用Adobe [!UICONTROL Admin Console] 以建立使用者並將其指派給產品設定檔（先前稱為產品設定），在Brand Portal中顯示為群組。 如需在中新增使用者的詳細資訊 [!UICONTROL Admin Console]，請參閱 [新增使用者](brand-portal-adding-users.md#add-a-user) （請依照程式中的步驟4-7新增使用者）。

## Brand Portal語言 {#brand-portal-language}

您可以從Adobe變更Brand Portal語言 [!UICONTROL Experience Cloud設定].

![存取要求的通知](assets/BPLang.png)

若要變更語言：

1. 選取 [!UICONTROL 使用者] > [!UICONTROL 編輯設定檔] 從頂端功能表。

   ![编辑个人资料](assets/EditBPProfile.png)

1. 開啟 [!UICONTROL Experience Cloud設定] 頁面，從中選擇語言 [!UICONTROL 語言] 下拉式功能表。

## Brand Portal維護通知 {#brand-portal-maintenance-notification}

Brand Portal在排程進行維護前會先在您登入Brand Portal後，通知會顯示為橫幅。 範例通知：

![](assets/bp_maintenance_notification.png)

您可以關閉此通知，並繼續使用Brand Portal。 此通知會出現在每個新工作階段中。

## 版本和系統資訊 {#release-and-system-information}

* [新增功能](whats-new.md)
* [发行说明](brand-portal-release-notes.md)
* [支持的文件格式](brand-portal-supported-formats.md)

## 相關資源 {#related-resources}

<!--
* [Adobe Customer Support]()
-->

* [AEM論壇](https://experienceleaguecommunities.adobe.com/t5/adobe-experience-manager/ct-p/adobe-experience-manager-community)
