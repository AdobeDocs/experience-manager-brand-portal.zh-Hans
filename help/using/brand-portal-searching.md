---
title: 在Brand Portal上搜索资产
seo-title: AEM Brand Portal上的资产搜索和保存搜索
description: Brand Portal搜索功能可让您使用Omnisearch快速搜索相关资产，搜索过滤器可帮助您进一步缩小搜索范围。将搜索另存为将来的智能收藏集。
seo-description: Brand Portal搜索功能可让您使用Omnisearch快速搜索相关资产，搜索过滤器可帮助您进一步缩小搜索范围。将搜索另存为将来的智能收藏集。
uuid: c2955198-bdc0-4853-a13 a-661e6 a9 ec61 f
contentOwner: bdar
content-type: 引用
products: SG_ EXPERIENCE MANAGER/Brand_ Portal
topic-tags: PresenAndPromote
discoiquuid: dc751cd7-f663-46d2-84c4-5b12 a4 fe1 ba
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# 在Brand Portal上搜索资产 {#search-assets-on-brand-portal}

[!DNL Brand Portal] 搜索功能允许您使用Omnisearch和facet搜索快速搜索相关资产，该搜索使用过滤器帮助您进一步缩小搜索范围。您还可以将搜索另存为将来的智能 [!UICONTROL 收藏集] 。

## 使用Omnisarch搜索资产 {#search-assets-using-omnisearch}

要搜索资产， [!DNL Brand Portal]请执行以下操作：

1. 在工具栏中，单击 **搜索** 图标，或按“**/**”键启动OmnisSearch。

   ![](assets/omnisearchicon-1.png)

2. 在搜索框中，键入要搜索的资产的关键字。

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >在omnisearch中至少需要个字符才能显示搜索建议。

3. 从下拉列表中显示的相关建议中进行选择，以快速访问相关资产。

   ![](assets/assets-search-result.png)

   使用Omnisearch进行资产搜索

## 在筛选器面板中使用facet进行搜索 {#search-using-facets-in-filters-panel}

在“过滤器”面板中搜索彩块化，为搜索体验添加粒度，并提高搜索功能。搜索彩块化使用多个维度(谓词)来执行复杂的搜索。您可以轻松向下钻取到所需的详细信息级别，以实现更集中的搜索。

例如，如果您要查找图像，则可以选择是要位图还是矢量图像。您可以通过在“文件类型”搜索facet中指定图像的MIME类型进一步减少搜索范围。同样，在搜索文档时，您可以指定格式，例如PDF或MS Word格式。

![[ [!DNL Brand Portal]](assets/file-type-search.png "！DNL Brand Portal]")

“滤镜”面板包括一些标准彩块化，如路径浏览器、文件类型、文件大小、状态和方向。但是，您可以通过在底层搜索表单中添加或删除谓词 [](../using/brand-portal-search-facets.md) ，从 **“筛选器** ”面板添加自定义搜索彩块化或删除特定搜索彩块化。请参阅Brand Portal上可用 [的可用搜索谓词列表](../using/brand-portal-search-facets.md#list-of-search-predicates)。

要使用可用 [的搜索彩块化将过滤器应用于搜索](../using/brand-portal-search-facets.md)，请执行以下操作：

1. 单击叠加图标，然后选择 **筛选器**。

   ![](assets/selectorrail.png)

2. 从左侧的 **“滤镜** ”面板中，选择相应的选项以应用相关滤镜。
例如，使用以下标准过滤器：

   * **路径浏览器** 可在特定目录中搜索资产。路径浏览器谓词的默认搜索路径为 *&lt; tenant-id&gt;/*，可通过编辑默认搜索表单来进行配置。
   >[!NOTE]
   >
   >对于非管理员用户，“过滤器”面板中的路径浏览器仅显示与其共享的文件夹(及其父文件夹)的内容结构。\
   >对于管理员用户，路径浏览器允许导航到任何文件夹 [!DNL Brand Portal]。

   * **“文件类型** ”用于指定您要查找的资产文件的类型(图像、文档、多媒体、存档)。此外，您还可以缩小搜索范围，例如，为文档指定MIME类型(TIFF、位图、GIMP图像)或格式(PDF或MS Word)。
   * **文件大小** 根据资产大小搜索资产。您可以指定大小范围的下限和上限以缩小搜索范围，并指定要搜索的度量单位。
   * **状态** 可根据资产状态搜索资产，如批准(已批准、已请求、已拒绝、待定)和过期。
   * **平均评级** 可根据资产的评级搜索资产。
   * **根据** 资产的方向(水平、垂直、平方)搜索资产的方向。
   * **样式** 根据资产的样式(彩色、单色)搜索资产。
   * **视频格式** 可根据视频资产格式(DVI、Flash、MPEG4、MPEG、OGG Theora、QuickTime、Windows Media、WebM)搜索视频资产。
   您可以通过编辑底层搜索表单，在“过滤器”面板中使用 [自定义搜索彩块化](../using/brand-portal-search-facets.md) 。

   * **属性谓词** (如果在搜索表单中使用)，可允许您搜索与该谓词的映射元数据属性匹配的资产。\
      例如，如果将属性谓词映射到 `jcr:content /metadata/dc:title`，则可以根据资产的标题搜索资产。\
      属性谓词支持文本搜索：

      **部分短语**&#x200B;要允许使用属性谓词中的部分短语进行资产搜索，请在“搜索表单”中启用&#x200B;**部分搜索**&#x200B;复选框。\
      该功能允许您搜索所需的资产，即使您没有指定资产元数据中使用的确切字词/短语。\
      您可以：
*在筛选器面板中的facet中指定在facet中出现的词。For example, if you search for the term **climb** (and Property Predicate is mapped to `dc:title` property), then all the assets with the word **climb** in their title phrase are returned.
*指定在搜索的短语中出现的单词部分，以及通配符字符(*)以填补间隙。
例如，搜索：
      **aup*** 返回所有资产(以字符“rating”开头，以标题短语开头)。
      ***爬出** 会返回标题短语中以字符“升序”结尾的所有资产。
      *** launch*** 返回所有包含字符“爬出”字样的资产的所有资产。\
      **非区分大小写的文本**&#x200B;要在属性谓词中允许区分大小写的搜索，请在搜索表单中启用 **“忽略大小写”** 复选框。默认情况下，属性谓词上的文本搜索区分大小写。
   >[!NOTE]
   >
   >选择 **“部分搜索** ”复选框时， **默认情况下会选中“忽略大小写** ”。

   ![](assets/wildcard-prop-1.png)

   搜索结果会根据应用的筛选器以及搜索结果计数来显示。

   ![](assets/omnisearch-with-filters.png)

   具有搜索结果计数的资产搜索结果

3. 您可以从搜索结果轻松导航到某个项目，并使用浏览器中的返回按钮返回相同的搜索结果，而不必重新运行搜索查询。

## 将搜索另存为智能收藏集 {#save-your-searches-as-smart-collection}

您可以将搜索设置保存为智能收藏集，以便快速重复同一搜索，而不必稍后重做相同设置。

要将搜索设置保存为智能收藏集，请执行以下操作：

1. 点按/单击 **保存智能收藏集** ，并为智能收藏集提供一个名称。

   要使所有用户都可以访问智能收藏集，请选择 **“公共**”。系统会显示一条消息，确认已创建智能收藏集并将其添加到保存的搜索列表中。

   >[!NOTE]
   >
   >不能限制非管理员用户将智能 [!UICONTROL 收藏集] 公开，以避免拥有组织的非管理员用户创建的大量公共智能 [!UICONTROL 收藏集][!DNL Brand Portal]。组织可以从管理工具面板中提供的“常规”设置禁用 **“允许公共智能[!UICONTROL 收藏集]创建****** 配置”。

   ![](assets/save_smartcollectionui.png)

1. 要以其他名称保存智能收藏集，并选择或清除 **“公共”** 复选框，请单击 **“编辑智能收藏集**”。

   ![](assets/edit_smartcollection.png)

1. 在 **“编辑智能收藏集** ”对话框中，选择 **“另存为”** 并输入智能收藏集的名称。单击&#x200B;**保存**。

   ![](assets/saveas_smartsearch.png)
