---
title: 共享收藏集
seo-title: Share a collection
description: Experience ManagerAssets Brand Portal管理员可以与授权用户共享和取消共享收藏集或智能收藏集。 编辑者只能查看和共享由他们创建、与他们共享的收藏集以及公共收藏集。
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

# 共享收藏集 {#share-collections}

收藏集表示存储在Adobe Experience Manager Assets Brand Portal中的一组相关资产。 用户可以通过[应用Omnisearch或Facet搜索创建智能收藏集，以筛选出相关资产](brand-portal-searching.md)并将它们存储在一起，以便轻松访问并进一步与其他Brand Portal用户共享。

管理员可以与授权的Brand Portal用户共享和取消共享收藏集。 编辑者和查看者可以查看和共享由他们创建的收藏集、与他们共享的收藏集以及公共收藏集。

>[!NOTE]
>
>编辑者无法将公共收藏集更改为非公共收藏集，因此在&#x200B;**[!UICONTROL 收藏集设置]**&#x200B;对话框中没有可用的&#x200B;**[!UICONTROL 公共收藏集]**&#x200B;复选框。

## 共享收藏集 {#share-collection}

以下是与授权的Brand Portal用户共享收藏集的步骤：

1. 登录到您的Brand Portal租户。 默认情况下，将打开&#x200B;**[!UICONTROL 文件]**&#x200B;视图，其中包含所有已发布的资产和文件夹。

1. 在顶部的快速导航中，单击&#x200B;**[!UICONTROL 收藏集]**。

1. 从&#x200B;**[!UICONTROL 收藏集]**&#x200B;控制台中，执行下列操作之一：

   * 将指针悬停在要共享的收藏集上。 在集合可用的快速操作缩略图中，单击&#x200B;**[!UICONTROL 设置]**&#x200B;图标。

      ![](assets/settings-icon.png)

   * 选择要共享的收藏集。 在顶部的工具栏中，单击&#x200B;**[!UICONTROL 设置]**。

      ![](assets/collection-console.png)

1. 在&#x200B;**[!UICONTROL 收藏集设置]**&#x200B;对话框中，选择要与其共享收藏集的用户，然后为该用户选择角色以匹配其全局角色。 例如，将“编辑者”角色分配给全局编辑者，将“查看者”角色分配给全局查看者。

   或者，要使集合可供所有用户使用，而不考虑其组成员资格和角色，请通过选中&#x200B;**[!UICONTROL Public Collection]**&#x200B;复选框将其公开。

   >[!NOTE]
   >
   >但是，可以限制非管理员用户创建公共集合，以避免拥有大量公共集合，从而可以节省系统空间。 组织可以禁用管理工具面板中提供的&#x200B;**[!UICONTROL 允许从**[!UICONTROL &#x200B;常规&#x200B;]**设置创建]**&#x200B;公共集合。

   ![](assets/collection_sharingadduser.png)

   编辑器无法将公共集合更改为非公共集合，因此在&#x200B;**[!UICONTROL 集合设置]**&#x200B;对话框中没有&#x200B;**[!UICONTROL 公共集合]**&#x200B;复选框。

   ![](assets/collection-setting-editor.png)

1. 单击&#x200B;**[!UICONTROL Add]**&#x200B;按钮以添加用户，然后单击&#x200B;**[!UICONTROL Save]**。 收藏集将与用户共享。

   >[!NOTE]
   >
   >用户的角色控制对收藏集中资产和文件夹的访问权限。 如果用户无权访问资产，则会与用户共享一个空的收藏集。 此外，用户的角色也控制可用于收藏集的操作。

## 取消共享收藏集 {#unshare-a-collection}

要取消共享之前共享的收藏集，请执行以下操作：

1. 从&#x200B;**[!UICONTROL 收藏集]**&#x200B;控制台中，选择要取消共享的收藏集。

   在顶部的工具栏中，单击&#x200B;**[!UICONTROL 设置]**。

   ![](assets/collection_settings.png)

1. 在&#x200B;**[!UICONTROL 收藏集设置]**&#x200B;对话框的&#x200B;**[!UICONTROL 成员]**&#x200B;部分下，单击用户旁边的&#x200B;**[!UICONTROL x]**&#x200B;符号，以从有权访问收藏集的用户列表中将其删除。

   ![](assets/unshare_collection.png)

1. 出现警告消息。 单击&#x200B;**[!UICONTROL Confirm]**&#x200B;取消共享该集合。

1. 单击&#x200B;**[!UICONTROL Save]**&#x200B;以应用更改。

   从共享列表中删除用户后，将从用户的&#x200B;**[!UICONTROL 收藏集]**&#x200B;控制台中删除非共享的收藏集。

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
