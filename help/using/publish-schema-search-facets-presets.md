---
title: 将预设、架构和 Facet 发布到 Brand Portal
seo-title: Publish presets, schema, and facets to Brand Portal
description: 了解如何将预设、架构和Facet发布到Brand Portal。
seo-description: Learn how to publish presets, schema, and facets to Brand Portal.
uuid: c836d9bb-074a-4113-9c91-b2bf7658b88d
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: bc305abc-9373-4d33-9179-0a5f3904b352
exl-id: 9b585606-6538-459b-87a9-2e68df0087b3
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '1141'
ht-degree: 2%

---

# 将预设、架构和 Facet 发布到 Brand Portal {#publish-presets-schema-and-facets-to-brand-portal}

本文深入探讨了将图像预设、元数据架构和自定义搜索彩块化从AEM创作实例发布到Brand Portal。 发布功能使组织能够重用在AEM创作实例中创建/修改的图像预设、元数据架构和搜索Facet，从而减少重复工作。

>[!NOTE]
>
>从AEM 6.2 SP1-CFP7和AEM 6.3 SP 1-CFP 1 (6.3.1.1)开始，将图像预设、元数据架构和搜索Facet从AEM创作实例发布到Brand Portal的功能可用。

## 将图像预设发布到Brand Portal {#publish-image-presets-to-brand-portal}

图像预设是在图像投放时应用于图像的一组大小调整和格式命令。 可在Brand Portal中创建和修改图像预设。 或者，如果AEM创作实例在Dynamic Media模式下运行，则用户可以在AEM创作中创建预设并将其发布到AEM Assets Brand Portal，并避免在Brand Portal中重新创建相同的预设。\
创建预设后，该预设将作为动态演绎版列在资源详细信息演绎版边栏和下载对话框中。

>[!NOTE]
>
>如果AEM创作实例未在中运行 **[!UICONTROL Dynamic Media模式]** (客户尚未购买Dynamic Media)，则 **[!UICONTROL 金字塔TIFF]**  上传时不会创建资产的演绎版。 图像预设或动态演绎版可用于 **[!UICONTROL 金字塔TIFF]** ，因此，如果 **[!UICONTROL 金字塔TIFF]** 在AEM创作实例上不可用，则在Brand Portal上也不可用。 因此，资产详细信息页面和下载对话框的演绎版边栏中不存在动态演绎版。

要将图像预设发布到Brand Portal，请执行以下操作：

1. 在AEM创作实例中，点按/单击AEM徽标以访问全局导航控制台，然后点按/单击工具图标并导航到 **[!UICONTROL 资产>图像预设]**.
1. 从图像预设列表中选择图像预设或多个图像预设，然后单击/点按 **[!UICONTROL 发布到Brand Portal]**.

![](assets/publishpreset.png)

>[!NOTE]
>
>当用户单击时 **[!UICONTROL 发布到Brand Portal]** 图像预设已排队等待发布。 建议用户监视复制代理的日志，以确认发布是否成功。

要从Brand Portal取消发布图像预设，请执行以下操作：

1. 在AEM创作实例中，点按/单击AEM徽标以访问全局导航控制台，然后点按/单击 **[!UICONTROL 工具]** 图标并导航到 **[!UICONTROL 资产>图像预设]**.
1. 选择图像预设，然后选择 **[!UICONTROL 从Brand Portal中删除]** 从顶部可用的选项中选择。

## 将元数据架构发布到Brand Portal  {#publish-metadata-schema-to-brand-portal}

元数据架构描述资产/收藏集的属性页面上显示的布局和属性。

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

如果用户已编辑AEM创作实例上的默认架构，并且愿意使用与Brand Portal上的默认架构相同的架构，则他们只需将元数据架构表单发布到Brand Portal即可。 在此类场景中，Brand Portal的默认架构会被从AEM创作实例发布的默认架构覆盖。

如果用户在AEM创作实例上创建自定义架构，则他们可以将自定义架构发布到Brand Portal，而不是在那里重新创建相同的自定义架构。 然后，用户可将此自定义架构应用于Brand Portal中的任何文件夹/收藏集。

>[!NOTE]
>
>如果默认架构在AEM实例中被锁定（即未编辑），则无法将其发布到Brand Portal。

![](assets/default-schema-form.png)

>[!NOTE]
>
>如果文件夹在AEM Author实例上应用了架构，则Brand Portal上也必须存在相同的架构，以保持AEM Author和Brand Portal上“资产属性”页面的一致性。

要将元数据架构从AEM创作实例发布到Brand Portal，请执行以下操作：

1. 在AEM创作实例中，点按/单击AEM徽标以访问全局导航控制台，然后点按/单击工具图标并导航到 **[!UICONTROL Assets >元数据架构]**.
1. 选择元数据架构，然后选择 **[!UICONTROL 发布到Brand Portal]** 从顶部可用的选项中选择。

>[!NOTE]
>
>当用户单击时 **[!UICONTROL 发布到Brand Portal]**，则元数据架构将排队等待发布。 建议用户监视复制代理的日志，以确认发布是否成功。

要从Brand Portal中取消发布元数据架构，请执行以下操作：

1. 在AEM创作实例中，点按/单击AEM徽标以访问全局导航控制台，然后点按/单击工具图标并导航到 **[!UICONTROL Assets >元数据架构]**.
1. 选择元数据架构，然后选择 **[!UICONTROL 从Brand Portal中删除]** 从顶部可用的选项中选择。

## 将搜索Facet发布到Brand Portal {#publish-search-facets-to-brand-portal}

搜索表单提供以下功能 [分面搜索](../using/brand-portal-search-facets.md) Brand Portal上的用户。 搜索Facet可为Brand Portal上的搜索提供更精细的粒度。 所有 [已添加谓词](https://experienceleague.adobe.com/docs/experience-manager-65/assets/administer/search-facets.html) 对于用户，搜索表单中的维度可用作搜索筛选器中的搜索Facet。

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

如果您愿意使用自定义搜索表单 **[!UICONTROL 资产管理搜索边栏]** 然后，您可以将自定义搜索表单从AEM创作实例发布到Brand Portal，而不是在Brand Portal上重新创建相同的表单。

>[!NOTE]
>
>锁定的搜索表单 **[!UICONTROL 资产管理搜索边栏]** 除非进行编辑，否则无法将on AEM Assets发布到Brand Portal。 编辑并发布到Brand Portal后，此搜索表单将覆盖Brand Portal上的搜索表单。

要将编辑后的搜索Facet从AEM创作实例发布到Brand Portal，请执行以下操作：

1. 点按/单击 AEM 徽标，然后转到&#x200B;**[!UICONTROL 工具 > 常规 > 搜索表单]**。
1. 选择编辑的搜索表单，然后选择 **[!UICONTROL 发布到Brand Portal]**.

   >[!NOTE]
   >
   >当用户单击时 **[!UICONTROL 发布到Brand Portal]**，则搜索Facet将排队等待发布。 建议用户监视复制代理的日志，以确认发布是否成功。

要从Brand Portal中取消发布搜索表单，请执行以下操作：

1. 在AEM创作实例中，点按/单击AEM徽标以访问全局导航控制台，然后点按/单击工具图标并导航到 **[!UICONTROL 常规>搜索Forms]**.
1. 选择搜索表单，然后选择 **[!UICONTROL 从Brand Portal中删除]** 从顶部可用的选项中选择。

>[!NOTE]
>
>此 **[!UICONTROL 从Brand Portal取消发布]** 操作会保留Brand Portal上的默认搜索表单，并且不会恢复到发布前使用的最后一个搜索表单。

### 限制 {#limitations}

1. 很少有搜索谓词不适用于Brand Portal上的搜索过滤器。 当这些搜索谓词作为搜索表单的一部分从AEM创作实例发布到Brand Portal时，会被过滤掉。 因此，用户在Brand Portal上看到的已发布表单中的谓词数量较少。 参见 [适用于Brand Portal上的过滤器的搜索谓词](../using/brand-portal-search-facets.md#list-of-search-predicates).

1. 对象 [!UICONTROL 选项谓词]，如果用户在AEM Author实例中使用任何自定义路径来读取选项，它将无法在Brand Portal中使用。 这些附加路径和选项未使用搜索表单发布到Brand Portal。 在这种情况下，用户可以选择 **[!UICONTROL 手动]** 中的选项 **[!UICONTROL 添加选项]** 范围 **[!UICONTROL 选项谓词]** 以在Brand Portal中手动添加这些选项。

![](assets/options-predicate-manual.png)
