---
title: 在 Brand Portal 上搜索资产
seo-title: 在AEM Brand Portal上搜索资产并保存搜索
description: Brand Portal搜索功能可让您使用搜索功能快速搜索相关资产，搜索过滤器可帮助您进一步缩小搜索范围。 将搜索保存为智能收藏集以供将来使用。
seo-description: Brand Portal搜索功能可让您使用搜索功能快速搜索相关资产，搜索过滤器可帮助您进一步缩小搜索范围。 将搜索保存为智能收藏集以供将来使用。
uuid: c2955198-bdc0-4853-a13a-661e6a9ec61f
contentOwner: bdhar
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: SearchandPromote
discoiquuid: dc751cd7-f663-46d2-84c4-5bb12a4fe1ba
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873
workflow-type: tm+mt
source-wordcount: '1163'
ht-degree: 5%

---


# 在 Brand Portal 上搜索资产 {#search-assets-on-brand-portal}

Brand Portal搜索功能允许您使用搜索功能快速搜索相关资产，并使用过滤器进行facet搜索以帮助您进一步缩小搜索范围。 您还可以将搜索另存为未来智能收藏集。

## 使用Omnisearch {#search-assets-using-omnisearch}搜索资产

要在Brand Portal上搜索资产，请执行以下操作：

1. 在工具栏中，单击&#x200B;**[!UICONTROL 搜索]**&#x200B;图标，或按“**[!UICONTROL /]**”键启动Omnisearch。

   ![](assets/omnisearchicon-1.png)

1. 在搜索框中，为要搜索的资产键入关键字。

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >搜索过程中至少需要3个字符，以便显示搜索建议。

1. 从下拉列表中显示的相关建议中进行选择，以快速访问相关资产。

   ![](assets/assets-search-result.png)

   *使用全局搜索进行资产搜索*

要了解带有智能标记的资产的搜索行为，请参阅[了解搜索结果和行为](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-assets.html)。

## 在“过滤器”面板{#search-using-facets-in-filters-panel}中使用彩块化进行搜索

过滤器面板中的搜索彩块化为您的搜索体验添加粒度，并提高搜索功能的效率。 搜索彩块化使用多个维度（谓词），使您能够执行复杂的搜索。 您可以轻松地向下展开到所需的详细级别，以便进行更集中的搜索。

例如，如果您要查找图像，则可以选择是要位图还是矢量图像。 您可以通过在文件类型搜索facet中为图像指定MIME类型，进一步缩小搜索范围。 同样，在搜索文档时，可以指定格式，例如PDF或MS Word格式。<br />

![过滤器面板Brand Portal中](assets/file-type-search.png "的“过滤器”面板")

该&#x200B;**[!UICONTROL 过滤器]**&#x200B;面板包括几个标准面，如- **[!UICONTROL 路径浏览器]**、**[!UICONTROL 文件类型]**、**[!UICONTROL 文件大小]**、**[!UICONTROL 状态]**&#x200B;和&#x200B;**[!UICONTROL 方向]**。 但是，您可以[添加自定义搜索彩块化](../using/brand-portal-search-facets.md)或通过在基础搜索表单中添加或删除谓词从&#x200B;**[!UICONTROL 过滤器]**&#x200B;面板中删除特定搜索彩块化。 请参阅品牌门户](../using/brand-portal-search-facets.md#list-of-search-predicates)上可用和可用的[搜索谓词的列表。

要将过滤器应用于搜索，请使用可用的[搜索彩块化](../using/brand-portal-search-facets.md):

1. 单击叠加图标，然后选择&#x200B;**[!UICONTROL 过滤器]**。

   ![](assets/selectorrail.png)

1. 从左侧的&#x200B;**[!UICONTROL 过滤器]**面板中，选择适当的选项以应用相关过滤器。
例如，使用以下标准过滤器:

   * **[!UICONTROL 路径浏]** 览器搜索特定目录中的资产。路径浏览器谓词的默认搜索路径为`/content/dam/mac/<tenant-id>/`，可通过编辑默认搜索表单来配置该路径。
   >[!NOTE]
   >
   >对于非管理员用户，[!UICONTROL 筛选器]面板中的[!UICONTROL 路径浏览器]仅显示与其共享的文件夹（及其上级文件夹）的内容结构。\
   >对于管理用户，路径浏览器允许导航到Brand Portal中的任意文件夹。

   * **[!UICONTROL 文]** 件类型指定您要查找的资源文件的类型(图像、文档、多媒体、存档)。此外，您还可以缩小搜索范围，例如，为文档指定图像或格式（PDF或MS Word）的MIME类型（Tiff、位图、GIMP图像）。
   * **[!UICONTROL 文件]** 大小：根据资产大小搜索资产。您可以指定大小范围的下限和上限以缩小搜索范围并指定要搜索的度量单位。
   * **[!UICONTROL 启]** 动以根据资产状态(如批准（已批准）、请求更改、被拒绝、待定)和到期情况搜索资产。
   * **[!UICONTROL 平均]** 评级：根据资产的评级搜索资产。
   * **[!UICONTROL 方向]** ：根据资产的方向（水平、垂直、正方形）搜索资产。
   * **[!UICONTROL 按]** 样式根据资产的样式（彩色、单色）搜索资产。
   * **[!UICONTROL 视]** 频格式，根据视频资源的格式(DVI、Flash、MPEG4、MPEG、OGG Theora、QuickTime、Windows Media、WebM)搜索视频资源。

   您可以通过编辑基础搜索表单，在“过滤器”面板中使用[自定义搜索彩块化](../using/brand-portal-search-facets.md)。

   * **[!UICONTROL 属性]** 谓词（如果在搜索表单中使用）允许您搜索与谓词所映射到的元数据属性匹配的资产。\
      例如，如果属性谓词已映射到[!UICONTROL `jcr:content /metadata/dc:title`]，则您可以根据资产的标题搜索资产。\
      [!UICONTROL 属性谓词]支持对以下内容进行文本搜索：

      **部分短语**&#x200B;要允许使用属性谓词中的部分短语进行资产搜索，请在“搜索表单”中启用&#x200B;**[!UICONTROL 部分搜索]**&#x200B;复选框。\
      该功能允许您搜索所需的资产，即使您没有指定资产元数据中使用的确切字词/短语。\
      您可以：
      * 在“过滤器”面板的facet中指定搜索短语中出现的单词。 例如，如果搜索词&#x200B;**climb**（属性谓词已映射到[!UICONTROL `dc:title`]属性），则返回标题短语中带有单词&#x200B;**climb**&#x200B;的所有资产。
      * 指定搜索词组中出现的单词的一部分，以及通配符(*)以填充间隙。
例如，搜索：
         * **climb*** 返回所有包含以标题短语中的字符“clim”开头的词的资产。
         * ***** gamping返回标题短语中带有“climb”字符的所有资产。
         * ***climb*返** 回所有包含标题短语中“clim”字符的资源。

要在属性谓词中允许非区分大小写的搜索，请启用       **非区分大小写文**
本要在属性谓词中允许非区分大小写的搜索，请在搜索表 **[!UICONTROL 单中]** 启用“忽略大小写”复选框。默认情况下，属性谓词上的文本搜索区分大小写。
   >[!NOTE]
   >
   >在选中&#x200B;**[!UICONTROL 部分搜索]**&#x200B;复选框时，默认情况下会选中&#x200B;**[!UICONTROL 忽略大小写]**。

   ![](assets/wildcard-prop-1.png)

   根据所应用的过滤器以及搜索结果计数显示搜索结果。

   ![](assets/omnisearch-with-filters.png)

   具有搜索结果计数的资产搜索结果。

1. 您可以轻松地从搜索结果导航到项目，并使用浏览器中的返回按钮返回到相同的搜索结果，而无需重新运行搜索查询。

## 将搜索另存为智能收藏集{#save-your-searches-as-smart-collection}

您可以将搜索设置保存为智能收藏集，以便快速重复相同的搜索，而无需稍后重做相同的设置。

要将搜索设置另存为智能收藏集，请执行以下操作：

1. 点按／单击&#x200B;**[!UICONTROL 保存智能收藏集]**&#x200B;并为智能收藏集提供名称。

   要使所有用户都可以访问该智能集合，请选择&#x200B;**[!UICONTROL 公共]**。 系统会显示一条消息，确认已创建智能收藏集并将其添加到保存的搜索的列表。

   >[!NOTE]
   >
   >非管理员用户可能被禁止公开智能收藏集，以避免在组织的品牌门户上拥有大量由非管理员用户创建的公共智能收藏集。 组织可以禁用&#x200B;**[!UICONTROL 允许从**[!UICONTROL &#x200B;管理工具面板中提供的常规&#x200B;]**设置创建公共智能集合]**&#x200B;配置。

   ![](assets/save_smartcollectionui.png)

1. 要以其他名称保存智能收藏集，并选中或清除&#x200B;**[!UICONTROL 公共]**&#x200B;复选框，请单击&#x200B;**[!UICONTROL 编辑智能收藏集]**。

   ![](assets/edit_smartcollection.png)

1. 在&#x200B;**[!UICONTROL 编辑智能收藏集]**&#x200B;对话框中，选择&#x200B;**[!UICONTROL 另存为]**&#x200B;并输入智能收藏集的名称。 单击&#x200B;**[!UICONTROL 保存]**。

   ![](assets/saveas_smartsearch.png)
