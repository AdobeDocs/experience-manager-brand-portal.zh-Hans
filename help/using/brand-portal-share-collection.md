---
title: 共享收藏集
seo-title: 共享收藏集
description: AEM Assets品牌门户管理员可以与授权用户共享和取消共享集合或智能集合。 编辑只能视图和共享由他们创建的集合、与他们共享的集合以及公共集合。
seo-description: AEM Assets品牌门户管理员可以与授权用户共享和取消共享集合或智能集合。 编辑只能视图和共享由他们创建的集合、与他们共享的集合以及公共集合。
uuid: 965f39cd-1378-42c1-a58a-01e1bf825aa3
contentOwner: bdhar
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f053013e-5981-419f-927e-b5bb1d47eae2
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 2%

---


# 在Brand Portal上共享集合 {#share-collections-bp}

AEM Assets品牌门户管理员可以与授权用户共享和取消共享集合或智能集合。 编辑只能视图和共享由他们创建的集合、与他们共享的集合以及公共集合。 但是，编辑人员无法将公共集合更改为非公共集合。

>[!NOTE]
>
>编辑者无法将公共集合更改为非公共集合，因此“集合设置”对话框中 **[!UICONTROL 不提供]** “公共集合” **[!UICONTROL 复选框]** 。

## 共享收藏集 {#share-collection}

要共享集合，请执行以下步骤：

1. 单击左侧的叠加图标，然后选择“ **[!UICONTROL 导航]**”。

   ![](assets/contenttree-1.png)

1. 在左侧的脱轨处，单击“ **[!UICONTROL 集合]**”。

   ![](assets/access_collections.png)

1. 在“收 **[!UICONTROL 藏集]** ”控制台中，执行下列操作之一：

   * 将指针悬停在要共享的集合上。 从集合可用的快速操作缩略图中，单击“设 **[!UICONTROL 置]** ”图标。

   ![](assets/settings_thumbnail.png)

   * 选择要共享的集合。 在顶部的工具栏中，单击“ **[!UICONTROL 设置”]**。

   ![](assets/collection-sharing.png)

1. 在收 [!UICONTROL 藏集设置] 对话框中，选择要与其共享收藏集的用户或用户组，然后为要匹配其全局角色的用户或用户组选择角色。 例如，将“编辑者”角色分配给全局编辑者，将“查看者”角色分配给全局查看者。

   或者，要使集合对所有用户可用（不论其用户组成员身份和角色如何），请通过选中“公共集合”复选 **[!UICONTROL 框将其公]** 开。

   >[!NOTE]
   >
   >但是，非管理员用户可能无法创建公共集合，以避免拥有大量公共集合，从而可以保存系统空间。 组织可以从管理工具 **[!UICONTROL 面板中提供的]** “常规” [!UICONTROL 设置禁用] “允许创建公共集合”配置。

   ![](assets/collection_sharingadduser.png)

   编辑者无法将公共集合更改为非公共集合，因此，“集合设置”对 **[!UICONTROL 话框中不]** 提供“公共 **[!UICONTROL 集合]** ”复选框。

   ![](assets/collection-setting-editor.png)

1. 选择 **[!UICONTROL 添加]**，然后选择 **[!UICONTROL 保存]**。 集合将与所选用户共享。

   >[!NOTE]
   >
   >用户的角色将控制对集合中的资产和文件夹的访问权限。 如果用户无权访问资产，则会与该用户共享一个空集合。 此外，用户的角色将控制集合的可用操作。

## 取消共享集合 {#unshare-a-collection}

要取消共享以前共享的集合，请执行以下操作：

1. 从“收 **[!UICONTROL 藏集]** ”控制台中，选择要取消共享的收藏集。

   在工具栏中，单击 **[!UICONTROL 设置]**。

   ![](assets/collection_settings.png)

1. 在“集 **[!UICONTROL 合设置]** ”对话框的“成员” **[!UICONTROL 下，单击]**&#x200B;用户或组旁的 **** x符号，将其从您与其共享集合的用户列表中删除。

   ![](assets/unshare_collection.png)

1. 在警告消息框中，单击“ **[!UICONTROL 确认]** ”以确认取消共享。

   单击&#x200B;**[!UICONTROL 保存]**。

1. 使用您从共享列表中删除的用户的凭据登录到Brand Portal。 集合将从“集合”控 **[!UICONTROL 制台]** 删除。
