---
title: 将预设、架构和彩块化发布到Brand Portal
seo-title: 将预设、架构和彩块化发布到Brand Portal
description: 了解如何将预设、架构和彩块化发布到Brand Portal。
seo-description: 了解如何将预设、架构和彩块化发布到Brand Portal。
uuid: c836d9bb-074a-4113-9c91-b2bf7658b88d
topic-tags: 发布
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: 引用
discoiquuid: bc305abc-9373-4d33-9179-0a5f3904b352
translation-type: tm+mt
source-git-commit: 86d4d5c358ea795e35db2dce8c9529ed14e9ee2d

---


# 将预设、架构和彩块化发布到Brand Portal {#publish-presets-schema-and-facets-to-brand-portal}

文章涉及将图像预设、元数据架构和自定义搜索彩块化从AEM作者实例发布到Brand Portal。 发布功能使组织能够重复使用在AEM作者实例中创建／修改的图像预设、元数据架构和搜索彩块化，从而减少重复工作。

>[!NOTE]
>
>从AEM作者实例到Brand Portal发布图像预设、元数据架构和搜索彩块化的功能可从AEM 6.2 SP1-CFP7和AEM 6.3 SP 1-CFP 1(6.3.1.1)开始使用。

## 将图像预设发布到Brand Portal {#publish-image-presets-to-brand-portal}

Image presets are a set of sizing and formatting commands that are applied to the image at the time of image delivery. Image presets can be created and modified at Brand Portal. Alternatively, if AEM Author instance is running in dynamic media mode then users can create presets at the AEM Author and publish them to AEM Assets Brand Portal, and avoid re-creating the same presets at Brand Portal.\
Once the preset is created, it is listed as dynamic rendition on asset detail renditions rail and download dialogue.

>[!NOTE]
>
>如果AEM作者实例未在 [!UICONTROL Dynamic Media模式下运行] （客户尚未购买Dynamic Media），则上传时不会创建资产的 [!UICONTROL Pyramid TIFF] 再现。 图像预设或动态演绎版适用于资产的 [!UICONTROL Pyramid TIFF] ，因此，如果 [!UICONTROL Pyramid TIFF] 在AEM作者实例中不可用，则Brand Portal中也不可用。 As a result of this, no dynamic renditions are present in renditions rail of asset details page and download dialogue.

要将图像预设发布到Brand Portal，请执行以下操作：

1. 在AEM作者实例中，点按／单击AEM徽标以访问全局导航控制台，然后点按／单击工具图标，然后导航到资产 **[!UICONTROL &gt;图]** 像预设 ****。
1. 从图像预设列表中选择一个或多个图像预设，然后单击／点按发布 **[!UICONTROL 到品牌门户]**。

![](assets/publishpreset.png)

>[!NOTE]
>
>当用户单击 **[!UICONTROL 发布到Brand Portal时]** ，图像预设将排队等待发布。 建议用户监视复制代理的日志以确认发布是否成功。

要从Brand Portal取消发布图像预设，请执行以下操作：

1. 在AEM作者实例中，点按／单击AEM徽标以访问全局导航控制台，然后点按／单击工具图标，然后导航到 **[!UICONTROL Assets]** &gt; **[!UICONTROL Image Presets]**。
1. 选择图像预设，然后从 **[!UICONTROL 顶部的可用选项中选择]** “从Brand Portal删除”。

## 将元数据架构发布到Brand Portal {#publish-metadata-schema-to-brand-portal}

元数据架构描述资产／集合的属性页面上显示的布局和属性。

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

如果用户已在AEM作者实例上编辑了默认架构，并且愿意使用与Brand Portal上的默认架构相同的架构，则他们只需将元数据架构表单发布到Brand Portal。 在这种情况下，Brand Portal的默认架构由从AEM作者实例发布的默认架构过度使用。

如果用户已在AEM作者实例上创建了自定义架构，则他们可以将自定义架构发布到Brand Portal，而不是在那里重新创建相同的自定义架构。 然后，用户可以将此自定义架构应用到Brand Portal中的任何文件夹／集合。

>[!NOTE]
>
>Default schemas cannot be published to the Brand Portal if they are locked at the AEM instance (that is they are unedited).

![](assets/default-schema-form.png)

>[!NOTE]
>
>如果文件夹已在AEM作者实例上应用了架构，则品牌门户上也必须存在相同的架构，以保持AEM作者和品牌门户上的资产属性页面的一致性。

要将元数据架构从AEM作者实例发布到Brand Portal，请执行以下操作：

1. 在AEM作者实例中，点按／单击AEM徽标以访问全局导航控制台，然后点按／单击工具图标，然后导航到资产&gt;元 **[!UICONTROL 数据架构]**。
1. Select a metadata schema, and select Publish to Brand Portal from the options available at the top.****

>[!NOTE]
>
>When users click Publish to Brand Portal, the metadata schemas are queued for publishing. **** Users are advised to monitor the log of the replication agents to confirm if the publish was successful.

要从Brand Portal取消发布元数据架构，请执行以下操作：

1. 在AEM作者实例中，点按／单击AEM徽标以访问全局导航控制台，然后点按／单击工具图标，然后导航到资产&gt;元 **[!UICONTROL 数据架构]**。
1. Select a metadata schema, and select Remove from Brand Portal from the options available at the top.****

## Publish search facets to Brand Portal {#publish-search-facets-to-brand-portal}

Search forms provide the capability of faceted search to users on Brand Portal. [](../using/brand-portal-search-facets.md)Search facets impart greater granularity to searches on Brand Portal. All the predicates added in the search form are available to users as search facets in search filters.[](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-facets.html#AddingaPredicate)

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

如果您愿意从AEM作者实例中使用自定义搜索表单资产管理搜索边栏 **** ，则您可以将自定义搜索表单从AEM作者实例发布到Brand Portal，而不是在Brand Portal上重新创建同一表单。

>[!NOTE]
>
>AEM资产上锁定 **[!UICONTROL 的搜索表单资产管理搜索边栏]** （除非已编辑）无法发布到Brand Portal。 编辑并发布到Brand Portal后，此搜索表单将覆盖Brand Portal上的搜索表单。

要将编辑后的搜索facet从AEM作者实例发布到Brand Portal，请执行以下操作：

1. 点按／单击AEM徽标，然后转到工具 **** &gt;常规 **[!UICONTROL &gt;搜]** 索表单 ****。
1. Select the edited search form, and select Publish to Brand Portal.****

   >[!NOTE]
   >
   >当用户单击“ **[!UICONTROL 发布到品牌门户”时]**，搜索彩块化将排队等待发布。 建议用户监视复制代理的日志以确认发布是否成功。

要从Brand Portal取消发布搜索表单，请执行以下操作：

1. In AEM Author instance, tap/ click the AEM logo to access the global navigation console and tap/click the Tools icon and navigate to General &gt; Search Forms.****
1. Select the search form, and select Remove from Brand Portal from the options available at the top.****

>[!NOTE]
>
>“从 **[!UICONTROL Brand Portal取消发布]** ”操作会在Brand Portal上保留默认的搜索表单，但不会恢复到发布前使用的最后一个搜索表单。

### 限制 {#limitations}

1. Few search predicates are not applicable to search filters on the Brand Portal. When these search predicates are published as part of the search form from AEM Author instance to Brand Portal, they are filtered out. 因此，用户在品牌门户的已发布表单中可看到的谓词数量较少。 See search predicates applicable to filters on Brand Portal.[](../using/brand-portal-search-facets.md#list-of-search-predicates)

1. 对于 [!UICONTROL 选项谓词]，如果用户在AEM作者实例中使用任何自定义路径读取选项，则它在Brand Portal中将无法使用。 这些附加路径和选项不会随搜索表单一起发布到Brand Portal。 在这种情况下，用户可以在“选项 **[!UICONTROL 谓词”中]** 的“添加选项 **[!UICONTROL ”中选择“手]****** 动”选项，以在Brand Portal手动添加这些选项。

![](assets/options-predicate-manual.png)
