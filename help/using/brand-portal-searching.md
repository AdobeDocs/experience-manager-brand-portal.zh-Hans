---
title: 在Brand Portal上搜索资源
seo-title: Asset searching and saved search on Experience Manager Assets Brand Portal
description: Brand Portal搜索功能允许您使用omnisearch快速搜索相关资源，而搜索筛选器可帮助您进一步缩小搜索范围。 将搜索另存为智能收藏集，以供将来使用。
seo-description: Brand Portal search capability lets you quickly search for relevant assets using omnisearch, and search filters help you further narrow down your search. Save your searches as smart collections for future.
uuid: c2955198-bdc0-4853-a13a-661e6a9ec61f
contentOwner: bdhar
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: SearchandPromote
discoiquuid: dc751cd7-f663-46d2-84c4-5bb12a4fe1ba
exl-id: 7297bbe5-df8c-4d0b-8204-218a9fdc2292
source-git-commit: cbdd943b904882cc9a455bab24c3cf732d5966ca
workflow-type: tm+mt
source-wordcount: '1341'
ht-degree: 2%

---

# 在Brand Portal上搜索资源 {#search-assets-on-brand-portal}

Brand Portal搜索功能允许您使用omnisearch快速搜索相关资源，并可通过使用过滤器的彩块化搜索帮助您进一步缩小搜索范围。 您可以在文件或文件夹级别搜索资产，并将搜索结果另存为智能收藏集。

>[!NOTE]
>
>Brand Portal不支持使用omnisearch进行收藏集搜索。
>
>但是，您可以使用[搜索筛选器来获取相关收藏集的列表](#search-collection)。

## 使用Omnisearch搜索资源 {#search-assets-using-omnisearch}

要在Brand Portal中搜索资源，请执行以下操作：

1. 在工具栏中，单击&#x200B;**[!UICONTROL 搜索]**&#x200B;图标，或按“**[!UICONTROL /]**”键启动Omnisearch。

   ![](assets/omnisearchicon-1.png)

1. 在搜索框中，键入要搜索的资源的关键字。

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >* omnisearch中至少需要3个字符才能显示搜索建议。
   >* 在搜索`mountain biking`时，omnisearch返回搜索结果中元数据字段中同时具有`mountain`和`biking`可用的所有资源。 例如，`Title`字段中的`mountain`和`Description`字段中的`biking`。 这两个术语必须在元数据字段中可用，才能显示在搜索结果中。 但是，omnisearch会在搜索结果中返回资产，即使智能标记元数据字段中只有两个术语之一可用。 例如，如果某个资产包含`mountain`作为智能标记之一，而在任何其他元数据字段中不包含`biking`且您搜索了`mountain biking`，则omnisearch仍会在搜索结果中返回该资产。

1. 从下拉列表中显示的相关建议中进行选择，以快速访问相关资源。

   ![](assets/assets-search-result.png)

   *使用omnisearch搜索资源*

要了解智能标记资源的搜索行为，请参阅[了解搜索结果和行为](https://experienceleague.adobe.com/docs/experience-manager-65/assets/using/search-assets.html)。

## 在“筛选器”面板中使用Facet进行搜索 {#search-using-facets-in-filters-panel}

“筛选器”面板中的搜索Facet可为您的搜索体验添加粒度，并使搜索功能变得高效。 搜索Facet使用多个维度（谓词），使您能够执行复杂的搜索。 您可以轻松地深入到所需的详细级别以进行更集中的搜索。

例如，如果要查找图像，您可以选择是要位图还是矢量图像。 可通过在“文件类型”搜索彩块中指定图像的MIME类型来进一步缩小搜索范围。 同样，在搜索文档时，可以指定格式，例如PDF或MS® Word格式。

Brand Portal中的![筛选器面板](assets/file-type-search.png "Brand Portal中的“筛选器”面板")

**[!UICONTROL 筛选器]**&#x200B;面板包含几个标准Facet，如 — **[!UICONTROL 路径浏览器]**、**[!UICONTROL 文件类型]**、**[!UICONTROL 文件大小]**、**[!UICONTROL 状态]**&#x200B;和&#x200B;**[!UICONTROL 方向]**。 但是，您可以通过添加或删除基础搜索表单中的谓词，向面板[添加自定义搜索彩块化](../using/brand-portal-search-facets.md)或从&#x200B;**[!UICONTROL 筛选器]**&#x200B;中删除特定搜索彩块化。 查看Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates)上可用的[搜索谓词列表。

要使用可用的[搜索Facet](../using/brand-portal-search-facets.md)将筛选器应用于搜索，请执行以下操作：

1. 单击叠加图标并选择&#x200B;**[!UICONTROL 筛选器]**。

   ![](assets/selectorrail.png)

1. 从左侧的&#x200B;**[!UICONTROL 筛选器]**面板中选择适当的选项以应用相关筛选器。
例如，使用以下标准过滤器：

   * **[!UICONTROL 路径浏览器]**&#x200B;以搜索特定目录中的资产。 路径浏览器的谓词的默认搜索路径为`/content/dam/mac/<tenant-id>/`，可以通过编辑默认搜索表单来配置该路径。

   >[!NOTE]
   >
   >对于非管理员用户，[!UICONTROL 筛选器]面板中的[!UICONTROL 路径浏览器]仅显示与他们共享的文件夹（及其上级文件夹）的内容结构。\
   >对于管理员用户，路径浏览器允许导航到Brand Portal中的任何文件夹。

   * **[!UICONTROL 文件类型]**，用于指定您要查找的资源文件的类型（图像、文档、多媒体、存档）。 此外，您可以缩小搜索范围，例如，为图像或文档格式(PDF或MS® Word)指定MIME类型（Tiff、位图、GIMP图像）。
   * **[!UICONTROL 文件大小]**&#x200B;以根据资源的大小搜索资源。 您可以指定大小范围的下限和上限以缩小搜索范围，并指定要搜索的度量单位。
   * **[!UICONTROL 状态]**&#x200B;以根据资产状态搜索资产，例如批准（已批准、已请求更改、已拒绝、待处理）和到期。
   * **[!UICONTROL 平均评分]**&#x200B;以根据资产的评分搜索资产。
   * **[!UICONTROL 方向]**，根据资源的方向（水平、垂直、正方形）搜索资源。
   * **[!UICONTROL 样式]**&#x200B;以根据资源的样式（彩色、单色）搜索资源。
   * **[!UICONTROL 视频格式]**，用于根据其格式(DVI、Flash、MPEG4、MPEG、OGG Theora、QuickTime、Windows Media、WebM)搜索视频资源。

   您可以通过编辑基础搜索表单在“筛选器”面板中使用[自定义搜索彩块化](../using/brand-portal-search-facets.md)。

   * **[!UICONTROL 属性谓词]**&#x200B;如果用在搜索表单中，则允许您搜索与谓词所映射到的元数据属性匹配的资源。\
     例如，如果属性谓词映射到[!UICONTROL `jcr:content /metadata/dc:title`]，则可以根据资产的标题搜索资产。\
     [!UICONTROL 属性谓词]支持以下内容的文本搜索：

     **部分短语**
要允许使用属性谓词中的部分短语进行资产搜索，请在“搜索表单”中启用**[!UICONTROL 部分搜索]**&#x200B;复选框。 该功能允许您搜索所需的资产，即使您没有指定资产元数据中使用的确切字词/短语。

     >[!NOTE]
     >
     > Brand Portal支持“部分搜索”的以下字段：
     >* jcr：content/metadata/dc：title
     >* jcr：content/jcr：title
     >* jcr：content/metadata/dam：search_promote
     >* jcr:content/metadata/dc:format

     您可以：
      * 在“过滤器”面板的Facet中，指定出现在搜索短语中的单词。 例如，如果您搜索术语&#x200B;**climb**（并且属性谓词映射到[!UICONTROL `dc:title`]属性），则返回其标题短语中包含单词&#x200B;**climb**&#x200B;的所有资产。
      * 指定出现在搜索短语中的单词的一部分，并使用通配符(&#42;)填补空白。
例如，搜索：
         * **climb&#42;**&#x200B;返回其标题短语中含有以“climb”开头的单词的所有资产。
         * **&#42;climb**&#x200B;返回标题短语中单词以“climb”结尾的所有资产。
         * **&#42;climb&#42;**&#x200B;返回其标题短语中包含字符“climb”的所有资产。

     **不区分大小写的文本**
若要允许在属性谓词中进行不区分大小写的搜索，请启用“搜索表单”中的**[!UICONTROL 忽略大小写]**&#x200B;复选框。 默认情况下，对属性谓词的文本搜索区分大小写。

   >[!NOTE]
   >
   >选中&#x200B;**[!UICONTROL 部分搜索]**&#x200B;复选框时，默认情况下会选中&#x200B;**[!UICONTROL 忽略大小写]**。

   ![](assets/wildcard-prop-1.png)

   根据应用的过滤器以及搜索结果计数显示搜索结果。

   ![](assets/omnisearch-with-filters.png)

   包含搜索结果计数的资源搜索结果。

1. 您可以从搜索结果轻松导航到某个项目，然后使用浏览器中的“返回”按钮返回到相同的搜索结果，而无需重新运行搜索查询。

## 将搜索另存为智能收藏集 {#save-your-searches-as-smart-collection}

您可以将搜索设置另存为智能收藏集，以便能够快速重复相同的搜索，而无需稍后重做相同的设置。 但是，您不能在收藏集中应用搜索过滤器。

要将搜索设置另存为智能收藏集，请执行以下操作：

1. 点按/单击&#x200B;**[!UICONTROL 保存智能收藏集]**，并提供智能收藏集的名称。

   要使所有用户均可访问智能收藏集，请选择&#x200B;**[!UICONTROL 公共]**。 将显示一条消息，确认智能收藏集已创建并已添加到保存的搜索列表。

   >[!NOTE]
   >
   >可以限制非管理员用户公开智能收藏集，以避免组织的Brand Portal上出现大量非管理员用户创建的公共智能收藏集。 组织可以禁用管理工具面板中可用的&#x200B;**[!UICONTROL 常规]**&#x200B;设置中的&#x200B;**[!UICONTROL 允许公共智能收藏集创建]**&#x200B;配置。

   ![](assets/save_smartcollectionui.png)

1. 若要以其他名称保存智能收藏集，并选择或清除&#x200B;**[!UICONTROL 公共]**&#x200B;复选框，请单击&#x200B;**[!UICONTROL 编辑智能收藏集]**。

   ![](assets/edit_smartcollection.png)

1. 在&#x200B;**[!UICONTROL 编辑智能收藏集]**&#x200B;对话框中，选择&#x200B;**[!UICONTROL 另存为]**，然后输入智能收藏集的名称。 单击&#x200B;**[!UICONTROL 保存]**。

   ![](assets/saveas_smartsearch.png)


## 搜索收藏集 {#search-collection}

收藏集不支持Omnisearch。 但是，您可以应用搜索筛选器以在[!UICONTROL 收藏集]界面中列出相关收藏集。

在[!UICONTROL 收藏集]界面中，单击叠加图标以在左边栏中打开过滤器面板。 从可用筛选器（`modified date`、`access type`和`tags`）中应用一个或多个搜索筛选器。 它会根据应用的过滤器列出最相关的收藏集集。

![](assets/collection-search.png)
