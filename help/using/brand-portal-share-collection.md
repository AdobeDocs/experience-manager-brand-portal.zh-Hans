---
title: 共享集合
seo-title: 共享集合
description: AEM Assets Brand Portal管理员可以与授权用户共享和取消共享集合或智能集合。 编辑只能查看和共享由他们创建的集合、与他们共享的集合以及公共集合。
seo-description: AEM Assets Brand Portal管理员可以与授权用户共享和取消共享集合或智能集合。 编辑只能查看和共享由他们创建的集合、与他们共享的集合以及公共集合。
uuid: 965f39cd-1378-42c1-a58a-01e1bf825aa3
contentOwner: bdhar
content-type: 引用
topic-tags: 共享
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f053013e-5981-419f-927e-b5bb1d47eae2
translation-type: tm+mt
source-git-commit: 86d4d5c358ea795e35db2dce8c9529ed14e9ee2d

---


# 在Brand Portal上共享集合 {#share-collections-bp}

AEM Assets Brand Portal管理员可以与授权用户共享和取消共享集合或智能集合。 编辑只能查看和共享由他们创建的集合、与他们共享的集合以及公共集合。 但是，编辑不能将公共集合更改为非公共集合。

>[!NOTE]
>
>编辑不能将公共集合更改为非公共集合，因此，“集合设置”对话框中不提供 [!UICONTROL “公共集合] ” [!UICONTROL 复选框] 。

## 共享集合 {#share-collection}

要共享集合，请执行以下步骤：

1. 单击左侧的叠加图标，然后选择“导 **[!UICONTROL 航”]**。

   ![](assets/contenttree-1.png)

1. 在左侧的脱轨处，单击“集 **[!UICONTROL 合”]**。

   ![](assets/access_collections.png)

1. 从“收 **[!UICONTROL 藏集]** ”控制台中，执行下列操作之一：

   * 将指针悬停在要共享的集合上。 在集合的可用快速操作缩略图中，单击“设 **[!UICONTROL 置]** ”图标。
   ![](assets/settings_thumbnail.png)

   * 选择要共享的集合。 在顶部的工具栏中，单击“设 **[!UICONTROL 置”]**。
   ![](assets/collection-sharing.png)

1. 在“收 [!UICONTROL 藏集设置] ”对话框中，选择要与其共享收藏集的一个或多个用户组，然后为用户或用户组选择与其全局角色匹配的角色。 例如，将“编辑者”角色分配给全局编辑者，将“查看者”角色分配给全局查看者。

   或者，要使集合对所有用户可用（不论其用户组成员关系和角色如何），请通过选中“公共集合 **** ”复选框将其公开。

   >[!NOTE]
   >
   >但是，非管理员用户可能无法创建公共集合，以避免拥有大量公共集合，从而可以保存系统空间。 组织可以从管理工具 **[!UICONTROL 面板中提供的常规设置]** ，禁  用“允许创建公共集合”配置。

   ![](assets/collection_sharingadduser.png)

   编辑不能将公共集合更改为非公共集合，因此，“集合设置”对话框中不提供 [!UICONTROL “公共集合] ” [!UICONTROL 复选框] 。

   ![](assets/collection-setting-editor.png)

1. 选择 **[!UICONTROL 添加]**，然后选择 **[!UICONTROL 保存]**。 集合将与所选用户共享。

   >[!NOTE]
   >
   >用户的角色控制对集合中的资产和文件夹的访问。 如果用户无权访问资产，则会与该用户共享空集合。 此外，用户的角色将控制集合的可用操作。

## 取消共享集合 {#unshare-a-collection}

要取消共享以前共享的集合，请执行以下操作：

1. 从“收 [!UICONTROL 藏集] ”控制台中，选择要取消共享的收藏集。

   在工具栏中，单击“设 **[!UICONTROL 置”]**。

   ![](assets/collection_settings.png)

1. 在“集 [!UICONTROL 合设置] ”对话框的“成员”下，单击用户或用户组旁边的 **** x符号，以从您与其共享集合的用户列表中删除它们。

   ![](assets/unshare_collection.png)

1. 在警告消息框中，单击“确 **[!UICONTROL 认]** ”以确认取消共享。

   Click **[!UICONTROL Save]**.

1. 使用您从共享列表中删除的用户的凭据登录到Brand Portal。 集合将从“集合”控制 **[!UICONTROL 台中删]** 除。
