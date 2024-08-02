---
title: 共享文件夹
description: Brand Portal要求从预配置的Experience Manager Assets创作实例发布资源。 只有在使用Experience Manager设置复制期间进行了配置时，非管理员用户才能访问已发布的资源，并且资源必须与其共享。
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
exl-id: d28cf927-60e8-437e-9cba-92f7e19020e7
source-git-commit: 32a67abf466dd3bf635b851b02377ed23591915e
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 1%

---

# 在Brand Portal上共享文件夹 {#share-folders}

由于Assets不支持资源摄取，因此需要从预配置的Experience Manager创作实例将Brand Portal发布到Brand Portal。

## Brand Portal中的文件夹共享工作流程 {#folder-sharing-workflow-in-brand-portal}

下面介绍了文件夹共享工作流和用户访问权限：

* 默认情况下，从Experience Manager Assets发布到Brand Portal的所有文件夹仅对Brand Portal管理员可见，除非在配置复制时标记为公用。
* 管理员使用&#x200B;**[!UICONTROL 文件夹属性]**&#x200B;控制台与选择性用户或组共享文件夹。 只有与其共享文件夹的用户或组在登录到Brand Portal后才能看到该文件夹。 其他用户看不到该文件夹。
* 管理员还可以选择通过&#x200B;**[!UICONTROL 文件夹属性]**&#x200B;控制台中的&#x200B;**[!UICONTROL 公用文件夹]**&#x200B;复选框将文件夹设为公用。 所有用户都可以看到公共文件夹。

* 无论用户角色和权限如何，当用户登录到Brand Portal时，都会看到所有公共文件夹，以及直接与他们共享或与他们所属的组共享的文件夹。 所有用户都看不到专用文件夹或与其他用户共享的文件夹。

### 在Brand Portal上与用户组共享文件夹 {#sharing-folders-with-user-groups-on-brand-portal}

文件夹资产的访问权限取决于其父文件夹的访问权限，而不管子文件夹的设置如何。 AEM中的[ACL](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/security/security)控制此行为，子文件夹从其父文件夹继承ACL。 例如，假设文件夹A包含文件夹B，其中包含文件夹C。然后，对文件夹A具有访问权限的用户组（或用户）对文件夹B和文件夹C也具有相同的访问权限。文件夹B是A的子文件夹，文件夹C是B的子文件夹，它继承了ACL。

同样，有权仅访问文件夹B的用户组（或用户）对文件夹C而不是文件夹A具有相同的访问权限。Adobe建议组织内容，以便将最公开的资源放在子文件夹中，从而允许从子文件夹一直到根文件夹的访问权限受到限制。

### 公共文件夹发布 {#public-folder-publish}

只有在配置AEM Assets复制期间选择了&#x200B;**[!UICONTROL 公用文件夹Publish]**&#x200B;选项时，非管理员用户（例如编辑者和查看者）才能访问从Brand Portal发布到Brand Portal的资源。

![](assets/assetbpreplication.png)

如果&#x200B;**[!UICONTROL 公用文件夹Publish]**&#x200B;选项已禁用，则管理员需要使用共享功能专门与非管理员用户共享这些资源。

>[!NOTE]
>
>启用&#x200B;**[!UICONTROL 公用文件夹Publish]**&#x200B;的选项在AEM 6.3.2.1及更高版本中可用。

## 访问共享文件夹 {#access-to-shared-folders}

以下矩阵讨论了各种用户角色的访问权限以及共享或取消共享资产的权限：

|               | 访问从AEM Assets发布到Brand Portal的所有文件夹 | 访问共享文件夹 | 共享或取消共享文件夹权限 |
|---------------|-----------|-----------|------------|
| 管理员 | 是 | 是 | 是 |
| 编辑器 | 否* | 是，仅当与他们共享或与他们所属的组共享时 | 是，仅适用于与其共享或与所属组共享的文件夹 |
| 查看者 | 否* | 是，仅当与他们共享或与他们所属的组共享时 | 否 |
| 来宾用户 | 否* | 是，仅当与他们共享或与他们所属的组共享时 | 否 |

>[!NOTE]
>
>默认情况下，在使用AEM Author配置Brand Portal复制时，**[!UICONTROL 公用文件夹Publish]**&#x200B;选项处于禁用状态。 如果启用了选项，则所有用户（非管理员用户）默认情况下都可以访问发布到Brand Portal的文件夹。

### 非管理员用户对共享文件夹的访问权限 {#non-admin-user-access-to-shared-folders}

非管理员用户只能访问在Brand Portal上与他们共享的文件夹。 但是，这些文件夹在登录时在门户上的显示方式取决于&#x200B;**[!UICONTROL 启用文件夹层次结构]**&#x200B;配置的设置。

**如果配置被禁用**

登录到Brand Portal后，非管理员用户可在登陆页面上看到与其共享的所有文件夹。

![](assets/disabled-folder-hierarchy1-1.png)

**如果配置已启用**

登录Brand Portal时，非管理员用户会看到文件夹树（从根文件夹开始）以及在其各自的父文件夹内排列的共享文件夹。

这些父文件夹是虚拟文件夹，无法对它们执行任何操作。 您可以使用锁图标来识别这些虚拟文件夹。

与共享文件夹不同，在&#x200B;**[!UICONTROL 卡片视图]**&#x200B;中悬停或选择操作任务时不会显示任何操作任务。 在&#x200B;**[!UICONTROL 列视图]**&#x200B;和&#x200B;**[!UICONTROL 列表视图]**&#x200B;中选择虚拟文件夹时显示&#x200B;**[!UICONTROL 概述]**&#x200B;按钮。

>[!NOTE]
>
>请注意，虚拟文件夹的默认缩略图是第一个共享文件夹的缩略图图像。

![](assets/enabled-hierarchy1-1.png) ![](assets/hierarchy1-nonadmin-1.png) ![](assets/hierarchy-nonadmin-1.png) ![](assets/hierarchy2-nonadmin-1.png)

## 共享文件夹 {#how-to-share-folders}

要与Brand Portal上的用户共享文件夹，请执行以下步骤：

1. 单击左侧的叠加图标，然后选择&#x200B;**[!UICONTROL 导航]**。

   ![](assets/selectorrail.png)

1. 从左侧的边栏中选择&#x200B;**[!UICONTROL 文件]**。

   ![](assets/access_files.png)

1. 在Brand Portal界面中，选择要共享的文件夹。

   ![](assets/share-folders.png)

1. 从顶部的工具栏中选择&#x200B;**[!UICONTROL 共享]**。

   ![](assets/share_icon.png)

   出现[!UICONTROL 文件夹属性]控制台。

   ![](assets/folder_properties.png)

1. 如果您不希望向用户显示默认名称，请在&#x200B;**[!UICONTROL 文件夹属性]**&#x200B;控制台的&#x200B;**[!UICONTROL 文件夹标题]**&#x200B;字段中指定文件夹标题。
1. 从&#x200B;**[!UICONTROL 添加用户]**&#x200B;列表中，选择要与其共享文件夹的用户或组，然后单击&#x200B;**[!UICONTROL 添加]**。
要仅与来宾用户共享文件夹，而不与其他用户共享，请从**[!UICONTROL 成员]**&#x200B;下拉列表中选择&#x200B;**[!UICONTROL 匿名用户]**。

   ![](assets/only-anonymous.png)

   >[!NOTE]
   >
   >若要使文件夹对所有用户可用，而不考虑其组成员资格和角色，请选中&#x200B;**[!UICONTROL 公用文件夹]**&#x200B;复选框，以将其设为公用文件夹。

1. 如有必要，请单击&#x200B;**[!UICONTROL 更改缩略图]**&#x200B;以修改文件夹的缩略图图像。
1. 单击&#x200B;**[!UICONTROL 保存]**。

1. 要访问共享文件夹，请使用与其共享该文件夹的用户的凭据登录Brand Portal。 在界面中查看共享文件夹。

## 取消共享文件夹 {#unshare-the-folders}

要取消共享以前共享的文件夹，请执行以下步骤：

1. 在Brand Portal界面中，选择要取消共享的文件夹。

   ![](assets/share-folders-1.png)

1. 在顶部的工具栏中，单击&#x200B;**[!UICONTROL 共享]**。
1. 在&#x200B;**[!UICONTROL 文件夹属性]**&#x200B;控制台的&#x200B;**[!UICONTROL 成员]**&#x200B;下，单击用户旁边的&#x200B;**[!UICONTROL x]**&#x200B;符号，将其从共享文件夹的用户列表中删除。

   ![](assets/folder_propertiesunshare.png)

1. 在警告消息框中，单击&#x200B;**[!UICONTROL 确认]**以确认取消共享。
单击**[!UICONTROL 保存]**。

1. 使用您从共享列表中删除的用户的凭据登录Brand Portal。 该文件夹在Brand Portal界面中不再可供用户使用。
