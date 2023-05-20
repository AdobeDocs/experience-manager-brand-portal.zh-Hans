---
title: 应用图像预设或动态演绎版
seo-title: Apply image presets or dynamic renditions
description: 像巨集一樣，影像預設集是預先定義的名稱下儲存的調整大小和格式指令集合。 影像預設集可讓Experience Manager Assets Brand Portal動態傳送不同大小、格式和屬性的影像。
seo-description: Like a macro, an image preset is a predefined collection of sizing and formatting commands saved under a name. Image presets enable Experience Manager Assets Brand Portal to dynamically deliver images of different sizes, formats, and properties.
uuid: a3c8705c-5fbd-472c-8b61-f65b3e552c1b
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: a512dfa0-fef3-4c3f-a389-a0a3a7415bac
role: Admin
exl-id: 212a1b3a-686f-4250-be06-b679b6039887
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '814'
ht-degree: 3%

---

# 应用图像预设或动态演绎版 {#apply-image-presets-or-dynamic-renditions}

像巨集一樣，影像預設集是預先定義的名稱下儲存的調整大小和格式指令集合。 影像預設集可讓Experience Manager Assets Brand Portal動態傳送不同大小、格式和屬性的影像。

影像預設集可用來產生影像的動態轉譯，且可供預覽和下載。 預覽影像及其轉譯時，您可以選擇預設集，將影像重新格式化為符合管理員所設定的規格。

(*如果Experience Manager Assets編寫執行個體執行於&#x200B;**Dynamic Media混合模式***)若要在Brand Portal中檢視資產的動態轉譯，請確定其金字塔tiff轉譯存在於您發佈至Brand Portal的Experience Manager Assets作者執行個體。 當您發佈資產時，其PTIFF轉譯也會發佈至Brand Portal。

>[!NOTE]
>
>下載影像及其轉譯時，無法從現有預設集進行選擇。 您可以改為指定自訂影像預設集的屬性。 如需詳細資訊，請參閱 [下載影像時套用影像預設集](../using/brand-portal-image-presets.md#main-pars-text-1403412644).


如需建立影像預設集時所需引數的詳細資訊，請參閱 [管理影像預設集](../using/brand-portal-image-presets.md).

## 建立影像預設集 {#create-an-image-preset}

Experience Manager Assets管理員可建立影像預設集，在資產詳細資訊頁面上顯示為動態轉譯。 您可以從頭開始建立影像預設集，或使用新名稱儲存現有影像預設集。 建立影像預設集時，請選擇影像傳送的大小和格式命令。 當傳送影像供檢視時，會根據選取的指令最佳化其外觀。

>[!NOTE]
>
>影像的動態轉譯是使用其「金字塔」TIFF建立的。 如果金字塔TIFF不適用於任何資產，則無法在Brand Portal中擷取該資產的動態轉譯。
>
>如果Experience Manager Assets編寫執行個體執行於 **Dynamic Media混合模式**，接著影像資產的金字塔TIFF轉譯專案就會建立並儲存在Experience Manager Assets存放庫中。
>
>然而，如果Experience Manager Assets編寫執行個體執行於 **Dynamic Media Scene 7模式**，則Scene 7伺服器上存在影像資產的金字塔TIFF轉譯。
>
>將這類資產發佈至Brand Portal時，會套用影像預設集並顯示動態轉譯。


1. 從頂端的工具列中，按一下Experience Manager標誌以存取管理工具。

1. 在管理工具面板中，按一下 **[!UICONTROL 影像預設集]**.

   ![](assets/admin-tools-panel-4.png)

1. 在影像預設集頁面中，按一下 **[!UICONTROL 建立]**.

   ![](assets/image_preset_homepage.png)

1. 在 **[!UICONTROL 編輯影像預設集]** 頁面，將值輸入至 **[!UICONTROL 基本]** 和 **[!UICONTROL 進階]** 適當標籤，包括名稱。 预设显示在左窗格中，并可以与其他资产一起动态使用。

   ![](assets/image_preset_create.png)

   >[!NOTE]
   >
   >您也可以使用 **[!UICONTROL 編輯影像預設集]** 頁面，以編輯現有影像預設集的屬性。 若要編輯影像預設集，請從影像預設集頁面中選取它，然後按一下 **[!UICONTROL 編輯]**.

1. 单击“**[!UICONTROL 保存]**”。影像預設集隨即建立並顯示在影像預設集頁面上。
1. 若要刪除影像預設集，請從影像預設集頁面中選取它，然後按一下 **[!UICONTROL 刪除]**. 在確認頁面中，按一下 **[!UICONTROL 刪除]** 以確認刪除。 影像預設集會從影像預設集頁面中移除。

## 預覽影像時套用影像預設集  {#apply-image-presets-when-previewing-images}

預覽影像及其轉譯時，請從現有的預設集中選擇，將影像重新格式化為管理員設定的規格。

1. 在Brand Portal介面中，按一下影像以開啟。
1. 按一下左側的覆蓋圖示，然後選擇 **[!UICONTROL 轉譯]**.

   ![](assets/image-preset-previewrenditions.png)

1. 從 **[!UICONTROL 轉譯]** 清單中，選取適當的動態轉譯，例如， **[!UICONTROL 縮圖]**. 預覽影像會根據您選擇的轉譯進行轉譯。

   ![](assets/image-preset-previewrenditionthumbnail.png)

## 下載影像時套用影像預設集 {#apply-image-presets-when-downloading-images}

從Brand Portal下載影像及其轉譯時，您無法從現有的影像預設集中選擇。 不過，您可以根據要重新格式化影像的來源來自訂影像預設集屬性。

1. 從Brand Portal介面，執行下列任一項作業：

   * 將指標暫留在您要下載的影像上。 在可用的快速動作縮圖中，按一下 **[!UICONTROL 下載]** 圖示。

   ![](assets/downloadsingleasset.png)

   * 選取您要下載的影像。 在頂端的工具列中，按一下 **[!UICONTROL 下載]** 圖示。

   ![](assets/downloadassets.png)

1. 從 **[!UICONTROL 下載]** 對話方塊，請根據您是否要下載資產及其轉譯，選取所需的選項。

   ![](assets/donload-assets-dialog.png)

1. 若要下載資產的動態轉譯，請選取 **[!UICONTROL 動態轉譯]** 選項。
1. 根據您要在下載期間動態重新格式化影像及其轉譯的方式，自訂影像預設集屬性。 指定大小、格式、色域、解析度和影像修飾元。

   ![](assets/dynamicrenditions.png)

1. 单击&#x200B;**[!UICONTROL 下载]**。自訂動態轉譯會下載為ZIP檔案，連同您選擇下載的影像和轉譯。 不過，如果下載單一資產，則不會建立任何zip檔案，這可確保快速下載。
