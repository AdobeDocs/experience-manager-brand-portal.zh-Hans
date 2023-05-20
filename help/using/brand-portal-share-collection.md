---
title: 共享收藏集
seo-title: Share a collection
description: Experience Manager Assets Brand Portal管理員可與授權使用者共用和取消共用集合或智慧型集合。 編輯人員只能檢視和共用他們建立、與他們共用以及公開集合的集合。
seo-description: Experience Manager Assets Brand Portal Administrators can share and unshare a collection or a smart collection with authorized users. Editors can view and share only the collections created by them, shared with them, and public collections.
uuid: 965f39cd-1378-42c1-a58a-01e1bf825aa3
contentOwner: Vishabh Gupta
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f053013e-5981-419f-927e-b5bb1d47eae2
exl-id: 29b877f6-4200-4299-9b8d-81d88f4e8221
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 1%

---

# 共用集合 {#share-collections}

集合代表儲存在Adobe Experience Manager Assets Brand Portal中一組相關資產。 使用者可透過以下方式建立智慧型集合 [套用omnisearch或facet搜尋以篩選掉相關資產](brand-portal-searching.md) 並將其儲存在一起，以便輕鬆存取並進一步與其他Brand Portal使用者共用。

管理員可與授權的Brand Portal使用者共用和取消共用集合。 編輯者和檢視者可以檢視和共用他們建立、與他們共用以及公開集合的集合。

>[!NOTE]
>
>編輯人員無法將公用集合變更為非公用集合，因此沒有 **[!UICONTROL 公開集合]** 中可用的核取方塊 **[!UICONTROL 集合設定]** 對話方塊。

## 共享收藏集 {#share-collection}

以下是和授權的Brand Portal使用者共用集合的步驟：

1. 登入您的Brand Portal租使用者。 根據預設， **[!UICONTROL 檔案]** 檢視會開啟，其中包含所有已發佈的資產和資料夾。

1. 在頂端的快速導覽中，按一下 **[!UICONTROL 集合]**.

1. 從 **[!UICONTROL 集合]** 主控台，執行下列任一項作業：

   * 將指標暫留在您要共用的集合上。 在集合可用的快速動作縮圖中，按一下 **[!UICONTROL 設定]** 圖示。

      ![](assets/settings-icon.png)

   * 選取您要共用的集合。 在頂端的工具列中，按一下 **[!UICONTROL 設定]**.

      ![](assets/collection-console.png)

1. 在 **[!UICONTROL 集合設定]** 對話方塊中，選取您要與其共用集合的使用者，並選取使用者的角色，以與其全域角色相符。 例如，將編輯者角色指派給全域編輯者，將檢視者角色指派給全域檢視者。

   或者，若要讓系列可供所有使用者使用（無論其群組成員資格和角色為何），請選取 **[!UICONTROL 公開集合]** 核取方塊。

   >[!NOTE]
   >
   >但是，非管理員使用者可以限制建立公開集合，以避免擁有許多公開集合，從而可以節省系統空間。 組織可以停用 **[!UICONTROL 允許建立公開集合]** 設定來源 **[!UICONTROL 一般]** 「管理工具」面板中可用的設定。

   ![](assets/collection_sharingadduser.png)

   編輯人員無法將公用集合變更為非公用集合，因此沒有 **[!UICONTROL 公開集合]** 中可用的核取方塊 **[!UICONTROL 集合設定]** 對話方塊。

   ![](assets/collection-setting-editor.png)

1. 按一下 **[!UICONTROL 新增]** 按鈕以新增使用者，然後按一下 **[!UICONTROL 儲存]**. 集合會與使用者共用。

   >[!NOTE]
   >
   >使用者的角色可控制對集合內資產和資料夾的存取權。 如果使用者無權存取資產，則會與使用者共用空白集合。 此外，使用者的角色會控制可用於集合的動作。

## 取消共用集合 {#unshare-a-collection}

若要取消共用先前共用的集合，請執行下列動作：

1. 從 **[!UICONTROL 集合]** 控制檯中，選取您要取消共用的集合。

   在頂端的工具列中，按一下 **[!UICONTROL 設定]**.

   ![](assets/collection_settings.png)

1. 在 **[!UICONTROL 集合設定]** 對話方塊，在 **[!UICONTROL 成員]** 區段，按一下 **[!UICONTROL x]** 使用者旁邊的符號，用於從擁有集合存取許可權的使用者清單中移除這些使用者。

   ![](assets/unshare_collection.png)

1. 出現警告訊息。 按一下 **[!UICONTROL 確認]** 以取消共用集合。

1. 按一下 **[!UICONTROL 儲存]** 以套用變更。

   從共用清單中移除使用者後，非共用集合就會從使用者的 **[!UICONTROL 集合]** 主控台。

<!--
1. Click the overlay icon on the left, and choose **[!UICONTROL Navigation]**.

   ![](assets/contenttree-1.png)

1. From the siderail on the left, click **[!UICONTROL Collections]**.

   ![](assets/access_collections.png)

1. From the **[!UICONTROL Collections]** console, do one of the following:

    * Hover the pointer over the collection you want to share. From the quick action thumbnails available for the collection, click the **[!UICONTROL Settings]** icon.

   ![](assets/settings_thumbnail.png)

    * Select the collection you want to share. From the toolbar at the top, click **[!UICONTROL Settings]**.
    
   ![](assets/collection-sharing.png)

1. In the [!UICONTROL Collection Settings] dialog box, select the users or groups with whom you want to share the collection and select the role for a user or a group to match their global role. For example, assign the Editor role to a global editor, the Viewer role to a global viewer.

   Alternatively, to make the collection available to all users irrespective of their group membership and role, make it public by selecting the **[!UICONTROL Public Collection]** check-box.

   >[!NOTE]
   >
   >However, non-admin users can be restricted from creating public collections, to avoid having numerous public collections so that system space can be saved. Organizations can disable the **[!UICONTROL Allow public collections creation]** configuration from [!UICONTROL General] settings available in admin tools panel.

   ![](assets/collection_sharingadduser.png)

   Editors cannot change a public collection to a non-public collection and, therefore, do not have **[!UICONTROL Public Collection]** check-box available in **[!UICONTROL Collection Settings]** dialog.

   ![](assets/collection-setting-editor.png)

1. Select **[!UICONTROL Add]**, and then **[!UICONTROL Save]**. The collection is shared with the chosen users.

   >[!NOTE]
   >
   >A user's role governs access to the assets and folders inside a collection. If a user does not have access to assets, an empty collection is shared with the user. Also, a user's role governs the actions available for collections.

## Unshare a collection {#unshare-a-collection}

To unshare a previously shared collection, do the following:

1. From the **[!UICONTROL Collections]** console, select the collection you want to unshare.

   In the toolbar, click **[!UICONTROL Settings]**.

   ![](assets/collection_settings.png)

1. On the **[!UICONTROL Collection Settings]** dialog box, under **[!UICONTROL Members]**, click the **[!UICONTROL x]** symbol next to users or groups to remove them from the list of users you shared the collection with.

   ![](assets/unshare_collection.png)

1. In the warning message box, click **[!UICONTROL Confirm]** to confirm unshare.

   Click **[!UICONTROL Save]**.

1. Log in to Brand Portal with the credentials of the user you removed from the shared list. The collection is removed from the **[!UICONTROL Collections]** console.
-->
