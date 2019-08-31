---
title: 将预设、架构和彩块化发布到Brand Portal
seo-title: 将预设、架构和彩块化发布到Brand Portal
description: 了解如何将预设、架构和彩块化发布到Brand Portal。
seo-description: 了解如何将预设、架构和彩块化发布到Brand Portal。
uuid: c836d9bb-074a-4113-9c91-b2 bf7658 b88 d
topic-tags: 发布
products: SG_ EXPERIENCE MANAGER/Brand_ Portal
content-type: 引用
discoiquuid: bc305abc-9373-4d33-9179-0a5f3904b352
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# 将预设、架构和彩块化发布到Brand Portal {#publish-presets-schema-and-facets-to-brand-portal}

本文介绍将AEM作者实例中的图像预设、元数据架构和自定义搜索彩块化发布到Brand Portal。发布功能使组织能够重用AEM作者实例创建/修改的图像预设、元数据架构和搜索彩块化，从而减少重复工作。

>[!NOTE]
>
>将AEM作者实例中的图像预设、元数据架构和搜索彩块化发布到Brand Portal的功能从AEM6.2SP1-CFP和AEM6.3 SP1-CFP(6.3.1.1)开始。

## 将图像预设发布到Brand Portal {#publish-image-presets-to-brand-portal}

图像预设是一组大小调整和格式设置命令，这些命令在图像交付时应用于图像。可以在Brand Portal中创建和修改图像预设。或者，如果AEM作者实例在动态媒体模式下运行，则用户可以在AEM作者处创建预设并将其发布到AEM Assets Brand Portal，并避免在Brand Portal上重新创建相同预设。\
创建预设后，该预设在资产详细信息演绎版边栏和下载对话框上作为动态演绎版列出。

>[!NOTE]
>
>如果AEM作者实例未在 [!UICONTROL Dynamic Media模式] 下运行(客户尚未购买Dynamic Media)，则不会在上传时创建资产 [!UICONTROL 的金字塔TIFF] 演绎版。图像预设或动态演绎版在资产 [!UICONTROL 的金字塔TIFF] 上工作，因此如果 [!UICONTROL AEM作者实例中不提供金字塔TIFF] ，则也在Brand Portal上不可用。因此，资产详细信息页面的演绎版边栏中没有动态演绎版，并下载对话框。

要将图像预设发布到Brand Portal，请执行以下操作：

1. 在AEM作者实例中，点按/单击AEM徽标以访问全局导航控制台，然后点按/单击工具图标，然后导航到 **[!UICONTROL “资产]** ”&gt; **[!UICONTROL “图像预设]**”。
2. 从图像预设列表中选择图像预设或多个图像预设，然后单击/点按 **[!UICONTROL 发布到Brand Portal]**。

![](assets/publishpreset.png)

>[!NOTE]
>
>当用户单击 **[!UICONTROL “发布到品牌门户”]** 时，图像预设将排队等待发布。建议用户监控复制代理的日志，以确认发布是否成功。

要从Brand Portal中取消发布图像预设，请执行以下操作：

1. 在AEM作者实例中，点按/单击AEM徽标以访问全局导航控制台，然后点按/单击 **[!UICONTROL 工具]** 图标，然后导航到 **[!UICONTROL “资产”&gt;“图像预设]**”。
2. 选择图像预设，然后从顶部可用的选项中选择 **[!UICONTROL “从Brand Portal]** 删除”。

## 将元数据架构发布到Brand Portal {#publish-metadata-schema-to-brand-portal}

元数据架构描述了资产/集合的属性页面上显示的布局和属性。

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

如果用户已在AEM作者实例上编辑默认架构，并且愿意在Brand Portal上使用与默认架构相同的架构，则只需将元数据架构表单发布到Brand Portal即可。在此类情况下，Brand Portal的默认架构由从AEM作者实例发布的默认架构覆盖。

如果用户在AEM作者实例上创建了自定义架构，则可以将自定义架构发布到Brand Portal，而不是在那里重新创建相同的自定义架构。然后，用户可以将此自定义架构应用到Brand Portal中的任何文件夹/集合。

>[!NOTE]
>
>如果在AEM实例中锁定了默认架构(即未编辑它们)，则无法将默认架构发布到品牌门户。

![](assets/default-schema-form.png)

>[!NOTE]
>
>如果某个文件夹在AEM作者实例上应用了某个架构，则品牌门户也必须存在相同的架构，以保持AEM作者和Brand Portal上资产属性页面的一致性。

要将元数据架构从AEM作者实例发布到Brand Portal，请执行以下操作：

1. 在AEM作者实例中，点按/单击AEM徽标以访问全局导航控制台，然后点按/单击工具图标，然后导航到 **[!UICONTROL “资产”&gt;“元数据架构]**”。
2. 选择元数据架构，然后从顶部可用的选项中选择 **[!UICONTROL 发布到Brand Portal]** 。

>[!NOTE]
>
>当用户单击 **[!UICONTROL “发布到品牌门户”]**&#x200B;时，元数据架构将排队等待发布。建议用户监控复制代理的日志，以确认发布是否成功。

要从Brand Portal中取消发布元数据架构，请执行以下操作：

1. 在AEM作者实例中，点按/单击AEM徽标以访问全局导航控制台，然后点按/单击工具图标，然后导航到 **[!UICONTROL “资产”&gt;“元数据架构]**”。
2. 选择元数据架构，然后从顶部可用的选项中选择 **[!UICONTROL “从Brand Portal]** 删除”。

## 将搜索彩块化发布到Brand Portal {#publish-search-facets-to-brand-portal}

搜索表单可为Brand Portal上的用户提供 [彩块化搜索](../using/brand-portal-search-facets.md) 功能。搜索彩块化可提高在Brand Portal上搜索的粒度。在搜索 [表单中添加](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-facets.html#AddingaPredicate) 的所有谓词均可在搜索过滤器中作为搜索彩块化供用户使用。

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

如果您愿意在AEM作者实例中使用自定义搜索表单 **[!UICONTROL Assets Admin Search边栏]** ，而不是在Brand Portal上重新创建相同表单，则可以将自定义搜索表单从AEM作者实例发布到Brand Portal。

>[!NOTE]
>
>除非已编辑AEM资产，否则无法将锁定的搜索表单 **[!UICONTROL 资产管理搜索边栏]** 发布到品牌门户网站。编辑并发布到Brand Portal后，此搜索表单将覆盖Brand Portal上的搜索表单。

要将经过编辑的搜索facet从AEM作者实例发布到Brand Portal，请执行以下操作：

1. 点按/单击AEM徽标，然后转到 **[!UICONTROL 工具]** &gt; **[!UICONTROL 常规]** &gt; **[!UICONTROL 搜索表单]**。
2. 选择编辑后的搜索表单，然后选择 **[!UICONTROL 发布到Brand Portal]**。

   >[!NOTE]
   >
   >当用户单击 **[!UICONTROL “发布到品牌门户”]**&#x200B;时，搜索彩块化将排队等待发布。建议用户监控复制代理的日志，以确认发布是否成功。

要从Brand Portal取消发布搜索表单，请执行以下操作：

1. 在AEM作者实例中，点按/单击AEM徽标以访问全局导航控制台，然后点按/单击工具图标，然后导航到 **[!UICONTROL “常规”&gt;“搜索表单]**”。
2. 选择搜索表单，然后从顶部可用的选项中选择 **[!UICONTROL “从Brand Portal]** 删除”。

>[!NOTE]
>
>“从Brand Portal **[!UICONTROL 取消发布”]** 操作将保留Brand Portal上的默认搜索表单，且不会恢复到发布前使用的上一个搜索表单。

### 限制 {#limitations}

1. 很少的搜索谓词不适用于在Brand Portal上搜索过滤器。当这些搜索谓词作为搜索表单的一部分从AEM作者实例发布到Brand Portal时，它们会被过滤掉。因此，用户在Brand Portal已发布表单中看到的谓词数量较少。请参阅 [适用于Brand Portal上筛选器的搜索谓词](../using/brand-portal-search-facets.md#list-of-search-predicates)。

2. [!UICONTROL 对于“选项谓词]”，如果用户使用任何自定义路径在AEM作者实例中阅读选项，则在Brand Portal中不起作用。这些附加路径和选项不会通过搜索表单发布到Brand Portal。在这种情况下，用户可以在 **[!UICONTROL 选项谓词]** 中 **[!UICONTROL 的“添加选项]** ”中 **[!UICONTROL 选择“手动”选项，]** 以便在Brand Portal手动添加这些选项。

![](assets/options-predicate-manual.png)
