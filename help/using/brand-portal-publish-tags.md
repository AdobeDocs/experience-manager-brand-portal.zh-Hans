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
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Publish tags to Brand Portal {#publish-tags-to-brand-portal}

了解如何将标记从 [!DNL AEM] 资产发布到 [!DNL Brand Portal]。

标记在组织资产时非常有用，并增强与资产关联的资产的可搜索性。可以将标记视为随资产附加的关键字或标签(元数据)，并允许在搜索结果中快速找到资产。要了解如何将标记分配到资产中 [!DNL AEM] 的资产，请参考 [使用标记来组织资产](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets)。

标记(与资产和集合关联)在 [!DNL AEM]将关联标记 [!DNL Brand Portal] 发布到 [!DNL Brand Portal]关联的资产(和集合)时自动发布到。已发布的标记有助于搜索查找关联资产。

>[!NOTE]
>
>但是，建议仅在发布标记与之关联的资产(和集合) [!DNL Brand Portal] 之前，才将其发布到发布。这可以确保更快地将资产(和集合)发布 [!DNL Brand Portal]到。

## Manage tags {#manage-tags}

您可以使用预存在的标记附加到资产或从 [!DNL AEM] “标记”控制台中创建新标记(**工具||标记||[!DNL AEM]标记**)。在这两种情况下，您首先必须将标记发布到相应的 [!DNL Brand Portal] 资产，然后将其与相应资产关联。

要在上创建标记 [!DNL AEM]，在上 [!DNL Brand Portal]发布标记并将标记与相应资产(或集合)关联，请按照以下步骤操作：

1. **创建标记**&#x200B;以管理权限登录 [!DNL AEM] 到作者实例，并从全局导航访问 **[!DNL AEM]“标记** ”控制台：

   1. 选择 **工具**

   2. 选择 **常规**

   3. 选择 **标记**

2. 选择 **创建** ，然后选择 **创建标记** 选项。
3. 指定：

   * **标题**
      *(必需)* 标记的显示标题。
   * **名称**
      *(必需)* 标记的名称。如果未指定，则从标题中创建有效的节点名称。请参阅 [TagID](https://helpx.adobe.com/experience-manager/6-5/sites/developing/using/framework.html#TagID)。
   * **描述**
      *(可选)* 标记的说明。
   * **标记路径** JCR路径。

4. 选择 **提交** 以创建标记。

   [!DNL AEM] 在实例上创建了标记后，将可将标记附加到资产(使用该资产的“属性”部分或“管理标记”部分)。

5. **将标记发布[!DNL Brand Portal]**&#x200B;到。

   转到 **[!DNL AEM]“标记** ”控制台(工具||标记|| [!DNL AEM] 标记)，选择所需的标记和发布到 **[!DNL Brand Portal]**。

6. **将标记附加到资产(或集合)**。

   选择资产(或集合)，然后使用资产的“属性”部分或“管理标记”部分附加所需的标记。要了解有关如何将标记分配到 [!DNL AEM] 资产中资产的更多信息，请参阅 [使用标记组织资产](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets)。

7. **将资产(或集合)发布到[!DNL Brand Portal]**。\
   当您将资产(或集合)发布到 [!DNL Brand Portal]时，附加的标记 [!DNL Brand Portal]也可用。

   要查看相应资产(或集合)上的附加标记 [!DNL Brand Portal]，请登录 [!DNL Brand Portal] 并选择资产，在属性部分下，您将看到附加的标记。

## 搜索提升 {#search-promote}

[!DNL AEM] 资产 [!DNL Brand Portal] 允许您将特定资产作为基于关键字标签进行搜索的主要结果。

要提升搜索关键字的资产，请按照以下步骤操作：

1. 在创作实例上打开资产的 **“属性**[!DNL AEM] ”页面。
2. 转到 **高级** 选项卡。
3. 在 ******提升搜索关键字** 部分的“提升”中，选择 **“添加”** 以添加搜索关键字或标记。

   ![](assets/search-promote.png)

4. 保存更改。
5. Publish the asset to [!DNL Brand Portal].
6. [!DNL Brand Portal]登录到。在 **资产****的属性** 部分查看高级选项卡。
请注意 **，Search Promotion** 关键字也在该资产的属性中可见。
