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
exl-id: 842656a6-1a2b-4b64-954d-1e663923a1a1
source-git-commit: d2bfd06f8cd8a9e78efbc8dd92880e0faae39176
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 4%

---

# 将标记发布到 Brand Portal {#publish-tags-to-brand-portal}

了解如何将标记从AEM Assets发布到Brand Portal。

标记可用于组织资产并增强与其关联的资产的可搜索性。 标记可以视为与资产附加的关键字或标签（元数据），并允许在搜索结果中快速找到资产。 要了解如何为AEM Assets中的资产分配标记，请参阅[使用标记来组织资产](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets)。

将具有关联标记的资产（和收藏集）发布到Brand Portal时，标记(与AEM中的资产和收藏集关联)会自动发布到Brand Portal。 发布的标记有助于搜索以查找关联的资产。

>[!NOTE]
>
>但是，建议在发布与标记关联的资产（和收藏集）之前，只将标记发布到Brand Portal。 这可确保更快地将资产（和收藏集）发布到Brand Portal。

## 管理标记{#manage-tags}

您可以使用预先存在的标记附加到资产，或从AEM标记控制台(**[!UICONTROL 工具 |标记 | AEM标记]**)。 在这两种情况下，您必须先将标记发布到Brand Portal，然后将它们与相应的资产相关联。

要在AEM上创建标记，在Brand Portal上发布标记，并将标记与相应的资产（或收藏集）相关联，请执行以下步骤：

1. **创建**
标记使用管理权限登录到AEM创作实例，并从全局导航 **[!UICONTROL 中]** 访问AEM Tagsconsole:

   1. 选择&#x200B;**[!UICONTROL 工具]**

   1. 选择&#x200B;**[!UICONTROL 常规]**

   1. 选择&#x200B;**[!UICONTROL Tagging]**

1. 选择&#x200B;**[!UICONTROL 创建]**，然后选择&#x200B;**[!UICONTROL 创建标记]**&#x200B;选项。
1. 指定：

   * **[!UICONTROL 标题]**

      *（必需）* 标记的显示标题。
   * **[!UICONTROL 名称]**
      *（必需）* 标记的名称。如果未指定，则从标题中创建有效的节点名称。 请参阅[TagID](https://helpx.adobe.com/experience-manager/6-5/sites/developing/using/framework.html#TagID)。
   * **描述**

      *（可选）* 标记的描述。
   * **标**
记的PathJCR路径。

1. 选择&#x200B;**[!UICONTROL Submit]**&#x200B;以创建标记。

   在AEM实例上创建标记后，该标记便可附加到资产（使用该资产的属性部分或管理标记部分）。

1. **将标记发布到Brand Portal**。

   转到&#x200B;**[!UICONTROL AEM Tags]**&#x200B;控制台([!UICONTROL 工具 |标记 | AEM标记])，选择所需的标记并发布到Brand Portal。

1. **将标记附加到资产（或收藏集）**。

   选择一个资产（或收藏集），然后使用该资产的属性部分或管理标记部分附加所需的标记。 要详细了解如何为AEM Assets中的资产分配标记，请参阅[使用标记来组织资产](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets)。

1. **将资产（或收藏集）发布到Brand Portal**。\
   将资产（或收藏集）发布到Brand Portal时，附加的标记也会在Brand Portal上可用。

   要在Brand Portal中查看相应资产（或集合）上附加的标记，请登录Brand Portal并选择资产，在属性部分下，您将看到附加的标记。

## 搜索提升 {#search-promote}

AEM Assets Brand Portal允许您根据关键字标记使特定资产成为搜索的最热门结果。

要提升搜索关键词的资产，请执行以下步骤：

1. 在AEM创作实例上打开资产的&#x200B;**[!UICONTROL 属性]**&#x200B;页面。
1. 转到&#x200B;**[!UICONTROL Advanced]**&#x200B;选项卡。
1. 在&#x200B;**[!UICONTROL Search Promote]**（位于&#x200B;**[!UICONTROL Evelate for search keywords]**&#x200B;部分）中，选择&#x200B;**[!UICONTROL Add]**&#x200B;以添加搜索关键词或标签。

   ![](assets/search-promote.png)

1. 保存更改。
1. 将资产发布到 Brand Portal.
1. 登录Brand Portal。 查看资产&#x200B;**[!UICONTROL 属性]**&#x200B;部分中的&#x200B;**[!UICONTROL 高级]**选项卡。
请注意，**[!UICONTROL Search Promote]**&#x200B;关键字也显示在该资产的属性中。
