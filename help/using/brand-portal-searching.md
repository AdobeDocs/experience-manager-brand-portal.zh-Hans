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

## 使用Omnisearch搜索资产 {#search-assets-using-omnisearch}

要在Brand Portal上搜索资产，请执行以下操作：

1. 在工具栏中，单 **[!UICONTROL 击]** “搜索”图标，或按&#x200B;**[!UICONTROL “/]**”键启动Omnisearch。

   ![](assets/omnisearchicon-1.png)

1. 在搜索框中，为要搜索的资产键入关键字。

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >搜索过程中至少需要3个字符，以便显示搜索建议。

1. 从下拉列表中显示的相关建议中进行选择，以快速访问相关资产。

   ![](assets/assets-search-result.png)

   *使用全局搜索进行资产搜索*

要了解带有智能标记的资产的搜索行为，请参 [阅了解搜索结果和行为](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-assets.html)。

## 在“过滤器”面板中使用彩块化进行搜索 {#search-using-facets-in-filters-panel}

过滤器面板中的搜索彩块化为您的搜索体验添加粒度，并提高搜索功能的效率。 搜索彩块化使用多个维度（谓词），使您能够执行复杂的搜索。 您可以轻松地向下展开到所需的详细级别，以便进行更集中的搜索。

例如，如果您要查找图像，则可以选择要位图还是矢量图像。 您可以通过在文件类型搜索facet中为图像指定MIME类型，进一步缩小搜索范围。 同样，在搜索文档时，可以指定格式，例如PDF或MS Word格式。<br />

![过滤器面板Brand Portal中](assets/file-type-search.png "的“过滤器”面板")

过滤器 **[!UICONTROL 面板]** 包括几个标准彩块化，如路径浏览器、文件类型 **[!UICONTROL 、文]**&#x200B;件大小、文 **[!UICONTROL 件大小、]**************&#x200B;状态、、和状态。 但是，您可以通 [过在基础搜索表单](../using/brand-portal-search-facets.md) 中添加或删除谓词，在“过滤器”面 **[!UICONTROL 板中添加或删]** 除特定搜索彩块化。 请参阅Brand Portal上可用和可用 [的搜索谓词的列表](../using/brand-portal-search-facets.md#list-of-search-predicates)。

要将过滤器应用于搜索，请使用可用的搜索彩 [块化](../using/brand-portal-search-facets.md):

1. 单击叠加图标，然后选择 **[!UICONTROL 过滤器]**。

   ![](assets/selectorrail.png)

1. 从左 **[!UICONTROL 侧的]** “过滤器”面板中，选择适当的选项以应用相关过滤器。
例如，使用以下标准过滤器:

   * **[!UICONTROL 路径浏览器]** ，用于在特定目录中搜索资产。 路径浏览器的谓词的默认搜索路径是 `/content/dam/mac/<tenant-id>/`，可以通过编辑默认搜索表单来配置。
   >[!NOTE]
   >
   >对于非管理员用户，“筛 [!UICONTROL 选器] ”面板中的路径浏览器仅显示与其共享的文件夹（及其上级文件夹）的内容结构。\
   >对于管理用户，路径浏览器允许导航到Brand Portal中的任意文件夹。

   * **[!UICONTROL 文件类型]** ，以指定您要查找的资源文件的类型(图像、文档、多媒体、存档)。 此外，您还可以缩小搜索范围，例如，为文档指定图像或格式（PDF或MS Word）的MIME类型（Tiff、位图、GIMP图像）。
   * **[!UICONTROL 文件大小]** ：根据资产的大小搜索资产。 您可以指定大小范围的下限和上限以缩小搜索范围并指定要搜索的度量单位。
   * **[!UICONTROL 状态]** ，根据资产状态(如批准（已批准）、请求更改、被拒绝、待定)和到期情况搜索资产。
   * **[!UICONTROL 平均评级]** ：根据资产的评级搜索资产。
   * **[!UICONTROL 方向]** ，根据资产的方向（水平、垂直、正方形）搜索资产。
   * **[!UICONTROL 样式]** ，根据资产的样式（彩色、单色）搜索资产。
   * **[!UICONTROL 视频格式]** ，根据视频资源的格式(DVI、Flash、MPEG4、MPEG、OGG Theora、QuickTime、Windows Media、WebM)搜索视频资源。

   您可以通过 [编辑基础搜索表单](../using/brand-portal-search-facets.md) ，在“过滤器”面板中使用自定义搜索彩块化。

   * **[!UICONTROL 属性谓词]** （如果在搜索表单中使用）允许您搜索与谓词所映射到的元数据属性相匹配的资产。\
      例如，如果属性谓词已映射到，则 [!UICONTROL `jcr:content /metadata/dc:title`]您可以根据资产的标题搜索资产。\
      属 [!UICONTROL 性谓词] ，支持以下文本搜索：

      **部分短语**&#x200B;要允许使用属性谓词中的部分短语进行资产搜索，请在“搜索表单”中启用&#x200B;**[!UICONTROL 部分搜索]**&#x200B;复选框。\
      该功能允许您搜索所需的资产，即使您没有指定资产元数据中使用的确切字词/短语。\
      您可以：
      * 在“过滤器”面板的facet中指定搜索短语中出现的单词。 For example, if you search for the term **climb** (and Property Predicate is mapped to [!UICONTROL `dc:title`] property), then all the assets with the word **climb** in their title phrase are returned.
      * 指定搜索词组中出现的单词的一部分，以及通配符(*)以填充间隙。
例如，搜索：
         * **climb*返回** 所有包含以标题短语中的字符“climb”开头的词的资产。
         * ***clim** 返回标题短语中带有“clim”字符的所有资产。
         * ***climb*返回** 所有包含标题短语中“climb”字符的词的资产。

要在属性谓词中允许非区分大小写的搜索，请启用       **非区分大小写的文本**&#x200B;要在属性谓词中允许非区分大小写的搜索，请在搜索表 **[!UICONTROL 单中启用]** “忽略大小写”复选框。 默认情况下，属性谓词上的文本搜索区分大小写。
   >[!NOTE]
   >
   >选中“部 **[!UICONTROL 分搜索]** ”复选 **[!UICONTROL 框时，默认]** 情况下会选择“忽略大小写”。

   ![](assets/wildcard-prop-1.png)

   根据所应用的过滤器以及搜索结果计数显示搜索结果。

   ![](assets/omnisearch-with-filters.png)

   具有搜索结果计数的资产搜索结果。

1. 您可以轻松地从搜索结果导航到项目，并使用浏览器中的返回按钮返回到相同的搜索结果，而无需重新运行搜索查询。

## 将搜索另存为智能收藏集 {#save-your-searches-as-smart-collection}

您可以将搜索设置保存为智能收藏集，以便快速重复相同的搜索，而无需稍后重做相同的设置。

要将搜索设置另存为智能收藏集，请执行以下操作：

1. 点按／单 **[!UICONTROL 击保存智能收藏]** ，并为智能收藏集提供名称。

   要使所有用户都可以访问智能集合，请选择“公 **[!UICONTROL 共”]**。 系统会显示一条消息，确认已创建智能收藏集并将其添加到保存的搜索的列表。

   >[!NOTE]
   >
   >非管理员用户可能被禁止公开智能收藏集，以避免在组织的品牌门户上拥有大量由非管理员用户创建的公共智能收藏集。 组织可以从管理工具 **[!UICONTROL 面板中提供的“常规]** ”设 **[!UICONTROL 置禁用“允]** 许公共智能集合创建配置”。

   ![](assets/save_smartcollectionui.png)

1. 要以其他名称保存智能收藏集，并选中或清除公共复选 **[!UICONTROL 框]** ，请单击 **[!UICONTROL 编辑智能收藏集]**。

   ![](assets/edit_smartcollection.png)

1. 在编辑 **[!UICONTROL 智能收藏集]** 对话框中，选择 **[!UICONTROL 另存为]** ，然后输入智能收藏集的名称。 单击&#x200B;**[!UICONTROL 保存]**。

   ![](assets/saveas_smartsearch.png)
