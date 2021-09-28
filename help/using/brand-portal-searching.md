---
title: 在 Brand Portal 上搜索资产
seo-title: Asset searching and saved search on AEM Brand Portal
description: Brand Portal搜索功能允许您使用omnisearch快速搜索相关资产，而搜索过滤器可以帮助您进一步缩小搜索范围。 将搜索另存为智能收藏集，以供将来使用。
seo-description: Brand Portal search capability lets you quickly search for relevant assets using omnisearch, and search filters help you further narrow down your search. Save your searches as smart collections for future.
uuid: c2955198-bdc0-4853-a13a-661e6a9ec61f
contentOwner: bdhar
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: SearchandPromote
discoiquuid: dc751cd7-f663-46d2-84c4-5bb12a4fe1ba
exl-id: 7297bbe5-df8c-4d0b-8204-218a9fdc2292
source-git-commit: d7dbf9ae2d27dda2edb60d8f861e618fb6332ec7
workflow-type: tm+mt
source-wordcount: '1123'
ht-degree: 5%

---

# 在 Brand Portal 上搜索资产 {#search-assets-on-brand-portal}

Brand Portal搜索功能允许您使用omnisearch和facet搜索来快速搜索相关资产，这些搜索使用过滤器来帮助您进一步缩小搜索范围。 您还可以将搜索另存为智能收藏集，以供将来使用。

## 使用Omnisearch搜索资产 {#search-assets-using-omnisearch}

要在Brand Portal上搜索资产，请执行以下操作：

1. 在工具栏中，单击&#x200B;**[!UICONTROL Search]**&#x200B;图标，或按“**[!UICONTROL /]**”键以启动Omnisearch。

   ![](assets/omnisearchicon-1.png)

1. 在搜索框中，为要搜索的资产键入关键字。

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >Omnisearch中至少需要3个字符才能显示搜索建议。

1. 从下拉列表中显示的相关建议中进行选择，以快速访问相关资产。

   ![](assets/assets-search-result.png)

   *使用Omnisearch搜索资产*

要了解智能标记资产的搜索行为，请参阅[了解搜索结果和行为](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-assets.html)。

## 在“过滤器”面板中使用Facet进行搜索 {#search-using-facets-in-filters-panel}

“过滤器”面板中的搜索彩块化可为您的搜索体验添加粒度，并提高搜索功能的效率。 搜索彩块化使用多个维度（谓词），允许您执行复杂搜索。 您可以轻松地向下展开到所需的详细信息级别，以便进行更集中的搜索。

例如，如果要查找图像，则可以选择想要位图还是矢量图像。 您可以通过在“文件类型”搜索方面中为图像指定MIME类型，进一步缩小搜索范围。 同样，在搜索文档时，可以指定格式，例如PDF或MS Word格式。

![Brand Portal中的“过滤器”面](assets/file-type-search.png "板Brand Portal中的“过滤器”面板")

**[!UICONTROL 过滤器]**&#x200B;面板包括一些标准方面，例如 — **[!UICONTROL 路径浏览器]**、**[!UICONTROL 文件类型]**、**[!UICONTROL 文件大小]**、**[!UICONTROL 状态]**&#x200B;和&#x200B;**[!UICONTROL 方向]**。 但是，您可以通过在基础搜索表单中添加或删除谓词，来[添加自定义搜索彩块化](../using/brand-portal-search-facets.md)或从&#x200B;**[!UICONTROL 过滤器]**&#x200B;面板中删除特定搜索彩块化。 请参阅Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates)上可用的[搜索谓词列表。

要对搜索应用过滤器，请使用可用的[搜索彩块化](../using/brand-portal-search-facets.md):

1. 单击叠加图标并选择&#x200B;**[!UICONTROL Filter]**。

   ![](assets/selectorrail.png)

1. 从左侧的&#x200B;**[!UICONTROL 过滤器]**面板中，选择相应的选项以应用相关过滤器。
例如，使用以下标准过滤器：

   * **[!UICONTROL 路径浏]** 览器在特定目录中搜索资产。路径浏览器谓词的默认搜索路径为`/content/dam/mac/<tenant-id>/`，可通过编辑默认搜索表单来配置该路径。
   >[!NOTE]
   >
   >对于非管理员用户， [!UICONTROL 过滤器]面板中的[!UICONTROL 路径浏览器]仅显示与其共享的文件夹（及其上级文件夹）的内容结构。\
   >对于管理员用户，路径浏览器允许导航到Brand Portal中的任意文件夹。

   * **[!UICONTROL 文]** 件类型，以指定要查找的资产文件的类型（图像、文档、多媒体、存档）。此外，您还可以缩小搜索范围，例如，为文档的图像或格式（PDF或MS Word）指定MIME类型（Tiff、位图、GIMP图像）。
   * **[!UICONTROL 文]** 件大小，以根据资产大小搜索资产。您可以为大小范围指定下限和上限，以缩小搜索范围并指定要搜索的度量单位。
   * **** 状态，用于根据资产状态(如批准（已批准）、请求更改、已拒绝、待定)和到期情况搜索资产。
   * **[!UICONTROL 平均]** 评分，以根据资产评级搜索资产。
   * **** 方向，以根据资产的方向（水平、垂直、正方形）搜索资产。
   * **** 样式：根据资产的样式（彩色、单色）搜索资产。
   * **[!UICONTROL 视]** 频格式，根据视频资产的格式(DVI、Flash、MPEG4、MPEG、OGG Theora、QuickTime、Windows Media、WebM)搜索视频资产。

   您可以通过编辑基础搜索表单，在“过滤器”面板中使用[自定义搜索彩块化](../using/brand-portal-search-facets.md)。

   * **[!UICONTROL 属性]** 谓词（如果在搜索表单中使用）允许您搜索与谓词所映射的元数据属性相匹配的资产。\
      例如，如果属性谓词映射到[!UICONTROL `jcr:content /metadata/dc:title`]，则可以根据资产的标题搜索资产。\
      [!UICONTROL 属性谓词]支持对以下项进行文本搜索：

      **部分短语**&#x200B;要允许使用属性谓词中的部分短语进行资产搜索，请在“搜索表单”中启用&#x200B;**[!UICONTROL 部分搜索]**&#x200B;复选框。\
      该功能允许您搜索所需的资产，即使您没有指定资产元数据中使用的确切字词/短语。\
      您可以：
      * 在“过滤器”面板的Facet中，指定出现在搜索短语中的单词。 例如，如果您搜索术语&#x200B;**climb**（“属性谓词”会映射到[!UICONTROL `dc:title`]属性），则会返回其标题短语中带有单词&#x200B;**climb**&#x200B;的所有资产。
      * 指定出现在搜索短语中的单词的一部分，以及通配符(*)以填补空白。
例如，搜索：
         * **climb*** 会返回所有包含以其标题短语中的字符“climb”开头的单词的资产。
         * ***** mabping会返回标题短语中包含以“climb”字符结尾的所有资产。
         * ***climb*** 会返回所有包含词语的资产，其标题短语中包含字符“climb”。

要允许在属性谓词中进行不区分大小写的搜索，请启用       **非区分大小写文**
本要允许在属性谓词中进行不区分大小写的搜索，请在“搜索 **[!UICONTROL 表单”]** 中启用“忽略大小写”复选框。默认情况下，对属性谓词的文本搜索区分大小写。
   >[!NOTE]
   >
   >选中&#x200B;**[!UICONTROL 部分搜索]**&#x200B;复选框时，默认情况下会选中&#x200B;**[!UICONTROL 忽略大小写]**。

   ![](assets/wildcard-prop-1.png)

   搜索结果将根据应用的过滤器以及搜索结果计数一起显示。

   ![](assets/omnisearch-with-filters.png)

   包含搜索结果计数的资产搜索结果。

1. 您可以轻松地从搜索结果导航到项目，并使用浏览器中的返回按钮返回到相同的搜索结果，而无需重新运行搜索查询。

## 将搜索另存为智能收藏集 {#save-your-searches-as-smart-collection}

您可以将搜索设置另存为智能收藏集，以便能够快速重复相同的搜索，而无需稍后重做相同的设置。

要将搜索设置另存为智能收藏集，请执行以下操作：

1. 点按/单击&#x200B;**[!UICONTROL 保存智能收藏集]**，并提供智能收藏集的名称。

   要使所有用户都可以访问智能收藏集，请选择&#x200B;**[!UICONTROL Public]**。 系统会显示一条消息，确认已创建智能收藏集并将其添加到保存的搜索列表。

   >[!NOTE]
   >
   >可以限制非管理员用户公开智能收藏集，以避免在组织的Brand Portal上拥有大量由非管理员用户创建的公共智能收藏集。 组织可以禁用“管理工具”面板中提供的“允许从&#x200B;**[!UICONTROL 常规]**&#x200B;创建公共智能收藏集&#x200B;]**”设置。**[!UICONTROL 

   ![](assets/save_smartcollectionui.png)

1. 要以其他名称保存智能收藏集，并选中或清除&#x200B;**[!UICONTROL 公共]**&#x200B;复选框，请单击&#x200B;**[!UICONTROL 编辑智能收藏集]**。

   ![](assets/edit_smartcollection.png)

1. 在&#x200B;**[!UICONTROL 编辑智能收藏集]**&#x200B;对话框中，选择&#x200B;**[!UICONTROL 另存为]**&#x200B;并输入智能收藏集的名称。 单击&#x200B;**[!UICONTROL 保存]**。

   ![](assets/saveas_smartsearch.png)
