---
title: 将标记发布到 Brand Portal
seo-title: 将标记发布到 Brand Portal
description: 了解如何将标记从AEM Assets发布到Brand Portal。
seo-description: 了解如何将标记从AEM Assets发布到Brand Portal。
uuid: 4167367e-1af8-476b-97a5-730c43bd0816
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: 3c8e9251-195d-4c56-a9a9-27bc8b2a82a4
translation-type: tm+mt
source-git-commit: 86d4d5c358ea795e35db2dce8c9529ed14e9ee2d
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 4%

---


# 将标记发布到 Brand Portal {#publish-tags-to-brand-portal}

了解如何将标记从AEM Assets发布到Brand Portal。

标记可用于组织资产并增强与资产关联的资产的可搜索性。 标记可以视为与资产附加的关键字或标签（元数据），并允许在搜索结果中快速找到资产。 要了解如何为AEM Assets的资产分配标记，请参阅[使用标记来组织资产](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets)。

当具有关联标记的资产（和集合）发布到Brand Portal时，标记(与AEM中的资产和集合关联)会自动发布到Brand Portal。 发布的标记有助于搜索找到相关资产。

>[!NOTE]
>
>但是，建议在发布与标记关联的资产（和集合）之前，只将标记发布到Brand Portal。 这可确保将资产（和集合）更快地发布到Brand Portal。

## 管理标记{#manage-tags}

您可以使用预先存在的标记附加到资产或从AEM标记控制台创建新标记(**[!UICONTROL 工具 |标记 | AEM标记]**)。 在这两种情况下，您必须先将标记发布到Brand Portal，然后将其与相应的资产关联。

要在AEM上创建标记，请在Brand Portal上发布标记，并将标记与相应的资产（或集合）关联，请按照以下步骤操作：

1. **创建**
标记以管理权限登录到AEM作者实例，并从全局导航 **[!UICONTROL 访]** 问AEM Tagsconsole:

   1. 选择&#x200B;**[!UICONTROL 工具]**

   1. 选择&#x200B;**[!UICONTROL 常规]**

   1. 选择&#x200B;**[!UICONTROL 标记]**

1. 选择&#x200B;**[!UICONTROL 创建]**，然后选择&#x200B;**[!UICONTROL 创建标记]**&#x200B;选项。
1. 指定：

   * **[!UICONTROL 标题]**

      *（必需）* 标记的显示标题。
   * **[!UICONTROL 名称]**
      *（必需）* 标记的名称。如果未指定，则从标题创建有效节点名称。 请参阅[TagID](https://helpx.adobe.com/experience-manager/6-5/sites/developing/using/framework.html#TagID)。
   * **描述**

      *（可选）* 标记的说明。
   * **标**
记PathJCR标记路径。

1. 选择&#x200B;**[!UICONTROL 提交]**&#x200B;以创建标记。

   在AEM实例上创建标记后，该标记便可以附加到资产（使用该资产的“属性”部分或“管理标记”部分）。

1. **将标记发布到Brand Portal**。

   转到&#x200B;**[!UICONTROL AEM标记]**&#x200B;控制台([!UICONTROL 工具 |标记 | AEM标记])，选择所需的标记并发布到品牌门户。

1. **将标记附加到资产（或集合）**。

   选择一个资产（或集合），然后使用该资产的属性部分或管理标记部分附加所需的标记。 要详细了解如何为AEM Assets的资产分配标记，请参阅[使用标记来组织资产](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets)。

1. **将资产（或集合）发布到Brand Portal**。\
   将资产（或集合）发布到Brand Portal时，Brand Portal中也提供附加的标记。

   要在Brand Portal中查看相应资产（或集合）上的附加标记，请登录Brand Portal并选择资产，在“属性”部分下，您将看到附加的标记。

## 搜索提升 {#search-promote}

AEM Assets品牌门户允许您根据关键字标签将特定资产作为搜索的最佳结果。

要提升搜索关键字的资产，请执行以下步骤：

1. 打开AEM作者实例上资产的&#x200B;**[!UICONTROL 属性]**&#x200B;页。
1. 转至&#x200B;**[!UICONTROL 高级]**&#x200B;选项卡。
1. 在&#x200B;**[!UICONTROL 提升搜索关键字]**&#x200B;部分的&#x200B;**[!UICONTROL 搜索提升]**&#x200B;中，选择&#x200B;**[!UICONTROL 添加]**&#x200B;以添加搜索关键字或标记。

   ![](assets/search-promote.png)

1. 保存更改。
1. 将资产发布到 Brand Portal.
1. 登录Brand Portal。 视图&#x200B;**[!UICONTROL 资产**[!UICONTROL &#x200B;属性&#x200B;]**部分的高级]**选项卡。
请注意，**[!UICONTROL 搜索提升]**&#x200B;关键字也会显示在该资产的属性中。
