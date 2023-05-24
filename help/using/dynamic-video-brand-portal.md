---
title: Brand Portal 上的动态视频支持
seo-title: Dynamic video support on Brand Portal
description: Brand Portal 上的动态视频支持
seo-description: Dynamic video support on Brand Portal
uuid: a3502a4d-3971-4ea4-953c-44ba04446269
contentOwner: mgulati
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: download-install
discoiquuid: e18d992a-a3b5-45f2-9696-8161993213ee
exl-id: 08d6a0fb-061e-4bef-b8e2-bb8522e7482e
source-git-commit: f56918ea8eb14ba04b7e141f4f1cae318e532512
workflow-type: tm+mt
source-wordcount: '1250'
ht-degree: 4%

---

# Brand Portal 上的动态视频支持 {#dynamic-video-support-on-brand-portal}

透過Dynamic Media支援，在Brand Portal上自適應的預覽和播放影片。 您也可以從入口網站和共用連結下載動態轉譯。
Brand Portal使用者可以：

* 在「資產詳細資訊」頁面、「卡片檢視」和連結共用預覽頁面中預覽影片。
* 在資產詳細資訊頁面上播放視訊編碼。
* 在「資產詳細資訊」頁面的「轉譯」索引標籤中檢視動態轉譯。
* 下載視訊編碼和包含視訊的資料夾。

>[!NOTE]
>
>若要使用影片並將影片發佈至Brand Portal，請確定您的Experience Manager作者例項設定在Dynamic Media混合模式或Dynamic Media上 **[!DNL Scene7]** 模式。

若要預覽、播放和下載影片，Brand Portal會向管理員公開下列兩個設定：

* [Dynamic Media混合式設定](#configure-dm-hybrid-settings)
如果Experience Manager作者例項在Dynamic Media混合模式下執行。
* [Dynamic Media [!DNL Scene7] 設定](#configure-dm-scene7-settings)
如果Experience Manager作者例項在Dynamic Media上執行 — **[!DNL Scene7]** 模式。
根據您在Brand Portal租使用者複製的Experience Manager作者執行個體中設定的設定，設定這些設定中的任一個。

>[!NOTE]
>
>Brand Portal租使用者不支援動態視訊，因為設定了Experience Manager Author執行於 **[!UICONTROL Scene7Connect]** 執行模式。

## 如何播放動態影片？ {#how-are-dynamic-videos-played}

![視訊編碼是從雲端擷取](assets/VideoEncodes.png)

如果Dynamic Media設定([混合式](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) 或 [[!DNL Scene7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) Brand Portal設定)，動態轉譯會從 **[!DNL Scene7]** 伺服器。 因此，視訊編碼可以不受延遲和品質扭曲地預覽和播放。

由於視訊編碼不會儲存在Brand Portal存放庫中，而是會從擷取 **[!DNL Scene7]** 伺服器，請確定Adobe Experience Manager編寫執行個體和Brand Portal上的Dynamic Media設定相同。

>[!NOTE]
>
>Brand Portal不支援視訊檢視器和檢視器預設集。 在Brand Portal中的預設檢視器上預覽和播放影片。

## 前提条件 {#prerequisites}

若要在Brand Portal上使用動態影片，請確定：

* **在Dynamic Media模式下啟動Experience Manager作者**
啟動Experience Manager Author例項(已設定Brand Portal)，請於 [DYNAMIC MEDIA - [!DNL Scene7] 模式](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html?lang=en#enabling-dynamic-media-in-scene-mode) 或 [Dynamic Media — 混合模式](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html) 或
* **在Experience Manager作者上設定Dynamic MediaCloud Services**
根據「作者」執行所在的Dynamic Media模式(Scene7Experience Manager模式或混合模式)，設定 [Dynamic MediaCloud Services([!DNL Scene7] 模式)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html?lang=zh-Hans#configuring-dynamic-media-cloud-services) 或 [Dynamic MediaCloud Services（混合模式）](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html?lang=en#configuring-dynamic-media-cloud-services) Experience Manager作者來源 **工具** | **Cloud Services** | **Dynamic Media**.
* **在Brand Portal上設定Dynamic Media**
根據Experience Manager作者的Dynamic Media雲端設定，設定 [Dynamic Media設定](#configure-dm-hybrid-settings) 或 [[!DNL Scene7] 設定](#configure-dm-scene7-settings) 從Brand Portal管理工具。
請確定 [區隔Brand Portal租使用者](#separate-tenants) 用於Dynamic Media中設定的Experience Manager作者執行個體 —  **[!UICONTROL Scene7]** 模式和Dynamic Media — 混合模式。 特別是如果您使用Dynamic Media的功能 **[!UICONTROL S7]** 和Dynamic Media Hybrid。
* **將視訊編碼套用至Brand Portal的發佈資料夾**
套用 [視訊編碼](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) 並將包含多媒體資產的資料夾從Experience Manager製作例項發佈至Brand Portal。
* **SPS中的允許清單輸出IP （如果已啟用安全預覽）**
如果使用Dynamic Media-**[!DNL Scene7]** (含 [已啟用安全預覽](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) （適用於公司），則建議 **[!DNL Scene7]** 公司管理員 [允許列出公用輸出IP](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) 針對個別使用SPS的地區(**[!UICONTROL Scene7]** Publishing System) flash UI。
輸出IP如下：

| **区域** | **輸出IP** |
|--- |--- |
| NA | 130.248.160.68,  20.94.203.130 |
| EMEA | 185.34.189.3,  51.132.146.75 |
| APAC | 63.140.44.54 |

若要將其中一個輸出IP加入允許清單，請參閱 [為安全測試服務準備您的帳戶](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## 最佳实践

若要確保從Brand Portal （和共用連結）成功預覽、播放和下載您的動態視訊資產，請遵循下列作法：

### 區隔Dynamic Media的租使用者 — Scene7和Dynamic Media — 混合模式 {#separate-tenants}

如果您同時使用Dynamic Media - **[!DNL Scene7]** 模式和Dynamic Media — 混合模式功能，針對以Dynamic Media設定的Experience Manager作者執行個體，使用不同的Brand Portal租使用者 —  **[!DNL Scene7]** 和Dynamic Media — 混合模式。


![作者與BP一對應](assets/BPDynamicMedia.png)

### Experience Manager作者執行個體和Brand Portal的設定詳細資料相同

請確定Brand Portal中的設定詳細資料與 **[!UICONTROL Experience Manager雲端設定]**. 相同的設定詳細資料包括：

* **[!UICONTROL 标题]**
* **[!UICONTROL 注册 ID]**
* **[!UICONTROL 視訊服務URL]** 在 **[!UICONTROL Dynamic Media — 混合模式]**
* **[!UICONTROL 标题]**
* 認證(**[!UICONTROL 電子郵件]** 和密碼)
* **[!UICONTROL 区域]**
* **[!UICONTROL 公司]** 在Dynamic Media中 —  **[!DNL Scene7]** 模式

### Dynamic Media Scene7模式的允許清單公開輸出IP

若為Dynamic Media **[!UICONTROL Scene7]** — 具有 [已啟用安全預覽](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) — 用於將視訊資產提供給Brand Portal，然後 **[!UICONTROL Scene7]** 建立專用影像伺服器，用於中繼環境或內部應用程式。 對此伺服器的任何請求都會檢查原始IP位址。 如果傳入的請求不在核准的IP位址清單中，則會傳回失敗回應。
此 **[!UICONTROL Scene7]** 因此，公司管理員會為公司設定核准的IP位址清單， **[!UICONTROL 安全測試]** 環境，透過 **[!UICONTROL SPS]** (Scene7 Publishing System) flash UI。 確保將您個別區域（來自以下區域）的輸出IP新增到該已核准清單。
若要將其中一個輸出IP加入允許清單，請參閱 [為安全測試服務準備您的帳戶](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
輸出IP如下：

| **区域** | **輸出IP** |
|--- |--- |
| NA | 130.248.160.66, 20.94.203.130 |
| EMEA | 51.132.146.75, 130.248.244.202, 130.248.244.203, 130.248.244.204, 130.248.244.210, 130.248.244.211, 130.248.244.212 |
| APAC | 63.140.44.54 |

## 設定Dynamic Media （混合）設定 {#configure-dm-hybrid-settings}

如果Experience Manager作者例項在Dynamic Media混合模式下執行，則使用 **[!UICONTROL 視訊]** 從「管理工具」面板中並排顯示，以設定Dynamic Media閘道設定。

>[!NOTE]
>
>此 [視訊編碼設定檔](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) 不會發佈至Brand Portal，而是會從 **[!UICONTROL Scene7]** 伺服器。 因此，若要在Brand Portal中成功播放視訊編碼，請確定設定詳細資料與 [Dynamic MediaCloud Services([!DNL Scene7] 模式)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html?lang=zh-Hans#configuring-dynamic-media-cloud-services) 在您的Experience Manager作者例項中。

若要在Brand Portal租使用者上設定Dynamic Media設定：

1. 選取Experience Manager標誌，以便您可以從頂端的工具列存取Brand Portal中的管理工具。
1. 從管理工具面板中，選取 **[!UICONTROL 視訊]** 圖磚。

   ![Brand Portal上的Dynamic Media混合式設定](assets/DMHybrid-Video.png)

   **[!UICONTROL 編輯Dynamic Media設定]** 頁面隨即開啟。

   ![Brand Portal上的Dynamic Media混合式設定](assets/edit-dynamic-media-config.png)

1. 指定 **[!UICONTROL 註冊ID]** 和 **[!UICONTROL 視訊服務URL]** （DM閘道URL）。 請確定這些詳細資料與中的詳細資料相同 **[!UICONTROL 「工具」>「Cloud Services」]** 在您的Experience Manager作者例項中。
1. 選取 **儲存** 以儲存設定。

## 配置Dynamic Media Scene7設定 {#configure-dm-scene7-settings}

如果Experience Manager作者執行個體在Dynamic Media上執行 —  **[!UICONTROL Scene7]** 模式，然後使用 **[!UICONTROL Dynamic Media設定]** 從「管理工具」面板中並排顯示，以設定 **[!UICONTROL Scene7]** 伺服器設定。

若要設定Dynamic Media **[!UICONTROL Scene7]** Brand Portal租戶的設定：

1. 選取Experience Manager標誌，以便您可以從頂端的工具列存取Brand Portal中的管理工具。

2. 從管理工具面板中，選取 **[!UICONTROL Dynamic Media設定]** 圖磚。

   ![DM [!UICONTROL Scene 7] 在Brand Portal上設定](assets/DMS7-Tile.png)

   **[!UICONTROL 編輯Dynamic Media設定]** 頁面隨即開啟。

   ![Brand Portal上的Scene 7設定](assets/S7Config.png)

3. 提供：

   * **[!UICONTROL 标题]**
   * 認證(**[!UICONTROL 電子郵件ID]** 和 **[!UICONTROL 密碼]**)以存取Scene7伺服器
   * **[!UICONTROL 区域]**

   請確定這些值與在Experience Manager編寫執行個體中找到的值相同。

4. 選取 **[!UICONTROL 連線至Dynamic Media]**.

5. 提供 **[!UICONTROL 公司名稱]**、和 **[!UICONTROL 儲存]** 設定。
