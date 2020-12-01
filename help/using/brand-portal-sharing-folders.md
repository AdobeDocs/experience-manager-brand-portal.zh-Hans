---
title: 共享文件夹
seo-title: 共享文件夹
description: Brand Portal不支持资产摄取，因此必须从预配置的AEM作者实例将资产发布到Brand Portal。 Brand Portal的非管理员用户无法访问发布的资产，除非在使用AEM实例配置复制时进行了配置，因此需要与他们共享。
seo-description: Brand Portal不支持资产摄取，因此必须从预配置的AEM作者实例将资产发布到Brand Portal。 Brand Portal的非管理员用户无法访问发布的资产，除非在使用AEM实例配置复制时进行了配置，因此需要与他们共享。
uuid: 340d0a49-b708-4f0e-9fb8-99c824942f34
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 2332c16f-40be-4673-8cc6-2360d5b74116
translation-type: tm+mt
source-git-commit: 0ae9860e2b6beb96f53e92bb114bb5756e371ad6
workflow-type: tm+mt
source-wordcount: '1154'
ht-degree: 1%

---


# 在Brand Portal上共享文件夹{#share-folders}

资产需要从预配置的AEM作者实例发布到Brand Portal，因为Brand Portal不支持资产摄取。

## Brand Portal {#folder-sharing-workflow-in-brand-portal}中的文件夹共享工作流

下面介绍了文件夹共享工作流和用户访问权限：

* 默认情况下，从AEM Assets发布到Brand Portal的所有文件夹只对Brand Portal管理员可见，除非在配置复制时标记为公共。
* 管理员使用&#x200B;**[!UICONTROL 文件夹属性]**&#x200B;控制台与选择性用户或用户组共享文件夹。 只有与共享文件夹的用户或用户组在登录到Brand Portal后才能看到该文件夹。 其他用户看不到该文件夹。
* 管理员还可以通过&#x200B;**[!UICONTROL 文件夹属性]**&#x200B;控制台中的&#x200B;**[!UICONTROL 公用文件夹]**&#x200B;复选框将文件夹公开。 公共文件夹对所有用户可见。

* 无论用户角色和权限如何，当用户登录到Brand Portal时，他们都会看到所有公共文件夹，以及直接与他们共享的文件夹或与他们所属的组共享的文件夹。 私人文件夹或与其他用户共享的文件夹对所有用户都不可见。

### 在Brand Portal上与用户组共享文件夹{#sharing-folders-with-user-groups-on-brand-portal}

对文件夹资产的访问权限取决于其父文件夹的访问权限，而与子文件夹的设置无关。 此行为受AEM中[ACL](https://helpx.adobe.com/experience-manager/6-5/sites/administering/using/security.html#PermissionsinAEM)的约束，因为子文件夹从父文件夹继承ACL。 例如，如果文件夹A包含包含文件夹C的文件夹B，则对文件夹A具有访问权限的用户组（或用户）对文件夹B和文件夹C也具有相同的访问权限。文件夹B是A的子文件夹继承其ACL，文件夹C是B的子文件夹继承其ACL。

同样，具有仅访问文件夹B权限的用户组（或用户）对文件夹C具有相同的访问权限，但对文件夹A不具有相同的访问权限。因此，建议组织安排其内容，以便将大多数暴露的资产放在子文件夹中，并限制从子文件夹到根文件夹的访问。

### 公用文件夹发布{#public-folder-publish}

除非在配置Brand Portal复制时选择&#x200B;**[!UICONTROL 公共文件夹发布]**&#x200B;选项，否则非管理员用户（如编辑和查看器）无权访问从AEM Assets发布到Brand Portal的资产。

![](assets/assetbpreplication.png)

如果禁用了&#x200B;**[!UICONTROL 公共文件夹发布]**&#x200B;选项，管理员需要使用共享功能专门与非管理员用户共享这些资产。

>[!NOTE]
>
>从AEM 6.3.2.1开始，可使用启用&#x200B;**[!UICONTROL 公共文件夹发布]**&#x200B;的选项。

## 访问共享文件夹{#access-to-shared-folders}

以下矩阵讨论了不同用户角色共享／取消共享资产的访问权限和权限：

|  | 访问从AEM Assets发布到Brand Portal的所有文件夹 | 访问共享文件夹 | 共享／取消共享文件夹权限 |
|---------------|-----------|-----------|------------|
| 管理员 | 是 | 是 | 是 |
| 编辑者 | 否* | 是，仅当与他们共享或与他们所属的组共享时 | 是，仅适用于与他们共享的文件夹或与他们所属的组共享的文件夹 |
| 查看者 | 否* | 是，仅当与他们共享或与他们所属的组共享时 | 否 |
| 来宾用户 | 否* | 是，仅当与他们共享或与他们所属的组共享时 | 否 |

>[!NOTE]
>
>默认情况下，在配置Brand Portal与AEM作者的复制时，将禁用&#x200B;**[!UICONTROL 公用文件夹发布]**&#x200B;选项。 如果启用此选项，则默认情况下，所有用户（非管理员用户）都可以访问发布到Brand Portal的文件夹。

### 非管理员用户访问共享文件夹{#non-admin-user-access-to-shared-folders}

非管理员用户只能访问品牌门户上与他们共享的文件夹。 但是，这些文件夹登录时在门户上的显示方式取决于&#x200B;**[!UICONTROL 启用文件夹层次结构]**&#x200B;配置的设置。

**如果禁用了配置**

非管理员用户登录到Brand Portal时，可以在登陆页查看与他们共享的所有文件夹。

![](assets/disabled-folder-hierarchy1-1.png)

**如果配置已启用**

非管理员用户登录到Brand Portal时，可以看到文件夹树（从根文件夹开始）和在其各自的父文件夹内排列的共享文件夹。

这些父文件夹是虚拟文件夹，不能对其执行任何操作。 您可以通过锁定图标识别这些虚拟文件夹。

与共享文件夹不同，在将鼠标悬停在&#x200B;**[!UICONTROL 卡片视图]**&#x200B;中选择操作任务时，不会显示任何操作。 **[!UICONTROL 在]** 列视图和列表视图中选择虚拟文件 **[!UICONTROL 夹]** 时，将显 **[!UICONTROL 示“概述”按钮]**。

>[!NOTE]
>
>请注意，虚拟文件夹的默认缩略图是第一个共享文件夹的缩略图。

![](assets/enabled-hierarchy1-1.png) ![](assets/hierarchy1-nonadmin-1.png) ![](assets/hierarchy-nonadmin-1.png) ![](assets/hierarchy2-nonadmin-1.png)

## 共享文件夹 {#how-to-share-folders}

要与Brand Portal上的用户共享文件夹，请执行以下步骤：

1. 单击左侧的叠加图标，然后选择&#x200B;**[!UICONTROL 导航]**。

   ![](assets/selectorrail.png)

1. 从左侧的脱轨中，选择&#x200B;**[!UICONTROL 文件]**。

   ![](assets/access_files.png)

1. 从Brand Portal界面中，选择要共享的文件夹。

   ![](assets/share-folders.png)

1. 从顶部的工具栏中，选择&#x200B;**[!UICONTROL 共享]**。

   ![](assets/share_icon.png)

   将显示[!UICONTROL 文件夹属性]控制台。

   ![](assets/folder_properties.png)

1. 在&#x200B;**[!UICONTROL 文件夹属性]**&#x200B;控制台中，如果不希望向用户显示默认名称，请在&#x200B;**[!UICONTROL 文件夹标题]**&#x200B;字段中指定文件夹标题。
1. 从&#x200B;**[!UICONTROL 添加用户]**&#x200B;列表中，选择要与其共享文件夹的用户或组，然后单击&#x200B;**[!UICONTROL 添加]**。
要仅与来宾用户共享文件夹，而不与其他用户共享文件夹，请从**[!UICONTROL 成员]**&#x200B;下拉菜单中选择&#x200B;**[!UICONTROL 匿名用户]**。

   ![](assets/only-anonymous.png)

   >[!NOTE]
   >
   >要使所有用户（不论其用户组成员身份和角色）都可以使用该文件夹，请选中&#x200B;**[!UICONTROL 公用文件夹]**&#x200B;复选框，以将其公开。

1. 如有必要，单击&#x200B;**[!UICONTROL 更改缩略图]**&#x200B;以修改文件夹的缩略图。
1. 单击&#x200B;**[!UICONTROL 保存]**。

1. 要访问共享文件夹，请使用您与之共享文件夹的用户的凭据登录到Brand Portal。 查看界面中的共享文件夹。

## 取消共享文件夹{#unshare-the-folders}

要取消共享以前共享的文件夹，请执行以下步骤：

1. 从Brand Portal界面中，选择要取消共享的文件夹。

   ![](assets/share-folders-1.png)

1. 在顶部的工具栏中，单击&#x200B;**[!UICONTROL 共享]**。
1. 在&#x200B;**[!UICONTROL 文件夹属性]**&#x200B;控制台的&#x200B;**[!UICONTROL 成员]**&#x200B;下，单击用户旁边的&#x200B;**[!UICONTROL x]**&#x200B;符号，将其从您与共享文件夹的用户列表中删除。

   ![](assets/folder_propertiesunshare.png)

1. 在警告消息框中，单击&#x200B;**[!UICONTROL 确认]**以确认取消共享。
单击**[!UICONTROL 保存]**。

1. 使用您从共享列表中删除的用户的凭据登录到Brand Portal。 该文件夹不再在用户的品牌门户界面中可用。
