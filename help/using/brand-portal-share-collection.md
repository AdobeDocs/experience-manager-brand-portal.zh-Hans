---
title: 共享集合
seo-title: 共享集合
description: AEM Assets Brand Portal管理员可以与授权用户共享和取消共享集合或智能收藏集。编辑人员只能查看和共享由它们创建、与其共享和公共集合的集合。
seo-description: AEM Assets Brand Portal管理员可以与授权用户共享和取消共享集合或智能收藏集。编辑人员只能查看和共享由它们创建、与其共享和公共集合的集合。
uuid: 965f39cd-1378-42c1-a58 a-01e1 bf825 aa3
contentOwner: bdar
content-type: 引用
topic-tags: sharing
products: SG_ EXPERIENCE MANAGER/Brand_ Portal
discoiquuid: f053013e-5981-419f-927e-b5 bb1 d47 eae2
translation-type: tm+mt
source-git-commit: 0b70e82d034ce56fcfc5b49396e6d3a9da4b49d4

---


# 在Brand Portal上共享收藏集 {#share-collections-bp}

AEM Assets Brand Portal管理员可以与授权用户共享和取消共享集合或智能收藏集。编辑人员只能查看和共享由它们创建、与其共享和公共集合的集合。但是，编辑人员无法将公共集合更改为非公开集合。

>[!NOTE]
>
>编辑人员无法将公共集合更改为非公开集合，因此 ******，“集合设置** ”对话框中没有“公共收藏集”复选框。

## 共享集合 {#share-collection}

要共享集合，请按照以下步骤操作：

1. 单击左侧的叠加图标，然后选择 **“导航**”。

   ![](assets/contenttree-1.png)

1. 从左侧的提要栏中，单击 **收藏集**。

   ![](assets/access_collections.png)

1. 从 **收藏集** 控制台中，执行下列操作之一：

   * 将指针悬停在要共享的集合上。从可用于集合的快速操作缩略图中，单击 **设置** 图标。
   ![](assets/settings_thumbnail.png)

   * 选择要共享的集合。在顶部的工具栏中，单击 **设置**。
   ![](assets/collection-sharing.png)

1. 在 **“集合设置”** 对话框中，选择要与之共享集合的用户或用户组，并选择用户或组的角色以匹配其全局角色。例如，将“编辑器”角色分配给全局编辑器，即全局查看器角色。

   或者，也可以通过选择 **“公共收藏集** ”复选框，为所有用户提供集合，而不管用户组成员资格和角色如何。

   >[!NOTE]
   >
   >但是，不能限制非管理员用户创建公共集合，以避免有大量公共集合，从而可以保存系统空间。组织可以从管理 **工具面板中提供****的常规** 设置禁用“允许公共集合创建配置”。

   ![](assets/collection_sharingadduser.png)

   编辑人员无法将公共集合更改为非公开集合，因此 ******，“集合设置** ”对话框中没有“公共收藏集”复选框。

   ![](assets/collection-setting-editor.png)

1. 单击 **添加**，然后单击 **保存**。集合将与选定的用户共享。

   >[!NOTE]
   >
   >用户的角色可控制集合中的资产和文件夹。如果用户无权访问资产，则会与该用户共享一个空集合。此外，用户的角色对集合的可用操作进行约束。

## 取消共享集合 {#unshare-a-collection}

要取消共享以前共享的集合，请执行以下操作：

1. 从 **收藏集** 控制台中，选择要取消共享的收藏集。

   在工具栏中，单击 **设置**。

   ![](assets/collection_settings.png)

1. 在 **“集合设置** ”对话框的 **“成员**”下，单击用户或用户组旁边 **的x** 符号，以便从您共享集合的用户列表中删除这些符号。

   ![](assets/unshare_collection.png)

1. 在警告消息框中，单击 **确认** 以确认取消共享。

   单击&#x200B;**保存**。

1. 使用您从共享列表中删除的用户凭据登录到Brand Portal。将从 **收藏集** 控制台中删除收藏集。
