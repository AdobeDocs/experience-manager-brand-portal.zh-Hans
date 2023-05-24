---
title: 在 Brand Portal 上搜索资产
seo-title: Asset searching and saved search on Experience Manager Assets Brand Portal
description: 通过Brand Portal搜索功能，您可以使用omnisearch快速搜索相关资源，而搜索筛选器可帮助您进一步缩小搜索范围。 将搜索另存为智能收藏集以供将来使用。
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
source-wordcount: '1358'
ht-degree: 5%

---

# 在 Brand Portal 上搜索资产 {#search-assets-on-brand-portal}

Brand Portal搜索功能允许您使用omnisearch快速搜索相关资源，以及使用筛选器的彩块化搜索帮助您进一步缩小搜索范围。 您可以在文件或文件夹级别搜索资产，并将搜索结果另存为智能收藏集。

>[!NOTE]
>
>Brand Portal不支持使用omnisearch进行收藏集搜索。
>
>但是，您可以使用 [搜索筛选器以获取相关收藏集的列表](#search-collection).

## 使用Omnisearch搜索资源 {#search-assets-using-omnisearch}

要在Brand Portal中搜索资源，请执行以下操作：

1. 在工具栏中，单击 **[!UICONTROL 搜索]** 图标，或按“**[!UICONTROL /]**”启动Omnisearch的关键。

   ![](assets/omnisearchicon-1.png)

1. 在搜索框中，键入要搜索的资产的关键字。

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >* omnisearch中至少需要3个字符才能显示搜索建议。
   >* 当您搜索 `mountain biking`， omnisearch返回搜索结果中所有同时包含两者的资产 `mountain` 和 `biking` 在元数据字段中可用。 例如， `mountain` 在 `Title` 字段和 `biking` 在 `Description` 字段。 这两个术语必须在元数据字段中均可用，才能显示在搜索结果中。 但是，即使“智能标记”元数据字段中只有两个术语之一，Omnisearch也会在搜索结果中返回资产。 例如，如果资产包含 `mountain` 作为其中一个智能标记，不包含 `biking` 在任何其他元数据字段中，并且您搜索 `mountain biking`，omnisearch仍会在搜索结果中返回资产。


1. 从下拉列表中显示的相关建议中进行选择，以快速访问相关资源。

   ![](assets/assets-search-result.png)

   *使用Omnisearch搜索资源*

要了解带有智能标记的资源搜索行为，请参阅 [了解搜索结果和行为](https://experienceleague.adobe.com/docs/experience-manager-65/assets/using/search-assets.html).

## 在“筛选器”面板中使用Facet进行搜索 {#search-using-facets-in-filters-panel}

“筛选器”面板中的搜索Facet可为您的搜索体验添加粒度，并使搜索功能高效运行。 搜索Facet使用多个维度（谓词），使您能够执行复杂的搜索。 您可以轻松地深入到所需的详细级别以进行更集中的搜索。

例如，如果您要查找图像，则可以选择是要位图还是矢量图像。 可以通过在“文件类型”搜索彩块中指定图像的MIME类型来进一步缩小搜索范围。 同样，在搜索文档时，可以指定格式，例如PDF或MS® Word格式。

![Brand Portal中的“筛选器”面板](assets/file-type-search.png "Brand Portal中的“筛选器”面板")

此 **[!UICONTROL 筛选器]** 面板包括几个标准方面，例如 **[!UICONTROL 路径浏览器]**， **[!UICONTROL 文件类型]**， **[!UICONTROL 文件大小]**， **[!UICONTROL 状态]**、和 **[!UICONTROL 方向]**. 但是，您可以 [添加自定义搜索Facet](../using/brand-portal-search-facets.md) 或从中移除特定的搜索彩块化 **[!UICONTROL 筛选器]** 面板，方法是在基础搜索表单中添加或删除谓词。 查看可用和可用内容的列表 [Brand Portal上的搜索谓词](../using/brand-portal-search-facets.md#list-of-search-predicates).

要将过滤器应用于您的搜索，请使用可用的 [搜索Facet](../using/brand-portal-search-facets.md)：

1. 单击叠加图标并选择 **[!UICONTROL 筛选条件]**.

   ![](assets/selectorrail.png)

1. 从 **[!UICONTROL 筛选器]** 选择适当的选项以应用相关的筛选器。
例如，使用以下标准过滤器：

   * **[!UICONTROL 路径浏览器]** 以搜索特定目录中的资产。 路径浏览器的谓词的默认搜索路径为 `/content/dam/mac/<tenant-id>/`，可通过编辑默认搜索表单来配置该选项。
   >[!NOTE]
   >
   >对于非管理员用户， [!UICONTROL 路径浏览器] 在 [!UICONTROL 筛选条件] 面板仅显示与其共享的文件夹（及其上级文件夹）的内容结构。\
   >对于管理员用户，路径浏览器允许导航到Brand Portal中的任何文件夹。

   * **[!UICONTROL 文件类型]** 以指定要查找的资源文件的类型（图像、文档、多媒体、存档）。 此外，您可以缩小搜索范围，例如，为图像或文档格式(PDF或MS® Word)指定MIME类型（Tiff、位图、GIMP图像）。
   * **[!UICONTROL 文件大小]** 以根据资源的大小搜索资源。 您可以指定大小范围的下限和上限以缩小搜索范围，并指定要搜索的度量单位。
   * **[!UICONTROL 状态]** 根据资产状态（如批准、已请求更改、已拒绝、待处理）和到期)搜索资产。
   * **[!UICONTROL 平均评分]** 以根据资产的评级搜索资产。
   * **[!UICONTROL 方向]** 根据资源的方向（水平、垂直、平方）搜索资源。
   * **[!UICONTROL 样式]** 根据资产的样式（彩色、单色）搜索资产。
   * **[!UICONTROL 视频格式]** 根据视频资源的格式(DVI、Flash、MPEG4、MPEG、OGG Theora、QuickTime、Windows Media、WebM)搜索视频资源。

   您可以使用 [自定义搜索Facet](../using/brand-portal-search-facets.md) 通过编辑基础搜索表单，在“筛选器”面板中查找。

   * **[!UICONTROL 属性谓词]** 如果在搜索表单中使用，则允许您搜索与谓词所映射到的元数据属性匹配的资源。\
      例如，如果属性谓词映射到 [!UICONTROL `jcr:content /metadata/dc:title`]，您可以根据资产的标题搜索资产。\
      此 [!UICONTROL 属性谓词] 支持以下内容的文本搜索：

      **部分短语**&#x200B;要允许使用属性谓词中的部分短语进行资产搜索，请在“搜索表单”中启用&#x200B;**[!UICONTROL 部分搜索]**&#x200B;复选框。该功能允许您搜索所需的资产，即使您没有指定资产元数据中使用的确切字词/短语。

      >[!NOTE]
      >
      > Brand Portal支持以下部分搜索字段：
      >* jcr：content/metadata/dc：title
      >* jcr：content/jcr：title
      >* jcr：content/metadata/dam：search_promote
      >* jcr:content/metadata/dc:format


      您可以：
      * 在“过滤器”面板的Facet中，指定出现在搜索短语中的单词。 例如，如果您搜索术语 **爬升** (属性谓词映射到 [!UICONTROL `dc:title`] 属性)，则包含单词的所有资源 **爬升** 返回其标题短语。
      * 指定出现在搜索短语中的单词的一部分，以及通配符(&#42;)以填补空白。
例如，搜索：
         * **爬升&#42;** 返回其标题短语中包含以“climb”字符开头的单词的所有资产。
         * **&#42;爬升** 返回其标题短语中包含以“climb”字符结尾的单词的所有资产。
         * **&#42;爬升&#42;** 返回其标题短语中包含字符“climb”的所有资产。

要允许在属性谓词中进行不区分大小写的搜索，请启用       **不区分大小写的文本**
要允许在属性谓词中进行不区分大小写的搜索，请启用 **[!UICONTROL 忽略大小写]** 复选框。 默认情况下，对属性谓词的文本搜索区分大小写。
   >[!NOTE]
   >
   >选择时 **[!UICONTROL 部分搜索]** 复选框， **[!UICONTROL 忽略大小写]** 默认情况下处于选中状态。

   ![](assets/wildcard-prop-1.png)

   根据应用的过滤器以及搜索结果计数显示搜索结果。

   ![](assets/omnisearch-with-filters.png)

   包含搜索结果计数的资源搜索结果。

1. 您可以轻松地从搜索结果中导航到某个项目，然后使用浏览器中的“返回”按钮返回到相同的搜索结果，而无需重新运行搜索查询。

## 将搜索另存为智能收藏集 {#save-your-searches-as-smart-collection}

您可以将搜索设置另存为智能收藏集，以便能够快速重复相同的搜索，而无需稍后重做相同的设置。 但是，无法在收藏集中应用搜索过滤器。

要将搜索设置另存为智能收藏集，请执行以下操作：

1. 点按/单击 **[!UICONTROL 保存智能收藏集]** 并提供智能收藏集的名称。

   要使所有用户都可访问智能收藏集，请选择 **[!UICONTROL 公共]**. 将显示一条消息，确认智能收藏集已创建并已添加到保存的搜索列表。

   >[!NOTE]
   >
   >可以限制非管理员用户公开智能收藏集，以避免非管理员用户在组织的Brand Portal上创建大量公开智能收藏集。 组织可以禁用 **[!UICONTROL 允许创建公共智能收藏集]** 配置自 **[!UICONTROL 常规]** “管理工具”面板中提供的设置。

   ![](assets/save_smartcollectionui.png)

1. 要以其他名称保存智能收藏集，请选择或清除 **[!UICONTROL 公共]** 复选框，单击 **[!UICONTROL 编辑智能收藏集]**.

   ![](assets/edit_smartcollection.png)

1. 在 **[!UICONTROL 编辑智能收藏集]** 对话框中，选择 **[!UICONTROL 另存为]** 并输入智能收藏集的名称。 单击“**[!UICONTROL 保存]**”。

   ![](assets/saveas_smartsearch.png)


## 搜索收藏集 {#search-collection}

收藏集不支持Omnisearch。 但是，您可以应用搜索筛选器以从中列出相关收藏集 [!UICONTROL 收藏集] 界面。

从 [!UICONTROL 收藏集] 界面中，单击叠加图标以打开左边栏中的过滤器面板。 从可用过滤器中应用一个或多个搜索过滤器(`modified date`， `access type`、和 `tags`)。 它会根据应用的过滤器列出最相关的收藏集集。

![](assets/collection-search.png)
