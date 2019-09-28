---
title: 将标记发布到Brand Portal
seo-title: 将标记发布到Brand Portal
description: 了解如何将标记从AEM资产发布到Brand Portal。
seo-description: 了解如何将标记从AEM资产发布到Brand Portal。
uuid: 4167367e-1af8-476b-97a5-730c43bd0816
topic-tags: 发布
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: 引用
discoiquuid: 3c8e9251-195d-4c56-a9a9-27bc8b2a82a4
translation-type: tm+mt
source-git-commit: 86d4d5c358ea795e35db2dce8c9529ed14e9ee2d

---


# Publish tags to Brand Portal {#publish-tags-to-brand-portal}

了解如何将标记从AEM资产发布到Brand Portal。

标记可用于组织资产并增强与其关联的资产的可搜索性。 可以将标记视为与资产一起附加的关键字或标签（元数据），并允许在搜索后快速找到资产。 要了解如何在AEM资产中为资产分配标记，请参 [阅使用标记来组织资产](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets)。

当具有关联标记的资产（和集合）发布到Brand Portal时，标记（与AEM中的资产和集合关联）会自动发布到Brand Portal。 发布的标记有助于搜索找到相关的资产。

>[!NOTE]
>
>但是，建议在发布与标记关联的资产（和集合）之前，只将标记发布到Brand Portal。 这可以确保将资产（和集合）更快地发布到Brand Portal。

## Manage tags {#manage-tags}

您可以使用预先存在的标记附加到资产，或从AEM标记控制台创建新标记(工&#x200B;**[!UICONTROL 具)|标记| AEM标记]**)。 在这两种情况下，您必须首先将标记发布到Brand Portal，然后将其与相应的资产关联。

要在AEM上创建标记，请在Brand Portal上发布标记，并将标记与相应的资产（或集合）关联，请按照以下步骤操作：

1. **创建标记**&#x200B;以管理权限登录到AEM作者实例，并从全局导航中访 **** 问AEM标记控制台：

   1. 选择工 **[!UICONTROL 具]**

   1. 选择一 **[!UICONTROL 般]**

   1. 选择标 **[!UICONTROL 记]**

1. 选择 **[!UICONTROL 创建]** ，然后选择 **[!UICONTROL 创建标记]** 。
1. 指定：

   * **[!UICONTROL 标题]**
      *（必需）* 标记的显示标题。
   * **[!UICONTROL 名称]**
      *（必需）* 标记的名称。 如果未指定，则从标题创建有效的节点名称。 请参 [阅TagID](https://helpx.adobe.com/experience-manager/6-5/sites/developing/using/framework.html#TagID)。
   * **描述**
      *（可选）* ，标记的说明。
   * **标记路径** JCR标记路径。

1. 选择 **[!UICONTROL 提交]** ，以创建标记。

   在AEM实例上创建标记后，该标记便可以附加到资产（使用该资产的“属性”部分或“管理标记”部分）。

1. **将标记发布到Brand Portal**。

   转到 **[!UICONTROL AEM标记控制台]** (工[!UICONTROL 具|标记| AEM标记])，选择所需的标记并发布到Brand Portal。

1. **将标记附加到资产（或集合）**。

   选择一个资产（或收藏集），然后使用该资产的“属性”部分或“管理标记”部分附加所需的标记。 要详细了解如何在AEM资产中为资产分配标记，请参阅 [使用标记来组织资产](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets)。

1. **将资产（或集合）发布到Brand Portal**。\
   将资产（或集合）发布到Brand Portal时，Brand Portal上也提供附加的标记。

   要在Brand Portal中查看相应资产（或集合）上的附加标记，请登录到Brand Portal并选择资产，在“属性”部分下，您将看到附加的标记。

## 搜索提升 {#search-promote}

通过AEM Assets Brand Portal，您可以根据关键字标记将特定资产作为搜索的最佳结果。

要提升搜索关键字的资产，请执行以下步骤：

1. 在AEM作 **[!UICONTROL 者实例上]** ，打开资产的“属性”页面。
1. 转到“高 **[!UICONTROL 级]** ”选项卡。
1. 在“提 **[!UICONTROL 升搜索关键字]** ”部分 **[!UICONTROL 的“搜索提升”中]** ，选择 **[!UICONTROL “添加]** ”以添加搜索关键字或标记。

   ![](assets/search-promote.png)

1. 保存更改。
1. 将资产发布到 Brand Portal.
1. 登录到Brand Portal。 查 **[!UICONTROL 看资产]** “属 **[!UICONTROL 性”部分的]** “高级”选项卡。
请注意，搜 **[!UICONTROL 索提升]** 关键字也显示在该资产的属性中。
