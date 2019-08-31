---
title: 共享文件夹
seo-title: 共享文件夹
description: Brand Portal不支持资产摄取，因此必须从预配置的AEM作者实例将资产发布到Brand Portal。Brand Portal的非管理员用户无法访问发布的资源，除非在使用AEM实例配置复制时配置，并且需要与它们共享。
seo-description: Brand Portal不支持资产摄取，因此必须从预配置的AEM作者实例将资产发布到Brand Portal。Brand Portal的非管理员用户无法访问发布的资源，除非在使用AEM实例配置复制时配置，并且需要与它们共享。
uuid: 340d0a49-b708-4f0 e-9fb8-99c824942 f34
content-type: 引用
topic-tags: sharing
products: SG_ EXPERIENCE MANAGER/Brand_ Portal
discoiquuid: 2332c16f-40be-4673-8cc6-2360d5b74116
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# 在Brand Portal上共享文件夹 {#share-folders}

需要从预配置的AEM作者实例将资产发布到Brand Portal，因为Brand Portal不支持资产摄取。

## Brand Portal中的文件夹共享工作流程 {#folder-sharing-workflow-in-brand-portal}

以下描述了文件夹共享工作流和用户访问权限：

* 默认情况下，除非在配置复制过程中标记为公共，否则从AEM Assets发布到Brand Portal的所有文件夹仅对Brand Portal管理员可见。
* 管理员使用 [!UICONTROL 文件夹属性] 控制台与选择性用户或用户组共享文件夹。只有那些共享文件夹的用户或用户组登录到Brand Portal后才能看到文件夹。其他用户看不到该文件夹。
* 管理员还可以选择通过文件夹属性控制台中的 [!UICONTROL “公共文件夹] ”复选 [!UICONTROL 框公开] 文件夹。所有用户都可以看到公共文件夹。

* 无论用户角色和权限是什么，当用户登录到Brand Portal时，他们都会看到所有公共文件夹，以及直接与他们共享的文件夹或与其所属的组共享的文件夹。所有用户都看不到私人文件夹或与其他用户共享的文件夹。

### 与Brand Portal上的用户组共享文件夹 {#sharing-folders-with-user-groups-on-brand-portal}

无论子文件夹的设置如何，对文件夹资源的访问权限均与其父文件夹上的访问权限相关。此行为受AEM中 [的ACL](https://helpx.adobe.com/experience-manager/6-5/sites/administering/using/security.html#PermissionsinAEM) 约束，因为子文件夹继承了父文件夹中的ACL。例如，如果文件夹A包含文件夹B，则在文件夹B中具有访问权限的用户组(或用户)也具有与文件夹B和文件夹相同的访问权限。文件夹B作为继承其ACL的子文件夹，而文件夹C作为继承其ACL的子文件夹C继承其ACL。

同样，只有有权访问文件夹B的用户组(或用户)具有对文件夹C但不在文件夹A上的访问权限。因此，建议组织安排其内容，使暴露的资源位于子文件夹中，并且从子文件夹到根文件夹访问可以受到限制。

### Public folder publish {#public-folder-publish}

除非在配置Brand Portal复制时选择 [!UICONTROL “Public Folder Publish] ”(公共文件夹发布)选项，否则非管理员用户(如编辑器和查看器)无权访问从AEM Assets发布到Brand Portal的资产。

![](assets/assetbpreplication.png)

如果禁用 [!UICONTROL 了“Public Folder Publish] ”(公共文件夹发布)选项，管理员需要使用共享功能与非管理员用户专门共享这些资产。

>[!NOTE]
>
>从AEM6.3.2.1开始，可以选择启用 [!UICONTROL “Public Folder Publish”] (公共文件夹发布)选项。

## 访问共享文件夹 {#access-to-shared-folders}

下面的矩阵讨论了用于为各种用户角色共享/取消共享资源的访问权限和权限：

|  | 访问从AEM资产发布到Brand Portal的所有文件夹 | 访问共享文件夹 | 共享/取消共享文件夹权限 |
|---------------|-----------|-----------|------------|
| 管理员 | 是 | 是 | 是 |
| 编辑者 | 否* | 是，仅当共享时或与其所属的组共享时 | 是，仅适用于与它们共享的文件夹或与其所属的用户组共享的文件夹 |
| 查看者 | 否* | 是，仅当共享时或与其所属的组共享时 | 否 |
| 来宾用户 | 否* | 是，仅当共享时或与其所属的组共享时 | 否 |

**默认情况下，在使用AEM作者配置Brand Portal复制时，[!UICONTROL “Public Folder Publish”](公共文件夹发布)选项被禁用。如果启用此选项，默认情况下所有用户(非管理员用户)均可访问发布到Brand Portal的文件夹。*

### 非管理员用户访问共享文件夹 {#non-admin-user-access-to-shared-folders}

非管理员用户只能访问在Brand Portal上共享的文件夹。但是，这些文件夹在登录时在门户网站上显示的方式取决于 [!UICONTROL “启用文件夹层次结构”] 配置的设置。

**如果配置被禁用**

非管理员用户在登录到Brand Portal时查看登录页面上与其共享的所有文件夹。

![](assets/disabled-folder-hierarchy1-1.png)

**如果已启用配置**

非管理员用户可在登录到Brand Portal时看到文件夹树(从根文件夹开始)以及排列在各自父文件夹内的共享文件夹。

这些父文件夹是虚拟文件夹，不可对这些文件夹执行任何操作。您可以使用锁定图标识别这些虚拟文件夹。

与共享文件夹不同，在 [!UICONTROL “卡片视图]”中悬停或选择操作任务时不会看到任何操作任务。[!UICONTROL 在][!UICONTROL 列视图] 和 [!UICONTROL 列表视图中选择虚拟文件夹时，会显示概述按钮]。

>[!NOTE]
>
>请注意，虚拟文件夹的默认缩略图是第一个共享文件夹的缩略图图象。

![](assets/enabled-hierarchy1-1.png) ![](assets/hierarchy1-nonadmin-1.png) ![](assets/hierarchy-nonadmin-1.png) ![](assets/hierarchy2-nonadmin-1.png)

## 共享文件夹 {#how-to-share-folders}

要与Brand Portal上的用户共享文件夹，请按照以下步骤操作：

1. 单击左侧的叠加图标，然后选择 **[!UICONTROL “导航]**”。

   ![](assets/selectorrail.png)

2. 从左侧的提要栏中，选择 **[!UICONTROL “文件]**”。

   ![](assets/access_files.png)

3. 从Brand Portal界面中，选择要共享的文件夹。

   ![](assets/share-folders.png)

4. 从顶部的工具栏中，选择 **[!UICONTROL 共享]**。

   ![](assets/share_icon.png)

   此时会显示 [!UICONTROL 文件夹属性] 控制台。

   ![](assets/folder_properties.png)

5. 如果您不希望向用户显示默认名称，请在 [!UICONTROL 文件夹属性] 控制台中，指定 [!UICONTROL 文件夹标题] 字段中的文件夹标题。
6. 从 [!UICONTROL 添加用户] 列表中，选择要与其共享文件夹的用户或用户组，然后单击 **[!UICONTROL 添加]**。
要仅与客人用户共享文件夹，而不是其他用户，请 **** 从 [!UICONTROL 成员] 下拉列表中选择“匿名用户”。

   ![](assets/only-anonymous.png)

   >[!NOTE]
   >
   >要使所有用户都可使用该文件夹，而不管其用户组成员资格和角色如何，请通过选择 **[!UICONTROL “公共文件夹]** ”复选框公开该文件夹。

7. 如有必要，单击 **[!UICONTROL “更改缩略图]** ”以修改文件夹的缩略图图象。
8. Click **[!UICONTROL Save]**.
9. 要访问共享文件夹，请使用您共享文件夹的用户凭据登录到Brand Portal。查看界面中的共享文件夹。

## 取消共享文件夹 {#unshare-the-folders}

要取消共享先前共享的文件夹，请按照以下步骤操作：

1. 从Brand Portal界面中，选择要取消共享的文件夹。

   ![](assets/share-folders-1.png)

2. 从顶部的工具栏中，单击 **[!UICONTROL 共享]**。
3. 在 [!UICONTROL 文件夹属性] 控制台的 [!UICONTROL 成员]下，单击用户旁边 **[!UICONTROL 的x]** 符号，从您共享文件夹的用户列表中删除这些符号。

   ![](assets/folder_propertiesunshare.png)

4. 在警告消息框中，单击 **[!UICONTROL 确认]** 以确认取消共享。
Click **[!UICONTROL Save]**.

5. 使用您从共享列表中删除的用户凭据登录到Brand Portal。该文件夹不再在用户的Brand Portal界面中提供。
