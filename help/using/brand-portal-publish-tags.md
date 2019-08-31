---
title: 将标签发布到Brand Portal
seo-title: 将标签发布到Brand Portal
description: 了解如何将标记从AEM资产发布到Brand Portal。
seo-description: 了解如何将标记从AEM资产发布到Brand Portal。
uuid: 4167367e-1af8-476b-97a5-730c43bd0816
topic-tags: 发布
products: SG_ EXPERIENCE MANAGER/Brand_ Portal
content-type: 引用
discoiquuid: 3c8e9251-195d-4c56-a9 a9-27bc8 b2 a82 a4
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Publish tags to Brand Portal {#publish-tags-to-brand-portal}

了解如何将标记从AEM资产发布到Brand Portal。

标记在组织资产时非常有用，并增强与资产关联的资产的可搜索性。可以将标记视为随资产附加的关键字或标签(元数据)，并允许在搜索结果中快速找到资产。要了解如何在AEM资产中将标记分配给资产，请参考 [使用标记来组织资产](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets)。

当具有关联标记的资产(和集合)发布到Brand Portal时，标记(与AEM中的资产和集合关联)会自动发布到Brand Portal。已发布的标记有助于搜索查找关联资产。

>[!NOTE]
>
>但是，建议在发布标记与之关联的资产(和集合)之前，专门将标记发布到Brand Portal。这可以确保更快地将资产(和集合)发布到Brand Portal。

## Manage tags {#manage-tags}

您可以使用预存在的标记附加到资产或从AEM标记控制台创建新标记(**[!UICONTROL 工具||标记||AEM标记]**)。在这两种情况下，您首先必须将标记发布到Brand Portal，然后将其与相应资产关联。

要在AEM上创建标记，在Brand Portal上发布标记，并将标记与相应的资产(或集合)相关联，请按照以下步骤操作：

1. **创建标记**&#x200B;以管理权限登录AEM作者实例，并从全局导航访问 **[!UICONTROL AEM标记]** 控制台：

   1. 选择 **[!UICONTROL 工具]**

   2. 选择 **[!UICONTROL 常规]**

   3. 选择 **[!UICONTROL 标记]**

2. 选择 **[!UICONTROL 创建]** ，然后选择 **[!UICONTROL 创建标记]** 选项。
3. 指定：

   * **[!UICONTROL 标题]**
      *(必需)* 标记的显示标题。
   * **[!UICONTROL 名称]**
      *(必需)* 标记的名称。如果未指定，则从标题中创建有效的节点名称。请参阅 [TagID](https://helpx.adobe.com/experience-manager/6-5/sites/developing/using/framework.html#TagID)。
   * **描述**
      *(可选)* 标记的说明。
   * **标记路径** JCR路径。

4. 选择 **[!UICONTROL 提交]** 以创建标记。

   在AEM实例上创建了一个标记后，将可将该标记附加到资产(使用该资产的“属性”部分或“管理标记”部分)。

5. **将标记发布到Brand Portal**。

   转到 **[!UICONTROL AEM标记]** 控制台([!UICONTROL 工具||标记||AEM标记])，选择所需标记并发布到Brand Portal。

6. **将标记附加到资产(或集合)**。

   选择资产(或集合)，然后使用资产的“属性”部分或“管理标记”部分附加所需的标记。要详细了解如何在AEM资产中将标记分配给资产，请参阅 [使用标记来组织资产](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets)。

7. **将资产(或集合)发布到Brand Portal**。\
   当您将资产(或集合)发布到Brand Portal时，附加的标记也可在Brand Portal上使用。

   要在Brand Portal中的相应资产(或集合)上看到附加的标记，请登录到Brand Portal并选择资产，在属性部分下，您将看到附加的标记。

## 搜索提升 {#search-promote}

AEM Assets Brand Portal允许您将特定资产作为基于关键字标签进行搜索的主要结果。

要提升搜索关键字的资产，请按照以下步骤操作：

1. 在AEM创作实例上打开资产的 **[!UICONTROL “属性]** ”页面。
2. 转到 **[!UICONTROL 高级]** 选项卡。
3. 在 ******[!UICONTROL 提升搜索关键字]** 部分的“提升”中，选择 **[!UICONTROL “添加”]** 以添加搜索关键字或标记。

   ![](assets/search-promote.png)

4. 保存更改。
5. 将资产发布到 Brand Portal.
6. 登录到Brand Portal。在 **[!UICONTROL 资产]****[!UICONTROL 的属性]** 部分查看高级选项卡。
请注意 **[!UICONTROL ，Search Promotion]** 关键字也在该资产的属性中可见。
