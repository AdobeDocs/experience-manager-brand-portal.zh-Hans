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
source-git-commit: 770c353b1143d879280df310012ce9d4d30b40c9

---


# 将预设、架构和彩块化发布到Brand Portal {#publish-presets-schema-and-facets-to-brand-portal}

本文介绍将 [!DNL AEM] “作者”实例中的图像预设、元数据架构和自定义搜索彩块化发布 [!DNL Brand Portal]到。发布功能使组织能够重复使用 [!DNL AEM] 在创作实例中创建/修改的图像预设、元数据架构和搜索彩块化，从而减少重复工作。

>[!NOTE]
>
>可以从 [!DNL AEM] 作者实例发布图像预设、元数据架构和搜索彩块化的功能 [!DNL Brand Portal][!DNL AEM 6.2 SP1-CFP7] 可用 [!DNL AEM 6.3 SP 1-CFP 1 (6.3.1.1)] 。

## 将图像预设发布到Brand Portal {#publish-image-presets-to-brand-portal}

图像预设是一组大小调整和格式设置命令，这些命令在图像交付时应用于图像。可以在以下位置创建和修改图像预设 [!DNL Brand Portal]。或者 [!DNL AEM] ，如果作者实例在动态媒体模式下运行，则用户可以在 [!DNL AEM] 作者处创建预设并将其发布到 [!DNL AEM Assets Brand Portal]，并避免在上重新创建相同的预设 [!DNL Brand Portal]。\
创建预设后，该预设在资产详细信息演绎版边栏和下载对话框上作为动态演绎版列出。

>[!NOTE]
>
>[!DNL AEM] 如果作者实例未在 [!DNL Dynamic Media] 模式中运行(客户尚未购买 [!DNL Dynamic Media])，则不会在上传时创建资产 [!UICONTROL 的金字塔TIFF] 演绎版。图像预设或动态演绎版在资产 [!UICONTROL 的金字塔TIFF] 上工作，因此如果  在作者实例上 [!DNL AEM] 不提供Moundid TIFF，则也不可使用 [!DNL Brand Portal] 该预设。因此，资产详细信息页面的演绎版边栏中没有动态演绎版，并下载对话框。

要将图像预设发布 [!DNL Brand Portal]到：

1. 在 [!DNL AEM] 创作实例中，点按/单击徽标 [!DNL AEM] 以访问全局导航控制台，然后点按/单击工具图标，然后导航到 **[!UICONTROL 资产]** &gt; **[!UICONTROL 图像预设]**。
2. 从图像预设列表中选择图像预设或多个图像预设，然后单击/点按 **[!UICONTROL 发布到Brand Portal]**。

![](assets/publishpreset.png)

>[!NOTE]
>
>当用户单击 **[!UICONTROL “发布到品牌门户”]** 时，图像预设将排队等待发布。建议用户监控复制代理的日志，以确认发布是否成功。

要将图像预设取消发布 [!DNL Brand Portal]，请执行以下操作：

1. 在 [!DNL AEM] 创作实例中，点按/单击徽标 [!DNL AEM] 以访问全局导航控制台，然后点按/单击工具图标，然后导航到 **[!UICONTROL 资产]** &gt; **[!UICONTROL 图像预设]**。
2. 选择图像预设，然后从顶部可用的选项中选择 **[!UICONTROL “从Brand Portal]** 删除”。

## 将元数据架构发布到Brand Portal {#publish-metadata-schema-to-brand-portal}

元数据架构描述了资产/集合的属性页面上显示的布局和属性。

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

如果用户已编辑作者实例上 [!DNL AEM] 的默认架构，并且愿意使用与上默认架构相同的架构 [!DNL Brand Portal]，则只需将元数据架构表单发布 [!DNL Brand Portal]到。在此类情况下，默认架构 [!DNL Brand Portal] 由 [!DNL AEM] 从作者实例发布的默认架构覆盖。

如果用户在作者实例上 [!DNL AEM] 创建了自定义架构，则他们可以将自定义架构发布到该模式 [!DNL Brand Portal] ，而不是在那里重新创建相同的自定义架构。然后，用户可以将此自定义架构应用到其中的任何文件夹/集合 [!DNL Brand Portal]。

>[!NOTE]
>
>无法将默认架构发布到 [!DNL Brand Portal][!DNL AEM] 在实例中锁定的(即未编辑它们)。

![](assets/default-schema-form.png)

>[!NOTE]
>
>如果某个文件夹在“作者实例”上 [!DNL AEM] 应用了某个架构，则也必须存在相同的架构， [!DNL Brand Portal] 以保持 [!DNL AEM] “作者”和 [!DNL Brand portal]“作者”上资产属性页面的一致性。

要将元数据架构从 [!DNL AEM] 作者实例发布 [!DNL Brand Portal]到：

1. 在 [!DNL AEM] 创作实例中，点按/单击AEM徽标以访问全局导航控制台，然后点按/单击工具图标，然后导航到 **[!UICONTROL 资产]** &gt; **[!UICONTROL 元数据架构]**。
2. 选择元数据架构，然后从顶部可用的选项中选择 **[!UICONTROL 发布到Brand Portal]** 。

>[!NOTE]
>
>当用户单击 **[!UICONTROL “发布到品牌门户”]**&#x200B;时，元数据架构将排队等待发布。建议用户监控复制代理的日志，以确认发布是否成功。

要将元数据架构取消发布 [!DNL Brand Portal]，请执行以下操作：

1. 在 [!DNL AEM] 创作实例中，点按/单击徽标 [!DNL AEM] 以访问全局导航控制台，然后点按/单击工具图标，然后导航到 **[!UICONTROL 资产]** &gt; **[!UICONTROL 元数据架构]**。
2. 选择元数据架构，然后从顶部可用的选项中选择 **[!UICONTROL “从Brand Portal]** 删除”。

## 将搜索彩块化发布到Brand Portal {#publish-search-facets-to-brand-portal}

搜索表单可为用户提供 [彩块化搜索](../using/brand-portal-search-facets.md) 的功能 [!DNL Brand Portal]。搜索彩块化具有更大的搜索粒度 [!DNL Brand Portal]。在搜索 [表单中添加](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-facets.html#AddingaPredicate) 的所有谓词均可在搜索过滤器中作为搜索彩块化供用户使用。

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

如果您愿意从作者实例使用自定义搜索表单 **[!UICONTROL 资产管理搜索边栏]**[!DNL AEM] ，则无需重新创建同一表单， [!DNL Brand Portal] 即可将自定义搜索表单从 [!DNL AEM] 作者实例发布到 [!DNL Brand Portal]。

>[!NOTE]
>
>除非已编辑AEM资产，否则无法将锁定的搜索表单 **[!UICONTROL 资产管理搜索边栏]** 发布到AEM [!DNL Brand Portal] 资产。编辑并发布到 [!DNL Brand Portal]该搜索表单后，此搜索表单将覆盖搜索表单 [!DNL Brand Portal]。

要将已编辑的搜索facet从 [!DNL AEM] 作者实例发布 [!DNL Brand Portal]到：

1. 点按/单击 [!DNL AEM] 徽标，然后转到 **[!UICONTROL 工具]** &gt; **[!UICONTROL 常规]** &gt; **[!UICONTROL 搜索表单]**。
2. 选择编辑后的搜索表单，然后选择 **[!UICONTROL 发布到Brand Portal]**。

   >[!NOTE]
   >
   >当用户单击 **[!UICONTROL “发布到品牌门户”]**&#x200B;时，搜索彩块化将排队等待发布。建议用户监控复制代理的日志，以确认发布是否成功。

要取消发布搜索表单 [!DNL Brand Portal]，请执行以下操作：

1. 在 [!DNL AEM] 创作实例中，点按/单击 [!DNL AEM] 徽标以访问全局导航控制台，然后点按/单击工具图标，然后导航到 **[!UICONTROL 常规]** &gt; **[!UICONTROL 搜索表单]**。
2. 选择搜索表单，然后从顶部可用的选项中选择 **[!UICONTROL “从Brand Portal]** 删除”。

>[!NOTE]
>
>“从Brand Portal **[!UICONTROL 取消发布”]** 操作将保留Brand Portal上的默认搜索表单，且不会恢复到发布前使用的上一个搜索表单。

### 限制 {#limitations}

1. 很少的搜索谓词不适用于在上搜索过滤器 [!DNL Brand Portal]。当这些搜索谓词作为搜索表单的一部分从 [!DNL AEM] 作者实例中发布时，它们 [!DNL Brand Portal]会被过滤掉。因此，用户在已发布的表单中看到的谓词数量较少 [!DNL Brand Portal]。请参阅 [适用于Brand Portal上筛选器的搜索谓词](../using/brand-portal-search-facets.md#list-of-search-predicates)。

2. [!UICONTROL 对于“选项] ”谓词，如果用户使用任何自定义路径在AEM作者实例中阅读选项，则在Brand Portal中不起作用。这些附加路径和选项不会通过搜索表单发布到Brand Portal。在这种情况下，用户可以在 **[!UICONTROL 选项]** 谓词中 **[!UICONTROL 的“添加选项]** ”中 **[!UICONTROL 选择“手动]** ”选项，以手动添加这些选项 [!DNL Brand Portal]。

![](assets/options-predicate-manual.png)
