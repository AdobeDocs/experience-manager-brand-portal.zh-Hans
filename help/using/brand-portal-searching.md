---
title: 在Brand Portal上搜索资产
seo-title: 在AEM Brand Portal上搜索资产并保存搜索
description: Brand Portal search capability lets you quickly search for relevant assets using omnisearch, and search filters help you further narrow down your search. 将搜索另存为智能收藏集，以供将来使用。
seo-description: Brand Portal搜索功能允许您使用搜索功能快速搜索相关资产，搜索筛选器可帮助您进一步缩小搜索范围。 将搜索另存为智能收藏集，以供将来使用。
uuid: c2955198-bdc0-4853-a13a-661e6a9ec61f
contentOwner: bdhar
content-type: 引用
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: SearchandPromote
discoiquuid: dc751cd7-f663-46d2-84c4-5bb12a4fe1ba
translation-type: tm+mt
source-git-commit: 9763a57a83db22cd6686701dcbd8fcde16bcbb31

---


# 在Brand Portal上搜索资产 {#search-assets-on-brand-portal}

Brand Portal搜索功能允许您使用搜索功能快速搜索相关资产，并使用多面搜索功能帮助您进一步缩小搜索范围。 您还可以将搜索保存为智能收藏集，以供将来使用。

## 使用Omnisearch搜索资产 {#search-assets-using-omnisearch}

要在Brand Portal上搜索资产，请执行以下操作：

1. 在工具栏中，单击 **[!UICONTROL 搜索]** 图标，或按“**[!UICONTROL /]**”键启动Omnisearch。

   ![](assets/omnisearchicon-1.png)

1. 在搜索框中，为要搜索的资产键入关键字。

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >搜索过程中至少需要3个字符，以便显示搜索建议。

1. 从下拉列表中显示的相关建议中进行选择，以快速访问相关资产。

   ![](assets/assets-search-result.png)

   *使用内部搜索进行资产搜索*

要了解带有智能标记资产的搜索行为，请参 [阅了解搜索结果和行为](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-assets.html)。

## 在“筛选器”面板中使用facet进行搜索 {#search-using-facets-in-filters-panel}

“筛选器”面板中的搜索彩块化为您的搜索体验增加了粒度，并使搜索功能更加高效。 搜索彩块化使用多个维度（谓词），这些维度（谓词）使您能够执行细微的搜索。 您可以轻松向下展开到所需的详细信息级别，以便进行更具针对性的搜索。

例如，如果要查找图像，则可以选择是要位图还是要矢量图像。 您可以通过在文件类型搜索facet中为图像指定MIME类型，进一步缩小搜索范围。 同样，在搜索文档时，可以指定格式，例如PDF或MS Word格式。<br />

![Brand](assets/file-type-search.png "Portal中的“过滤器”面板Brand Portal中的“过滤器”面板")

“滤 [!UICONTROL 镜] ”面板包括几个标准彩块化，如- [!UICONTROL Path Facets、]Path Facets、 [!UICONTROL File Type]、 File Size、FileAcromediaStatus和OrientationFacets等。 However, you can add custom search facets or remove specific search facets from the Filters panel by adding or removing predicates in the underlying Search Form. [](../using/brand-portal-search-facets.md)See the list of the available and usable [search predicates on Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates).

To apply filters to your search, using the available [search facets](../using/brand-portal-search-facets.md):

1. Click the overlay icon and select Filter.****

   ![](assets/selectorrail.png)

2. From the Filters panel on the left, select the appropriate options to apply the relevant filters.
**** For example, use the following standard filters:

   * **[!UICONTROL Path Browser]** to search assets in a specific directory. The default search path of the predicate for Path Browser is /content/dam/mac/&lt;tenant-id&gt;/, which can be configured by editing the default search form.****
   >[!NOTE]
   >
   >To non-admin users, Path Browser in Filter panel shows only the content structure of the folders (and their ancestor folders) shared with them.\
   >To admin users, Path Browser allows navigating to any folder in Brand Portal.

   * **[!UICONTROL File Type to specify the type (image, document, multimedia, archive) of asset file you are looking for.]** Further, you can narrow down the scope of your search, for example, specify the MIME type (Tiff, Bitmap, GIMP Images) for image or format (PDF or MS Word) for the documents.
   * **[!UICONTROL File Size]** to search for assets based on their size. You can specify the lower and upper limits for the size range to narrow down your search and specify the unit of measure to search.
   * **[!UICONTROL 状态]** ，用于根据资产状态(如批准（已批准）、已请求更改、已拒绝、待定)和到期等资产状态搜索资产。
   * **[!UICONTROL Average Rating to search for assets based on the rating of the assets.]**
   * **[!UICONTROL 方向]** ：根据资产的方向（水平、垂直、正方形）搜索资产。
   * **[!UICONTROL 样式]** ，以根据资产的样式（彩色、单色）搜索资产。
   * **[!UICONTROL 视频格式]** ，根据视频资源的格式(DVI、Flash、MPEG4、MPEG、OGG Theora、QuickTime、Windows Media、WebM)搜索视频资源。
   您可以通过编 [辑基础的搜索表单](../using/brand-portal-search-facets.md) ，在“筛选器”面板中使用自定义搜索彩块化。

   * **[!UICONTROL 属性谓词]** （如果在搜索表单中使用）允许您搜索与谓词所映射到的元数据属性相匹配的资产。\
      例如，如果属性谓词已映射到，则 [!UICONTROL `jcr:content /metadata/dc:title`]您可以根据资产的标题搜索资产。\
      属性 [!UICONTROL 谓词支持] :

      **部分短语**&#x200B;要允许使用属性谓词中的部分短语进行资产搜索，请在“搜索表单”中启用&#x200B;**[!UICONTROL 部分搜索]复选框。**\
      该功能允许您搜索所需的资产，即使您没有指定资产元数据中使用的确切字词/短语。\
      您可以：*在“过滤器”面板的facet中指定搜索短语中出现的单词。 For example, if you search for the term **climb** (and Property Predicate is mapped to [!UICONTROL `dc:title`] property), then all the assets with the word **climb** in their title phrase are returned.
*指定搜索短语中出现的单词的一部分，以及通配符(*)以填补间隙。
例如，搜索：
      **climb*** 返回所有资源，其标题短语中的单词以字符“clamp”开头。
      ***climp** 返回标题短语中带有“climp”字符的所有资产。
      ***climb*** 返回标题短语中包含“climb”字符的所有资源。\
      **非区分大小写文本**&#x200B;要允许在属性谓词中进行非区分大小写的搜索，请在搜索表单中启 **[!UICONTROL 用“忽略大小写]** ”复选框。 默认情况下，对属性谓词的文本搜索区分大小写。
   >[!NOTE]
   >
   >在选中“部 **[!UICONTROL 分搜索]** ”复选框时， [!UICONTROL 默认情况下会选中“忽略大小写] ”。

   ![](assets/wildcard-prop-1.png)

   根据所应用的过滤器以及搜索结果计数显示搜索结果。

   ![](assets/omnisearch-with-filters.png)

   具有搜索结果计数的资产搜索结果

3. 您可以轻松地从搜索结果中导航到项目，并使用浏览器中的返回按钮返回到相同的搜索结果，而不必重新运行搜索查询。

## 将搜索另存为智能收藏集 {#save-your-searches-as-smart-collection}

您可以将搜索设置另存为智能收藏集，以便能够快速重复相同的搜索，而无需稍后重做相同的设置。

将搜索设置另存为智能收藏集：

1. 点按／单击 **[!UICONTROL 保存智能收藏集]** ，并为智能收藏集提供名称。

   要使智能收藏集可供所有用户访问，请选择“公 **[!UICONTROL 共”]**。 系统会显示一条消息，确认已创建智能收藏集并将其添加到保存的搜索列表中。

   >[!NOTE]
   >
   >非管理员用户可限制其公开智能集合，以避免组织的品牌门户上有大量非管理员用户创建的公共智能集合。 组织可以从管理工具 **[!UICONTROL 面板中提供的常规设置中禁用]****** “允许创建公共智能集合”配置。

   ![](assets/save_smartcollectionui.png)

2. 要以其他名称保存智能收藏集，并选中或清除“公共”复选 **[!UICONTROL 框]** ，请单击“ **[!UICONTROL 编辑智能收藏集”]**。

   ![](assets/edit_smartcollection.png)

3. 在“编 **[!UICONTROL 辑智能收藏集]** ”对话框中，选择 **[!UICONTROL 另存为]** ，然后输入智能收藏集的名称。 Click **[!UICONTROL Save]**.

   ![](assets/saveas_smartsearch.png)
