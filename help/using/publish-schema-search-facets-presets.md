---
title: 将预设、架构和 Facet 发布到 Brand Portal
seo-title: 将预设、架构和 Facet 发布到 Brand Portal
description: 了解如何将预设、架构和Facet发布到Brand Portal。
seo-description: 了解如何将预设、架构和Facet发布到Brand Portal。
uuid: c836d9bb-074a-4113-9c91-b2bf7658b88d
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: bc305abc-9373-4d33-9179-0a5f3904b352
exl-id: 9b585606-6538-459b-87a9-2e68df0087b3
source-git-commit: d2bfd06f8cd8a9e78efbc8dd92880e0faae39176
workflow-type: tm+mt
source-wordcount: '1160'
ht-degree: 3%

---

# 将预设、架构和 Facet 发布到 Brand Portal {#publish-presets-schema-and-facets-to-brand-portal}

本文将介绍如何将图像预设、元数据架构和自定义搜索Facet从AEM创作实例发布到Brand Portal。 发布功能使组织能够重复使用在AEM创作实例中创建/修改的图像预设、元数据架构和搜索彩块化，从而减少重复工作。

>[!NOTE]
>
>从AEM 6.2 SP1-CFP7和AEM 6.3 SP 1-CFP 1(6.3.1.1)开始，可以将图像预设、元数据架构和搜索Facet从AEM创作实例发布到Brand Portal。

## 将图像预设发布到Brand Portal {#publish-image-presets-to-brand-portal}

图像预设是一组大小调整和格式设置命令，这些命令在图像交付时应用于图像。 可以在Brand Portal中创建和修改图像预设。 或者，如果AEM创作实例在Dynamic Media模式下运行，则用户可以在AEM创作中创建预设并将其发布到AEM Assets Brand Portal，同时避免在Brand Portal重新创建相同的预设。\
创建预设后，该预设将作为动态演绎版列在资产详细信息演绎版边栏和下载对话框中。

>[!NOTE]
>
>如果AEM创作实例未在&#x200B;**[!UICONTROL Dynamic Media模式]**&#x200B;中运行(客户尚未购买Dynamic Media)，则上传时不会创建资产的&#x200B;**[!UICONTROL Pyramid TIFF]**&#x200B;演绎版。 图像预设或动态演绎版适用于资产的&#x200B;**[!UICONTROL Pyramid TIFF]**，因此，如果&#x200B;**[!UICONTROL Pyramid TIFF]**&#x200B;在AEM创作实例上不可用，则它也在Brand Portal上不可用。 因此，资产详细信息页面和下载对话框的演绎版边栏中不存在动态演绎版。

要将图像预设发布到Brand Portal，请执行以下操作：

1. 在AEM创作实例中，点按/单击AEM徽标以访问全局导航控制台，然后点按/单击工具图标，然后导航到&#x200B;**[!UICONTROL Assets >图像预设]**。
1. 从图像预设列表中选择一个或多个图像预设，然后单击/点按&#x200B;**[!UICONTROL 发布到Brand Portal]**。

![](assets/publishpreset.png)

>[!NOTE]
>
>当用户单击&#x200B;**[!UICONTROL 发布到Brand Portal]**&#x200B;时，图像预设将排入队列进行发布。 建议用户监视复制代理的日志，以确认发布是否成功。

要从Brand Portal取消发布图像预设，请执行以下操作：

1. 在AEM创作实例中，点按/单击AEM徽标以访问全局导航控制台，然后点按/单击&#x200B;**[!UICONTROL 工具]**&#x200B;图标，然后导航到&#x200B;**[!UICONTROL 资产>图像预设]**。
1. 选择图像预设，然后从顶部可用的选项中选择&#x200B;**[!UICONTROL 从Brand Portal中删除]** 。

## 将元数据架构发布到Brand Portal {#publish-metadata-schema-to-brand-portal}

元数据架构描述资产/收藏集的属性页面上显示的布局和属性。

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

如果用户在AEM创作实例上编辑了默认架构，并且愿意使用与Brand Portal上的默认架构相同的架构，则他们只需将元数据架构表单发布到Brand Portal即可。 在这种情况下，Brand Portal的默认架构会被从AEM创作实例发布的默认架构覆盖。

如果用户在AEM创作实例上创建了自定义架构，则他们可以将自定义架构发布到Brand Portal，而不是在此处重新创建相同的自定义架构。 然后，用户可以将此自定义架构应用于Brand Portal中的任何文件夹/收藏集。

>[!NOTE]
>
>如果默认架构在AEM实例处被锁定（即未编辑），则它们无法发布到Brand Portal。

![](assets/default-schema-form.png)

>[!NOTE]
>
>如果文件夹在AEM创作实例上应用了架构，则Brand Portal上还必须存在相同的架构，以保持AEM创作和Brand Portal上资产属性页面的一致性。

要将元数据架构从AEM创作实例发布到Brand Portal，请执行以下操作：

1. 在AEM创作实例中，点按/单击AEM徽标以访问全局导航控制台，然后点按/单击工具图标，然后导航到&#x200B;**[!UICONTROL Assets >元数据架构]**。
1. 选择元数据架构，然后从顶部的可用选项中选择&#x200B;**[!UICONTROL 发布到Brand Portal]** 。

>[!NOTE]
>
>当用户单击&#x200B;**[!UICONTROL 发布到Brand Portal]**&#x200B;时，元数据架构将排队等待发布。 建议用户监视复制代理的日志，以确认发布是否成功。

要从Brand Portal取消发布元数据架构，请执行以下操作：

1. 在AEM创作实例中，点按/单击AEM徽标以访问全局导航控制台，然后点按/单击工具图标，然后导航到&#x200B;**[!UICONTROL Assets >元数据架构]**。
1. 选择元数据架构，然后从顶部可用的选项中选择&#x200B;**[!UICONTROL 从Brand Portal中删除]** 。

## 将搜索彩块化发布到Brand Portal {#publish-search-facets-to-brand-portal}

搜索表单为Brand Portal上的用户提供了[多面搜索](../using/brand-portal-search-facets.md)的功能。 搜索彩块化可为Brand Portal上的搜索提供更大的粒度。 在搜索表单中添加的所有[谓词](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-facets.html#AddingaPredicate)作为搜索筛选器中的搜索彩块化可供用户使用。

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

如果您愿意从AEM创作实例中使用自定义搜索表单&#x200B;**[!UICONTROL 资产管理员搜索边栏]**，则可以将自定义搜索表单从AEM创作实例发布到Brand Portal，而不是在Brand Portal上重新创建相同的表单。

>[!NOTE]
>
>AEM Assets上的锁定搜索表单&#x200B;**[!UICONTROL 资产管理员搜索边栏]**&#x200B;无法发布到Brand Portal，除非对其进行编辑。 编辑并发布到Brand Portal后，此搜索表单将覆盖Brand Portal上的搜索表单。

要将编辑的搜索Facet从AEM创作实例发布到Brand Portal，请执行以下操作：

1. 点按/单击 AEM 徽标，然后转到&#x200B;**[!UICONTROL 工具 > 常规 > 搜索表单]**。
1. 选择编辑后的搜索表单，然后选择&#x200B;**[!UICONTROL 发布到Brand Portal]**。

   >[!NOTE]
   >
   >当用户单击&#x200B;**[!UICONTROL 发布到Brand Portal]**&#x200B;时，搜索彩块化将排入队列进行发布。 建议用户监视复制代理的日志，以确认发布是否成功。

要从Brand Portal取消发布搜索表单，请执行以下操作：

1. 在AEM创作实例中，点按/单击AEM徽标以访问全局导航控制台，然后点按/单击工具图标，然后导航到&#x200B;**[!UICONTROL 常规>搜索Forms]**。
1. 选择搜索表单，然后从顶部可用的选项中选择&#x200B;**[!UICONTROL 从Brand Portal中删除]** 。

>[!NOTE]
>
>**[!UICONTROL 从Brand Portal取消发布]**&#x200B;操作会保留Brand Portal上的默认搜索表单，并且不会恢复到发布前使用的最后一个搜索表单。

### 限制 {#limitations}

1. 很少有搜索谓词不适用于Brand Portal上的搜索过滤器。 当这些搜索谓词作为搜索表单的一部分从AEM创作实例发布到Brand Portal时，它们会被过滤掉。 因此，用户在Brand Portal上的已发布表单中看到的谓词数较少。 请参阅[搜索适用于Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates)上过滤器的谓词。

1. 对于[!UICONTROL 选项谓词]，如果用户在AEM创作实例中使用任何自定义路径读取选项，则该路径在Brand Portal中不起作用。 这些其他路径和选项不会随搜索表单一起发布到Brand Portal。 在这种情况下，用户可以选择&#x200B;**[!UICONTROL **[!UICONTROL &#x200B;选项谓词&#x200B;]**中的添加选项]**&#x200B;中的&#x200B;**[!UICONTROL 手动]**&#x200B;选项，以在Brand Portal中手动添加这些选项。

![](assets/options-predicate-manual.png)
