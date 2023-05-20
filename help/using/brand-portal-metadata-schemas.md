---
title: 使用元数据架构表单
seo-title: Use the metadata schema form
description: 中繼資料結構描述會說明「屬性」頁面的配置，以及針對使用特定結構描述的資產所顯示的中繼資料屬性。 您套用至資產的結構描述會決定出現在其「屬性」頁面上的中繼資料欄位。
seo-description: A metadata schema describes the layout of the Properties page and the metadata properties displayed for assets that use the particular schema. The schema that you apply to an asset determines the metadata fields that appear on its Properties page.
uuid: 1a944a3b-5152-425f-b1ea-bfe3331de928
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: administration
discoiquuid: 500b46da-ef67-46a0-a069-192f4b1a0eca
role: Admin
exl-id: fbedff90-a6cb-4175-8308-817cc9f5b450
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '1718'
ht-degree: 10%

---

# 使用元数据架构表单 {#use-the-metadata-schema-form}

中繼資料結構描述會說明「屬性」頁面的配置，以及針對使用特定結構描述的資產所顯示的中繼資料屬性。 您套用至資產的結構描述會決定出現在其「屬性」頁面上的中繼資料欄位。

此 **[!UICONTROL 屬性]** 每個資產的頁面包含預設中繼資料屬性，具體取決於資產的MIME型別。 管理員可以使用中繼資料結構編輯器來修改現有結構或新增自訂中繼資料結構。 Experience Manager Assets Brand Portal為各種MIME型別的資產提供預設表單。 不過，您也可以為這類資產新增自訂表單。

## 新增中繼資料結構表單 {#add-a-metadata-schema-form}

若要建立新的中繼資料結構表單，請執行下列動作：

1. 從頂端的工具列中，按一下Experience Manager標誌以存取管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，按一下 **[!UICONTROL 中繼資料結構]**.

   ![](assets/navigation-panel.png)

1. 於 **[!UICONTROL 中繼資料結構Forms]** 頁面，按一下 **[!UICONTROL 建立]**.

   ![](assets/create-metadata-schema-form.png)

1. 在 **[!UICONTROL 建立結構表單]** 對話方塊中，指定「架構」表單的標題，然後按一下 **[!UICONTROL 建立]** 以完成表單建立程式。

   ![](assets/create-schema-form.png)

## 編輯中繼資料結構表單 {#edit-a-metadata-schema-form}

您可以編輯新新增或現有的中繼資料結構表單。 中繼資料結構表單包含衍生自其父項的內容，包括索引標籤和索引標籤內的表單專案。 您可以將這些表單專案對應或設定至中繼資料節點內的欄位。

您可以將新標籤或表單專案新增到中繼資料結構表單。 衍生的標籤和表單專案（來自父項）處於鎖定狀態。 您無法在子層級變更它們。

若要編輯中繼資料結構表單，請執行下列動作：

1. 從頂端的工具列中，按一下Experience Manager標誌以存取管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，按一下 **[!UICONTROL 中繼資料結構]**.
1. 從 **[!UICONTROL 中繼資料結構Forms]** 頁面中，選取要編輯其屬性的綱要表單，例如， **[!UICONTROL 集合]**.

   ![](assets/metadata-schema-forms.png)

   >[!NOTE]
   >
   >未編輯的範本會在它們之前顯示鎖定符號。 如果您自訂任何範本，則範本前的「鎖定」符號會消失。

1. 在頂端的工具列中，按一下 **[!UICONTROL 編輯]**.

   此 **[!UICONTROL 中繼資料結構編輯器]** 頁面開啟，其中包含 **[!UICONTROL 基本]** 標籤在左側開啟，然後 **[!UICONTROL 建置表單]** 標籤在右側開啟。

1. 在 **[!UICONTROL 中繼資料結構編輯器]** 頁面，自訂 **[!UICONTROL 屬性]** 頁面（透過從中的元件型別清單拖曳一個或多個元件） **[!UICONTROL 建置表單]** 按Tab鍵至 **[!UICONTROL 基本]** 標籤。

   ![](assets/metadata-schemaeditor-page.png)

1. 若要設定元件，請選取該元件，並在下列位置修改其屬性： **[!UICONTROL 設定]** 標籤。

### 「建置表單」標籤中的元件 {#components-in-the-build-form-tab}

此 **[!UICONTROL 建置表單]** 索引標籤會列出可在結構描述表單中使用的專案。 此 **[!UICONTROL 設定]** 索引標籤會提供您在「 」中選取的每個專案的屬性。 **[!UICONTROL 建置表單]** 標籤。 下表列出 **[!UICONTROL 建置表單]** 標籤：

| 元件名稱 | 描述 |
|---------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **[!UICONTROL 章节标题]** | 為常見元件清單新增區段標題。 |
| **[!UICONTROL 单行文本]** | 新增單行文字屬性。 它會儲存為字串。 |
| **[!UICONTROL 多值文字]** | 新增多值文字屬性。 它會儲存為字串陣列。 |
| **[!UICONTROL 数字]** | 新增數字元件。 |
| **[!UICONTROL 日期]** | 新增日期元件。 |
| **[!UICONTROL 下拉列表]** | 新增下拉式清單。 |
| **[!UICONTROL 标准标记]** | 添加标记. **注意：** 管理員可能需要變更路徑值，例如 `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`，如果他們從Experience Manager Assets發佈中繼資料結構表單，其中路徑不包含租使用者資訊，例如 `/etc/tags/<custom_tag_namespace>`. |
| **[!UICONTROL 智能标记]** | 自動偵測標籤(如果您已購買並設定Experience Manager Assets智慧標籤附加元件)。 |
| **[!UICONTROL 隐藏字段]** | 新增隱藏欄位。 儲存資產時，這會傳送為POST引數。 |
| **[!UICONTROL 资产引用对象]** | 新增此元件以檢視資產所參考的資產清單。 |
| **[!UICONTROL 资产引用]** | 新增以顯示參照資產的資產清單。 |
| **[!UICONTROL 资产评级]** | 在資產發佈至Brand Portal之前，從Experience Manager Assets新增資產的平均評分。 |
| **[!UICONTROL 上下文元数据]** | 新增以控制其他中繼資料索引標籤在資產屬性頁面的顯示。 |

>[!NOTE]
>
>不要使用 **[!UICONTROL 產品引用]**，因為它無法運作。

#### 編輯中繼資料元件 {#edit-the-metadata-component}

若要編輯表單上中繼資料元件的屬性，請按一下該元件，然後在 **[!UICONTROL 設定]** 標籤。

* **[!UICONTROL 欄位標籤]**：在資產的「屬性」頁面上顯示的中繼資料屬性名稱。

* **[!UICONTROL 對應至屬性]**：此屬性的值會提供資產節點的相對路徑/名稱，該資產節點會儲存在CRX存放庫中。 開頭是&quot;**./**」是因為，表示路徑在資產的節點下。

以下是此屬性的有效值：

— `./jcr:content/metadata/dc:title`：將值儲存在資產的中繼資料節點，做為屬性 [!UICONTROL `dc:title`].

— `./jcr:created`：在資產的節點顯示jcr屬性。 如果您在视图属性上配置这些属性，我们建议您将这些属性标记为“禁用编辑”，因为它们是受保护属性。否则，在保存资产的属性时，会出现“资产修改失败”错误。

* **[!UICONTROL 預留位置]**：使用此屬性可向使用者提供有關中繼資料屬性的任何相關資訊。
* **[!UICONTROL 必填]**：使用此屬性可將中繼資料屬性標示為「屬性」頁面上的必要屬性。
* **[!UICONTROL 停用編輯]**：使用此屬性可讓中繼資料屬性在「屬性」頁面上無法編輯。
* **[!UICONTROL 以唯讀方式顯示空白欄位]**：標示此屬性以在「屬性」頁面上顯示中繼資料屬性，即使該屬性沒有值亦然。 根據預設，當中繼資料屬性沒有值時，它不會列在屬性頁面上。
* **[!UICONTROL 說明]**：使用此屬性為中繼資料元件新增簡短說明。
* **[!UICONTROL 「刪除」圖示]**：按一下此圖示可從結構表單中刪除元件。

![](assets/delete_icon_editmetadataschemaform.png)

>[!NOTE]
>
>資產的中繼資料編輯器表單中的所有中繼資料欄位都是唯讀的。 由於資產的中繼資料必須先在Experience Manager Assets中編輯，資產才會發佈至Brand Portal。

#### 在結構表單中新增或刪除索引標籤 {#add-or-delete-a-tab-in-the-schema-form}

預設結構表單包括 **[!UICONTROL 基本]** 和 **[!UICONTROL 進階]** 索引標籤。 通过架构编辑器，可以添加或删除选项卡。

![](assets/add_delete_tabs_metadataschemaform.png)

* 若要在結構表單上新增索引標籤，請按一下 **[!UICONTROL +]**. 依預設，新索引標籤的名稱為「Unnamed-1」。 您可以修改名稱，從 **[!UICONTROL 設定]** 標籤。

![](assets/add-tab-metadata-form.png)

* 若要刪除標籤，請按一下 **[!UICONTROL x]**. 按一下 **[!UICONTROL 儲存]** 以儲存變更。

## 將中繼資料結構描述套用至資料夾 {#apply-a-metadata-schema-to-a-folder}

Brand Portal可讓您自訂和控制中繼資料結構，以便 **[!UICONTROL 屬性]** 資產的頁面只會顯示您選擇顯示的特定資訊。 若要控制在中顯示的中繼資料 **[!UICONTROL 屬性]** 頁面，從中繼資料結構表單中移除所需的中繼資料，並將其套用至特定資料夾。

若要將中繼資料結構表單套用至資料夾，請執行下列動作：

1. 從頂端的工具列中，按一下Experience Manager標誌以存取管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，按一下 **[!UICONTROL 中繼資料結構]**.

1. 從 **[!UICONTROL 中繼資料結構Forms]** 頁面上，選取您要套用至資產的結構描述表單，例如， **[!UICONTROL 服裝]**.

   ![](assets/apply-metadata-schema-form-to-folder.png)

1. 在頂端的工具列中，按一下 **[!UICONTROL 套用至資料夾]**.

1. 從 **[!UICONTROL 選取資料夾]** 頁面上，導覽至您要套用的資料夾。 **[!UICONTROL 服裝]** 中繼資料結構，例如， **[!UICONTROL 手套]**.

   ![](assets/apply_metadata_schemaformtofoldergloves.png)

1. 按一下 **[!UICONTROL 套用]** 將中繼資料結構表單套用至資料夾。

   中可用的中繼資料 **[!UICONTROL 服裝]** 中繼資料結構表單已套用至 **[!UICONTROL 手套]** 資料夾並顯示在 **[!UICONTROL 屬性]** 檔案夾的頁面。

   ![](assets/folder_metadata_properties.png)

>[!NOTE]
>
>如果您將包含巢狀結構描述的結構描述套用至包含視訊檔案的資料夾，視訊檔案的中繼資料屬性可能無法正確呈現。 為確保中繼資料屬性正確呈現，請移除巢狀結構描述，並僅將父結構描述套用至資料夾。

## 刪除中繼資料結構表單 {#delete-a-metadata-schema-form}

Brand Portal僅可讓您刪除自訂結構表單。 它不允許您刪除預設結構表單/範本。 不過，您可以刪除這些表單中的任何自訂變更。

若要刪除表單，請選取表單並按一下 **[!UICONTROL 刪除]** 圖示。

![](assets/delete_icon_metadataschemaeditorform.png)

>[!NOTE]
>
>刪除對預設表單進行的自訂變更後， **[!UICONTROL 鎖定]** 符號會重新出現在中繼資料結構介面的表單名稱前，以表示表單已恢復為預設狀態。

## MIME型別的結構表單 {#schema-forms-for-mime-types}

### 為MIME型別新增表單 {#adding-new-forms-for-mime-types}

除了預設表單之外，您還可以為各種MIME型別的資產新增自訂表單，或在適當的表單型別下建立新表單。 例如，要为 **[!UICONTROL image/png]** 子类型添加新模板，请在“image”表单下创建表单。架构表单的标题是子类型名称。在此範例中，標題為&quot;png&quot;。

#### 針對各種MIME型別使用現有結構描述範本 {#using-an-existing-schema-template-for-various-mime-types}

您可以將現有範本用於不同的MIME型別。 例如，使用 **image/jpeg** MIME型別資產的表單 **image/png**.

在此情況下，請在以下位置建立新節點： [!UICONTROL `/etc/dam/metadataeditor/mimetypemappings`] 在CRX存放庫中。 指定節點名稱並定義下列屬性：

| **名称** | **类型** | **值** |
|---|---|---|
| exposedmimetype | 字符串 | image/jpeg |
| mimetypes | 字符串[] | image/png |

* **exposedmimetype**：要對應的現有表單名稱
* **mimetypes**：使用中定義之表單的MIME型別清單 **exposedmimetype** 屬性

Brand Portal對應下列MIME型別和結構表單：

| **結構表單** | **MIME型別** |
|---|---|
| image/jpeg | image/pjpeg |
| image/tiff | image/x-tiff |
| application/pdf | application/postscript |
| application/x-ImageSet | Multipart/Related; type=application/x-ImageSet |
| application/x-SpinSet | Multipart/Related; type=application/x-SpinSet |
| application/x-MixedMediaSet | Multipart/Related; type=application/x-MixedMediaSet |
| video/quicktime | video/x-quicktime |
| video/mpeg4 | video/mp4 |
| video/avi | video/avi， video/msvideo， video/x-msvideo |
| video/wmv | video/x-ms-wmv |
| video/flv | video/x-flv |

以下是預設中繼資料屬性的清單：

* jcr:content/metadata/cq:tags
* jcr:content/metadata/dc:format
* jcr:content/metadata/dam:status
* jcr：content/metadata/videoCodec
* jcr：content/metadata/audioCodec
* jcr：content/metadata/dc：title
* jcr：content/metadata/dc：description
* jcr：content/metadata/xmpMM：InstanceID
* jcr：content/metadata/xmpMM：DocumentID
* jcr：content/metadata/dam：sha1
* jcr：content/metadata/dam：solutionContext
* jcr：content/metadata/videoBitrate
* jcr：content/metadata/audioBitrate
* jcr：content/usages/usedBy
* jcr:content/jcr:lastModified
* jcr:content/metadata/prism:expirationDate
* jcr：content/onTime
* jcr：content/offTime
* jcr:content/metadata/dam:size
* jcr：content/metadata/tiff：ImageWidth
* jcr：content/metadata/tiff：ImageLength
