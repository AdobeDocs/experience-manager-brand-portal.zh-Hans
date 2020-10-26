---
title: 共享收藏集
seo-title: 共享收藏集
description: AEM Assets品牌门户管理员可以与授权用户共享和取消共享集合或智能集合。 编辑只能视图和共享由他们创建的集合、与他们共享的集合以及公共集合。
seo-description: AEM Assets品牌门户管理员可以与授权用户共享和取消共享集合或智能集合。 编辑只能视图和共享由他们创建的集合、与他们共享的集合以及公共集合。
uuid: 965f39cd-1378-42c1-a58a-01e1bf825aa3
contentOwner: Vishabh Gupta
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f053013e-5981-419f-927e-b5bb1d47eae2
translation-type: tm+mt
source-git-commit: a587061bc8afe250a88b4a02b42b6acd9ef6bbeb
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 1%

---


# 共享集合 {#share-collections}

集合表示存储在Adobe Experience Manager资产品牌门户中的一组相关资产。 用户可通过应用全搜索或 [facet搜索来创建智能收藏集，从而筛选出相关资产](brand-portal-searching.md) ，并将它们存储在一起，以便轻松访问，并进一步与其他Brand Portal用户共享。

管理员可以与授权的Brand Portal用户共享和取消共享集合。 编辑和查看者可以视图和共享由他们创建的集合、与他们共享的集合以及公共集合。

>[!NOTE]
>
>编辑者无法将公共集合更改为非公共集合，因此“集合设置”对话框中 **[!UICONTROL 不提供]** “公共集合” **[!UICONTROL 复选框]** 。

## 共享收藏集 {#share-collection}

以下是与授权Brand Portal用户共享集合的步骤：

1. 登录到您的Brand Portal租户。 默认情况下，将打 **[!UICONTROL 开]** “文件”视图，其中包含所有已发布的资产和文件夹。

1. 在顶部的快速导航中，单击“集 **[!UICONTROL 合”]**。

1. 在“收 **[!UICONTROL 藏集]** ”控制台中，执行下列操作之一：

   * 将指针悬停在要共享的集合上。 从集合可用的快速操作缩略图中，单击“设 **[!UICONTROL 置]** ”图标。

      ![](assets/settings-icon.png)

   * 选择要共享的集合。 在顶部的工具栏中，单击“ **[!UICONTROL 设置”]**。

      ![](assets/collection-console.png)

1. 在收 **[!UICONTROL 藏集设置]** 对话框中，选择要与其共享收藏集的用户，然后为用户选择与其全局角色匹配的角色。 例如，为全局编辑器分配“编辑者”角色，为全局查看器分配“查看者”角色。

   或者，要使集合对所有用户可用（不论其用户组成员身份和角色如何），请通过选中“公共集合”复选 **[!UICONTROL 框将其公]** 开。

   >[!NOTE]
   >
   >但是，非管理员用户可能无法创建公共集合，以避免拥有大量公共集合，从而可以保存系统空间。 组织可以从管理工具 **[!UICONTROL 面板中提供的]** “常规 **[!UICONTROL ”设置禁]** 用“允许创建公共集合”配置。

   ![](assets/collection_sharingadduser.png)

   编辑者无法将公共集合更改为非公共集合，因此“集合设置”对话框 **[!UICONTROL 中不提供]** “公共集合” **[!UICONTROL 复选框]** 。

   ![](assets/collection-setting-editor.png)

1. 单击“ **[!UICONTROL 添加]** ”按钮以添加用户，然后单击“ **[!UICONTROL 保存”]**。 集合将与用户共享。

   >[!NOTE]
   >
   >用户的角色控制对集合中的资产和文件夹的访问权限。 如果用户无权访问资产，则会与该用户共享一个空集合。 此外，用户的角色将控制集合的可用操作。

## 取消共享集合 {#unshare-a-collection}

要取消共享以前共享的集合，请执行以下操作：

1. 从“收 **[!UICONTROL 藏集]** ”控制台中，选择要取消共享的收藏集。

   在顶部的工具栏中，单击“ **[!UICONTROL 设置”]**。

   ![](assets/collection_settings.png)

1. 在“集 **[!UICONTROL 合设置]** ”对话框的“成员 **[!UICONTROL ”部分下，单击]** 用户旁的 **** x符号，将其从有权访问该集合的用户列表中删除。

   ![](assets/unshare_collection.png)

1. 出现警告消息。 单击 **[!UICONTROL 确认]** ，取消共享集合。

1. Click **[!UICONTROL Save]** to apply the changes.

   从共享列表中删除用户后，将从用户的“集合”控制台中删除未共享的 **[!UICONTROL 集合]** 。

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