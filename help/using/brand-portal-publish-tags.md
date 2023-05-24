---
title: 将标记发布到 Brand Portal
seo-title: Publish tags to Brand Portal
description: 了解如何将标记从Experience Manager Assets发布到Brand Portal。
seo-description: Learn how to publish tags from Experience Manager Assets to Brand Portal.
uuid: 4167367e-1af8-476b-97a5-730c43bd0816
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: 3c8e9251-195d-4c56-a9a9-27bc8b2a82a4
exl-id: 842656a6-1a2b-4b64-954d-1e663923a1a1
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 4%

---

# 将标记发布到 Brand Portal {#publish-tags-to-brand-portal}

了解如何将标记从Experience Manager Assets发布到Brand Portal。

标记可用于组织资源并提高与其关联的资源的可搜索性。 标记可以视为与资产附加的关键字或标签（元数据），并允许作为搜索结果快速找到资产。 要了解如何在Experience Manager Assets中为资产分配标记，请参阅 [使用标记来组织资源](https://experienceleague.adobe.com/docs/experience-manager-65/assets/managing/organize-assets.html).

将带有关联标记的资产（和收藏集）发布到Brand Portal后，标记(与AEM中的资产和收藏集关联)会自动发布到Brand Portal。 发布的标记有助于使搜索功能查找关联的资产。

>[!NOTE]
>
>但是，建议在发布与标记关联的资产（和收藏集）之前，仅将标记发布到Brand Portal。 这可确保将资产（和收藏集）更快发布到Brand Portal。

## 管理标记 {#manage-tags}

您可以使用预先存在的标记附加到资产，或从AEM Tags控制台创建新标记(**[!UICONTROL 工具 |标记 | AEM标记]**)。 在这两种情况下，您必须先将标记发布到Brand Portal，然后将它们与相应的资产关联。

要在AEM上创建标记，请在Brand Portal上发布标记，并将标记与相应的资产（或收藏集）相关联，请执行以下步骤：

1. **创建标记**
使用管理权限登录AEM创作实例并获取访问权限 **[!UICONTROL AEM标记]** 控制台来自全局导航：

   1. 选择 **[!UICONTROL 工具]**

   1. 选择 **[!UICONTROL 常规]**

   1. 选择 **[!UICONTROL 标记]**

1. 选择 **[!UICONTROL 创建]** 然后选择 **[!UICONTROL 创建标记]** 选项。
1. 指定：

   * **[!UICONTROL 标题]**

      *（必需）* 标记的显示标题。
   * **[!UICONTROL 名称]**
      *（必需）* 标记的名称。 如果未指定，则从标题创建有效的节点名称。 参见 [标记ID](https://experienceleague.adobe.com/docs/experience-manager-65/developing/platform/tagging/framework.html).
   * **描述**

      *（可选）* 标记的描述。
   * **标记路径**
标记的JCR路径。

1. 选择 **[!UICONTROL 提交]** 以创建标记。

   在AEM实例上创建标记后，该标记将附加到资源中（使用该资源的“属性”部分或“管理标记”部分）。

1. **将标记发布到Brand Portal**.

   转到 **[!UICONTROL AEM标记]** 控制台([!UICONTROL 工具 |标记 | AEM标记])，选择所需的标记并发布到Brand Portal。

1. **将标记附加到资产（或收藏集）**.

   选择一个资产（或收藏集），然后使用该资产的“属性”部分或“管理标记”部分附加所需的标记。 要详细了解如何在AEM Assets中为资产分配标记，请参阅 [使用标记来组织资源](https://experienceleague.adobe.com/docs/experience-manager-65/assets/managing/organize-assets.html).

1. **将资源（或收藏集）发布到Brand Portal**.\
   在将资产（或收藏集）发布到Brand Portal时，附加的标记也在Brand Portal上可用。

   要在Brand Portal中查看相关资产（或收藏集）上的附加标记，请登录Brand Portal并选择资产，在“属性”部分下，您将看到附加的标记。

## 搜索提升 {#search-promote}

AEM Assets Brand Portal允许您将特定资源作为基于关键词标记的搜索排名最前的结果。

要提升搜索关键字的资产，请执行以下步骤：

1. 打开 **[!UICONTROL 属性]** AEM创作实例上资源的页面。
1. 转到 **[!UICONTROL 高级]** 选项卡。
1. In **[!UICONTROL 搜索提升]** 范围 **[!UICONTROL 提升搜索关键词]** 部分，选择 **[!UICONTROL 添加]** 以添加搜索关键字或标记。

   ![](assets/search-promote.png)

1. 保存更改。
1. 将资产发布到 Brand Portal.
1. 登录到Brand Portal。 视图 **[!UICONTROL 高级]** 按Tab键进入 **[!UICONTROL 属性]** 资产的部分。
请注意 **[!UICONTROL 搜索提升]** 关键字还在该资产的属性中可见。
