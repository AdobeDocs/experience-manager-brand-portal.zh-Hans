---
title: 将预设、架构和 Facet 发布到 Brand Portal
seo-title: 将预设、架构和 Facet 发布到 Brand Portal
description: 了解如何将预设、模式和彩块化发布到Brand Portal。
seo-description: 了解如何将预设、模式和彩块化发布到Brand Portal。
uuid: c836d9bb-074a-4113-9c91-b2bf7658b88d
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: bc305abc-9373-4d33-9179-0a5f3904b352
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873
workflow-type: tm+mt
source-wordcount: '1160'
ht-degree: 3%

---


# 将预设、架构和 Facet 发布到 Brand Portal {#publish-presets-schema-and-facets-to-brand-portal}

文章将从AEM作者实例向品牌门户发布图像预设、元数据模式和自定义搜索彩块化。 发布功能使组织能够重复使用在AEM作者实例中创建／修改的图像预设、元数据模式和搜索彩块化，从而减少重复工作。

>[!NOTE]
>
>从AEM 6.2 SP1-CFP7和AEM 6.3 SP 1-CFP 1(6.3.1.1)开始，可将图像预设、元数据模式和搜索彩块化从AEM作者实例发布到品牌门户。

## 将图像预设发布到Brand Portal {#publish-image-presets-to-brand-portal}

图像预设是一组调整大小和设置格式的命令，这些命令在图像投放时应用于图像。 可以在品牌门户中创建和修改图像预设。 或者，如果AEM作者实例以动态媒体模式运行，则用户可以在AEM作者处创建预设并将其发布到AEM Assets品牌门户，并避免在品牌门户重新创建相同的预设。\
创建预设后，资产详细信息演绎版边栏和下载对话框中的预设将作为动态演绎版列出。

>[!NOTE]
>
>如果AEM作者实例未在&#x200B;**[!UICONTROL Dynamic Media Mode]**&#x200B;中运行（客户尚未购买Dynamic Media），则上传时不会创建资产的&#x200B;**[!UICONTROL 金字塔TIFF]**&#x200B;再现。 图像预设或动态演绎版适用于资产的&#x200B;**[!UICONTROL 金字塔TIFF]**，因此，如果&#x200B;**[!UICONTROL 金字塔TIFF]**&#x200B;在AEM作者实例中不可用，则它也不适用于品牌门户。 因此，资产详细信息页面和下载对话框的演绎版边栏中不存在动态演绎版。

要将图像预设发布到Brand Portal，请执行以下操作：

1. 在AEM作者实例中，点按／单击AEM徽标以访问全局导航控制台，然后点按／单击工具图标并导航到&#x200B;**[!UICONTROL 资产>图像预设]**。
1. 从图像预设列表中选择图像预设或多个图像预设，然后单击／点按&#x200B;**[!UICONTROL 发布到品牌门户]**。

![](assets/publishpreset.png)

>[!NOTE]
>
>当用户单击&#x200B;**[!UICONTROL 发布到Brand Portal]**&#x200B;时，图像预设将排队等待发布。 建议用户监视复制代理的日志以确认发布是否成功。

要从Brand Portal取消发布图像预设，请执行以下操作：

1. 在AEM作者实例中，点按／单击AEM徽标以访问全局导航控制台，然后点按／单击&#x200B;**[!UICONTROL 工具]**&#x200B;图标，然后导航到&#x200B;**[!UICONTROL 资产>图像预设]**。
1. 选择图像预设，然后从顶部的可用选项中选择&#x200B;**[!UICONTROL 从Brand Portal]**&#x200B;删除。

## 将元数据模式发布到Brand Portal {#publish-metadata-schema-to-brand-portal}

元数据模式描述资产／收藏集的属性页面上显示的布局和属性。

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

如果用户已编辑AEM Author实例上的默认模式，并且愿意使用与Brand Portal上的默认模式相同的模式，则他们只需将元数据模式表单发布到Brand Portal。 在这种情况下，Brand Portal的默认模式由从AEM Author实例发布的默认模式过度。

如果用户已在AEM作者实例上创建自定义模式，则他们可以将自定义模式发布到Brand Portal，而不是在Brand Portal上重新创建相同的自定义模式。 然后，用户可以将此自定义模式应用到Brand Portal中的任何文件夹／集合。

>[!NOTE]
>
>如果默认模式锁定在AEM实例中（即它们未编辑），则无法将其发布到品牌门户。

![](assets/default-schema-form.png)

>[!NOTE]
>
>如果某个文件夹在AEM作者实例上应用了模式，则该模式还必须存在于品牌门户上，以便在AEM作者和品牌门户的资产属性页面中保持一致。

要将元数据模式从AEM作者实例发布到Brand Portal，请执行以下操作：

1. 在AEM作者实例中，点按／单击AEM徽标以访问全局导航控制台，然后点按／单击工具图标，导航至&#x200B;**[!UICONTROL 资产>元数据模式]**。
1. 选择元数据模式，然后从顶部的可用选项中选择&#x200B;**[!UICONTROL 发布到品牌门户]**。

>[!NOTE]
>
>当用户单击&#x200B;**[!UICONTROL 发布到Brand Portal]**&#x200B;时，元数据模式将排队等待发布。 建议用户监视复制代理的日志以确认发布是否成功。

要从Brand Portal取消发布元数据模式，请执行以下操作：

1. 在AEM作者实例中，点按／单击AEM徽标以访问全局导航控制台，然后点按／单击工具图标，导航至&#x200B;**[!UICONTROL 资产>元数据模式]**。
1. 选择元数据模式，然后从顶部的可用选项中选择&#x200B;**[!UICONTROL 从Brand Portal]**&#x200B;删除。

## 将搜索彩块化发布到Brand Portal {#publish-search-facets-to-brand-portal}

搜索表单为品牌门户上的用户提供[多面搜索](../using/brand-portal-search-facets.md)的功能。 搜索彩块化可为品牌门户上的搜索提供更高的粒度。 搜索表单中添加的[谓词](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-facets.html#AddingaPredicate)对于用户来说，在搜索过滤器中作为搜索彩块化可用。

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

如果您愿意从AEM作者实例使用自定义搜索表单&#x200B;**[!UICONTROL 资产管理员搜索边栏]**，则无需在品牌门户上重新创建相同的表单，即可将自定义搜索表单从AEM作者实例发布到品牌门户。

>[!NOTE]
>
>锁定的搜索表单&#x200B;**[!UICONTROL AEM Assets上的资产管理员搜索边栏]**&#x200B;无法发布到品牌门户，除非对其进行编辑。 编辑并发布到Brand Portal后，此搜索表单将覆盖Brand Portal上的搜索表单。

要将已编辑的搜索facet从AEM作者实例发布到Brand Portal，请执行以下操作：

1. 点按/单击 AEM 徽标，然后转到&#x200B;**[!UICONTROL 工具 > 常规 > 搜索表单]**。
1. 选择已编辑的搜索表单，然后选择&#x200B;**[!UICONTROL 发布到品牌门户]**。

   >[!NOTE]
   >
   >当用户单击&#x200B;**[!UICONTROL 发布到Brand Portal]**&#x200B;时，搜索彩块化将排队等待发布。 建议用户监视复制代理的日志以确认发布是否成功。

要从Brand Portal取消发布搜索表单，请执行以下操作：

1. 在AEM作者实例中，点按／单击AEM徽标以访问全局导航控制台，然后点按／单击工具图标并导航到&#x200B;**[!UICONTROL 常规>搜索Forms]**。
1. 选择搜索表单，然后从顶部的可用选项中选择&#x200B;**[!UICONTROL 从Brand Portal]**&#x200B;删除。

>[!NOTE]
>
>**[!UICONTROL 从Brand Portal]**&#x200B;取消发布操作会保留Brand Portal上的默认搜索表单，并且不会恢复到发布前使用的最后一个搜索表单。

### 限制 {#limitations}

1. 少数搜索谓词不适用于品牌门户上的搜索过滤器。 当这些搜索谓词作为搜索表单的一部分从AEM作者实例发布到Brand Portal时，它们会被过滤掉。 因此，用户在品牌门户上的已发布表单中看到的谓词数量较少。 请参阅[搜索适用于品牌门户](../using/brand-portal-search-facets.md#list-of-search-predicates)上的过滤器的谓词。

1. 对于[!UICONTROL 选项谓词]，如果用户在AEM作者实例中使用任何自定义路径读取选项，则该路径在Brand Portal中将无效。 这些附加路径和选项不会随搜索表单一起发布到Brand Portal。 在这种情况下，用户可以在&#x200B;**[!UICONTROL 选项谓词]**&#x200B;中选择&#x200B;**[!UICONTROL 添加选项]**&#x200B;中的&#x200B;**[!UICONTROL 手动]**&#x200B;选项，以在品牌门户中手动添加这些选项。

![](assets/options-predicate-manual.png)
