---
title: 共享文件夹
seo-title: Share folders
description: Brand Portal不支援資產擷取，因此資產必須從預先設定的Experience Manager Assets Author例項發佈至Brand Portal。 Brand Portal的非管理員使用者無法存取已發佈的資產，除非在使用Experience Manager執行個體設定復寫時進行設定，否則需要與他們共用。
seo-description: Brand Portal does not support asset ingestion so assets must be published to Brand Portal from a pre-configured Experience Manager Assets Author instance. Published assets are not accessible to non-admin users of Brand Portal, unless configured while configuring replication with Experience Manager instance, and need to be shared with them.
uuid: 340d0a49-b708-4f0e-9fb8-99c824942f34
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 2332c16f-40be-4673-8cc6-2360d5b74116
exl-id: d28cf927-60e8-437e-9cba-92f7e19020e7
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 2%

---

# 在Brand Portal上共用資料夾 {#share-folders}

資產需要從預先設定的Experience Manager製作例項發佈到Brand Portal，因為Brand Portal不支援資產擷取。

## Brand Portal中的資料夾共用工作流程 {#folder-sharing-workflow-in-brand-portal}

以下說明資料夾共用工作流程和使用者存取權：

* 根據預設，從Experience Manager Assets發佈至Brand Portal的所有資料夾僅對Brand Portal管理員可見，除非在設定復寫時標籤為公開。
* 管理員使用 **[!UICONTROL 資料夾屬性]** 主控台，與選擇性使用者或群組共用資料夾。 只有共用資料夾的使用者或群組，才能在登入Brand Portal後檢視資料夾。 其他使用者看不到該資料夾。
* 管理員也可以選擇透過 **[!UICONTROL 公用資料夾]** 核取方塊 **[!UICONTROL 資料夾屬性]** 主控台。 所有使用者皆可看到公用資料夾。

* 無論使用者角色和許可權為何，當使用者登入Brand Portal時，他們會看到所有公用資料夾，以及直接與他們共用或與其所屬群組共用的資料夾。 所有使用者都無法看見私人資料夾或與其他使用者共用的資料夾。

### 在Brand Portal上與使用者群組共用資料夾 {#sharing-folders-with-user-groups-on-brand-portal}

檔案夾資產的存取權取決於其父檔案夾的存取權，無論子檔案夾的設定為何。 此行為受下列專案管理： [ACL](https://experienceleague.adobe.com/docs/experience-manager-65/administering/security/security.html) 在AEM中，子資料夾繼承父資料夾的ACL。 例如，如果資料夾A包含包含資料夾C的資料夾B，則對資料夾A具有存取許可權的使用者群組（或使用者）也對資料夾B和資料夾C具有相同的存取許可權。資料夾B是A的子資料夾，會繼承其ACL，而資料夾C是B的子資料夾，會繼承其ACL。

同樣地，僅擁有資料夾B存取許可權的使用者群組（或使用者）對資料夾C但不對資料夾A擁有相同的存取許可權。因此，建議組織安排其內容，以便將大多數公開的資產放在子資料夾中，並可限制從子資料夾到根資料夾的存取。

### 公用資料夾發佈 {#public-folder-publish}

除非 **[!UICONTROL 公用資料夾發佈]** 在設定Brand Portal復寫時會選取此選項，但非管理員使用者（例如編輯者和檢視者）無法存取從AEM Assets發佈至Brand Portal的資產。

![](assets/assetbpreplication.png)

如果 **[!UICONTROL 公用資料夾發佈]** 選項已停用，管理員需要使用共用功能明確與非管理員使用者共用這些資產。

>[!NOTE]
>
>要啟用的選項 **[!UICONTROL 公用資料夾發佈]** 可自AEM 6.3.2.1使用。

## 共用資料夾的存取權 {#access-to-shared-folders}

下列矩陣討論各種使用者角色的存取許可權以及共用/取消共用資產的許可權：

|  | 存取從AEM Assets發佈至Brand Portal的所有資料夾 | 共用資料夾的存取權 | 共用/取消共用資料夾許可權 |
|---------------|-----------|-----------|------------|
| 管理员 | 是 | 是 | 是 |
| 编辑器 | 否* | 是，僅當與他們共用或與他們所屬的群組共用時 | 是，僅適用於與其共用或與所屬群組共用的資料夾 |
| 查看者 | 否* | 是，僅當與他們共用或與他們所屬的群組共用時 | 否 |
| 来宾用户 | 否* | 是，僅當與他們共用或與他們所屬的群組共用時 | 否 |

>[!NOTE]
>
>根據預設， **[!UICONTROL 公用資料夾發佈]** 使用AEM Author設定Brand Portal復寫時停用選項。 如果已啟用此選項，則所有使用者（非管理員使用者）預設都能存取發佈至Brand Portal的資料夾。

### 非管理員使用者對共用資料夾的存取權 {#non-admin-user-access-to-shared-folders}

非管理員使用者只能存取他們在Brand Portal上共用的資料夾。 不過，這些資料夾在登入時如何顯示在入口網站上，取決於 **[!UICONTROL 啟用資料夾階層]** 設定。

**如果已停用設定**

非管理員使用者在登入Brand Portal時，會在登陸頁面上看見與其共用的所有資料夾。

![](assets/disabled-folder-hierarchy1-1.png)

**如果已啟用設定**

非管理員使用者在登入Brand Portal時，可看見資料夾樹狀結構（從根資料夾開始）和在各自父資料夾中排列的共用資料夾。

這些父資料夾是虛擬資料夾，無法對它們執行任何動作。 您可以使用鎖定圖示來識別這些虛擬資料夾。

暫留或選取動作任務時未顯示任何動作任務 **[!UICONTROL 卡片檢視]**，不同於共用資料夾。 **[!UICONTROL 概觀]** 選擇中的虛擬資料夾時顯示按鈕 **[!UICONTROL 欄檢視]** 和 **[!UICONTROL 清單檢視]**.

>[!NOTE]
>
>請注意，虛擬資料夾的預設縮圖為第一個共用資料夾的縮圖影像。

![](assets/enabled-hierarchy1-1.png) ![](assets/hierarchy1-nonadmin-1.png) ![](assets/hierarchy-nonadmin-1.png) ![](assets/hierarchy2-nonadmin-1.png)

## 共享文件夹 {#how-to-share-folders}

若要在Brand Portal上和使用者共用資料夾，請執行下列步驟：

1. 按一下左側的覆蓋圖示，然後選擇 **[!UICONTROL 導覽]**.

   ![](assets/selectorrail.png)

1. 從左側的側邊欄中選取 **[!UICONTROL 檔案]**.

   ![](assets/access_files.png)

1. 在Brand Portal介面中，選取您要共用的資料夾。

   ![](assets/share-folders.png)

1. 從頂端的工具列中，選取 **[!UICONTROL 共用]**.

   ![](assets/share_icon.png)

   此 [!UICONTROL 資料夾屬性] 主控台隨即顯示。

   ![](assets/folder_properties.png)

1. 在 **[!UICONTROL 資料夾屬性]** 控制檯中，指定資料夾標題 **[!UICONTROL 資料夾標題]** 欄位。
1. 從 **[!UICONTROL 新增使用者]** 清單，選取您要共用資料夾的使用者或群組，然後按一下 **[!UICONTROL 新增]**.
若要僅與訪客使用者共用資料夾，而不與其他使用者共用，請選取 **[!UICONTROL 匿名使用者]** 從 **[!UICONTROL 成員]** 下拉式清單。

   ![](assets/only-anonymous.png)

   >[!NOTE]
   >
   >若要讓所有使用者都可以使用資料夾，而不論其群組成員資格和角色為何，請選取 **[!UICONTROL 公用資料夾]** 核取方塊。

1. 如有必要，請按一下 **[!UICONTROL 變更縮圖]** 修改資料夾的縮圖影像。
1. 单击“**[!UICONTROL 保存]**”。

1. 若要存取共用資料夾，請使用共用該資料夾的使用者憑證登入Brand Portal。 在介面中檢閱共用資料夾。

## 取消共用資料夾 {#unshare-the-folders}

若要取消共用先前共用的資料夾，請遵循下列步驟：

1. 在Brand Portal介面中，選取您要取消共用的資料夾。

   ![](assets/share-folders-1.png)

1. 在頂端的工具列中，按一下 **[!UICONTROL 共用]**.
1. 在 **[!UICONTROL 資料夾屬性]** 主控台，在 **[!UICONTROL 成員]**，按一下 **[!UICONTROL x]** 符號來將資料夾從共用資料夾的使用者清單中移除。

   ![](assets/folder_propertiesunshare.png)

1. 在警告訊息方塊中，按一下 **[!UICONTROL 確認]** 以確認取消共用。
单击“**[!UICONTROL 保存]**”。

1. 使用您從共用清單中移除之使用者的憑證登入Brand Portal。 使用者的Brand Portal介面中不再提供資料夾。
