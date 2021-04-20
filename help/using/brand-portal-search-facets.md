---
title: 使用自定义搜索 Facet
seo-title: 使用自定义搜索 Facet
description: 管理员可以向“过滤器”面板添加搜索谓词，以自定义搜索并使搜索功能具有多种用途。
seo-description: 管理员可以向“过滤器”面板添加搜索谓词，以自定义搜索并使搜索功能具有多种用途。
uuid: 986fba5a-fac5-4128-ac75-d04da5b52d45
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 19faa028-246b-42c7-869f-97c95c7a1349
role: Administrator
translation-type: tm+mt
source-git-commit: 263653916e4bc183827c197c3beb137c9e59ccb1
workflow-type: tm+mt
source-wordcount: '1299'
ht-degree: 20%

---


# 使用自定义搜索 Facet {#use-custom-search-facets}

管理员可以向[!UICONTROL 过滤器]面板添加搜索谓词，以自定义搜索并使搜索功能具有通用性。

Brand Portal支持[多面搜索](../using/brand-portal-searching.md#search-using-facets-in-filters-panel)以对已批准的品牌资产进行精细搜索，这可能是由于&#x200B;[**过滤器**&#x200B;面板](../using/brand-portal-searching.md#search-using-facets-in-filters-panel)所致。 通过管理工具中的&#x200B;**[!UICONTROL 搜索表单]**，搜索彩块化可在“过滤器”面板上使用。 在管理工具的“搜索Forms”页面中，存在名为“资产管理搜索边栏”的默认搜索表单。 但是，管理员可以通过添加、修改或删除搜索谓词来编辑默认搜索表单（资产管理搜索边栏），从而自定义默认过滤器面板，从而使搜索功能具有多种用途。

可以使用各种搜索谓词自定义&#x200B;**[!UICONTROL 过滤器]**&#x200B;面板。 例如，添加属性谓词用于搜索与在此谓词中指定的单个属性相匹配的资产。 添加此选项谓词，用于搜索与您为特定属性指定的一个或多个值相匹配的资产。 添加日期范围谓词，用于搜索在指定日期范围内创建的资产。

>[!NOTE]
>
>AEM允许组织将自定义的搜索表单从AEM作者](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal)发布到Brand Portal，而不是在Brand Portal上重新创建相同的表单。[

## 添加搜索谓词{#add-a-search-predicate}

要向&#x200B;**[!UICONTROL 过滤器]**&#x200B;面板添加搜索谓词，请执行以下操作：

1. 要访问管理工具，请单击顶部工具栏中的AEM徽标。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，单击&#x200B;**[!UICONTROL 搜索Forms]**。

   ![](assets/navigation-panel-1.png)

1. 在&#x200B;**[!UICONTROL 搜索Forms]**&#x200B;页面中，选择&#x200B;**[!UICONTROL 资产管理搜索边栏]**。

   ![](assets/search-forms-page.png)

1. 在顶部显示的工具栏上，单击&#x200B;**[!UICONTROL 编辑]**&#x200B;以打开编辑搜索表单。

   ![](assets/edit-search-form-1.png)

1. 在[!UICONTROL 编辑搜索表单]页中，将谓词从[!UICONTROL 选择谓词]选项卡拖到主窗格。 例如，拖动&#x200B;**[!UICONTROL 属性谓词]**。

   主窗格中显示&#x200B;**[!UICONTROL 属性]**&#x200B;字段，右侧的&#x200B;**[!UICONTROL 设置]**&#x200B;选项卡显示属性谓词。

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >**[!UICONTROL 设置]**&#x200B;选项卡中的标题标签标识您选择的谓词类型。

1. 在&#x200B;**[!UICONTROL 设置]**&#x200B;选项卡中，输入属性谓词的标签、占位符文本和描述。

   * 如果希望根据指定的属性值对资产进行部分短语搜索（和通配符搜索），请选择&#x200B;**[!UICONTROL 部分搜索]**。 默认情况下，此谓词支持全文搜索。
   * 如果希望基于属性值的资产搜索不区分大小写，请选择&#x200B;**[!UICONTROL 忽略大小写]**。 默认情况下，搜索筛选器中的属性值会区分大小写。

   >[!NOTE]
   >
   >在选中&#x200B;**[!UICONTROL 部分搜索]**&#x200B;复选框时，默认情况下会选中&#x200B;**[!UICONTROL 忽略大小写]**。

1. 在&#x200B;**[!UICONTROL 属性名称]**&#x200B;字段中，打开属性选取器并选择执行搜索时所依据的属性。 或者，输入属性的名称。 例如，输入 `  jcr :content/metadata/dc:title` 或 `./jcr:content/metadata/dc:title`。

   >[!NOTE]
   >
   >在Brand Portal中，默认情况下将索引`dam:asset`的`jcrcontent/metadata`中的所有属性（以`xmp`开头的属性除外）。
   >
   >创建属性谓词时，可以使用索引的任何属性。 如果配置了任何非索引属性，则未索引属性上的搜索查询可能不会给出任何搜索结果。

   ![](assets/title-prop.png)

1. 单击&#x200B;**[!UICONTROL 完成]**&#x200B;以保存设置。
1. 在[!UICONTROL Assets]用户界面中，单击叠加图标，然后选择&#x200B;**[!UICONTROL Filter]**&#x200B;导航到&#x200B;**[!UICONTROL 过滤器]**&#x200B;面板。 将&#x200B;**[!UICONTROL 属性]**&#x200B;谓词添加到面板。

   ![](assets/property-filter-panel.png)

1. 在&#x200B;**[!UICONTROL 属性]**&#x200B;文本框中输入要搜索的资产的标题。 例如，“Adobe”。 当您执行搜索时，标题与“Adobe”匹配的资产会显示在搜索结果中。

## 搜索谓词列表{#list-of-search-predicates}

与添加&#x200B;**[!UICONTROL Property]**&#x200B;谓词的方式类似，您可以在&#x200B;**[!UICONTROL 过滤器]**&#x200B;面板中添加以下谓词：

| **谓词名称** | **描述** | **属性** |
|-------|-------|----------|
| **[!UICONTROL 路径浏览器]** | 此搜索谓词用于在某个特定位置搜索资产. **注意：** *对于登录用户，“筛选器”上的路径浏览器仅显示与该用户共享的文件夹（及其祖先）的内容结构。* <br> 管理员用户可以使用路径浏览器导航到任意文件夹中的资产，从而搜索任意文件夹中的资产。<br> 而非管理员用户则可以通过在路径浏览器中导航到该文件夹来搜索文件夹（他们可以访问）中的资产。 | <ul><li>字段标签</li><li>路径</li><li>描述</li></ul> |
| **[!UICONTROL 属性]** | 根据特定元数据属性搜索资产。 **注意：在** *选择“部分搜索”时，默认情况下会选择“忽略大小写”*。 | <ul><li>字段标签</li><li>占位符</li><li>属性名称</li><li>部分搜索</li><li>忽略大小写</li><li> 描述</li></ul> |
| **[!UICONTROL 多值属性]** | 与属性谓词类似，但允许多个输入值，以分隔符分隔（默认为COMMA[,]），这些值与任何输入值匹配，结果都会返回。 | <ul><li>字段标签</li><li>占位符</li><li>属性名称</li><li>分隔符支持</li><li>忽略大小写</li><li>描述</li></ul> |
| **[!UICONTROL 标记]** | 此搜索谓词用于根据标记搜索资产。您可以配置“路径”属性，以在“标记”列表中填充各种标记。*注意：如果管理员从AEM发布搜索表单，而路径不包含租户信息，例如[!UICONTROL `/etc/tags/<custom_tag_namespace>`]，则可能需要更改路径值（例如[!UICONTROL `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`]）。 | <ul><li>字段标签</li><li>属性名称</li><li>路径</li><li>描述</li></ul> |
| **[!UICONTROL 路径]** | 此搜索谓词用于在某个特定位置搜索资产. | <ul><li>字段标签</li><li>路径</li><li>描述</li></ul> |  |
| **[!UICONTROL 相对日期]** | 此搜索谓词用于根据创建资产的相对日期搜索资产. | <ul><li>字段标签</li><li>属性名称</li><li>相对日期</li></ul> |
| **[!UICONTROL 范围]** | 此搜索谓词用于搜索属性值指定范围内的资产。 在“过滤器”面板中，可以指定范围的最小和最大属性值。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 日期范围]** | 此搜索谓词用于搜索在日期属性的指定范围内创建的资产。在“过滤器”面板中，可以指定开始和结束日期。 | <ul><li>字段标签</li><li>占位符</li><li>属性名称</li><li>范围文本（始于）</li><li>范围文本（止于）</li><li>描述</li></ul> |
| **[!UICONTROL 日期]** | 此搜索谓词用于根据日期属性进行基于滑块的资产搜索。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 文件大小]** | 此搜索谓词用于根据资产的大小搜索资产. | <ul><li>字段标签</li><li>属性名称</li><li>路径</li><li>描述</li></ul> |
| **[!UICONTROL 上次修改的资源]** | 此搜索谓词用于根据上次修改日期搜索资产。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 批准状态]** | 此搜索谓词用于根据批准元数据属性搜索资产。 默认属性名为&#x200B;**dam:status**。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 签出状态]** | 此搜索谓词用于根据从AEM Assets发布资产时的资产的签出状态搜索资产。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 签出方]** | 此搜索谓词用于根据已签出资产的用户搜索资产。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 到期状态]** | 此搜索谓词用于根据过期状态搜索资产。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 集合成员]** | 此搜索谓词用于根据资产是否是收藏集的一部分来搜索资产。 | 描述 |
| **[!UICONTROL 隐藏]** | 此谓词未对最终用户显式可见，用于任何隐藏约束，通常用于将搜索结果类型限制为&#x200B;**dam:Asset**。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |

>[!NOTE]
>
>请勿使用&#x200B;**[!UICONTROL 选项谓词]**、**[!UICONTROL 发布状态谓词]**&#x200B;和&#x200B;**[!UICONTROL 评级谓词]**，因为这些谓词在品牌门户中不起作用。

## 删除搜索谓词{#delete-a-search-predicate}

要删除搜索谓词，请执行以下步骤：

1. 单击Adobe徽标以访问管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，单击&#x200B;**[!UICONTROL 搜索Forms]**。

   ![](assets/navigation-panel-2.png)

1. 在&#x200B;**[!UICONTROL 搜索Forms]**&#x200B;页面中，选择&#x200B;**[!UICONTROL 资产管理搜索边栏]**。

   ![](assets/search-forms-page.png)

1. 在顶部显示的工具栏上，单击&#x200B;**[!UICONTROL 编辑]**&#x200B;以打开编辑搜索表单。

   ![](assets/edit-search-form-2.png)

1. 在[!UICONTROL 编辑搜索表单]页面中，从主窗格中选择要删除的谓词。 例如，选择&#x200B;**[!UICONTROL 属性谓词]**。

   右侧的&#x200B;**[!UICONTROL 设置]**&#x200B;选项卡显示属性谓词字段。

1. 要删除属性谓词，请单击“素材箱”图标。 在&#x200B;**[!UICONTROL 删除字段]**&#x200B;对话框中，单击&#x200B;**[!UICONTROL 删除]**&#x200B;以确认删除操作。

   将从主窗格中删除&#x200B;**[!UICONTROL 属性谓词]**&#x200B;字段，并且&#x200B;**[!UICONTROL 设置]**&#x200B;选项卡变为空。

   ![](assets/search-form-delete-predicate.png)

1. 要保存更改，请单击工具栏中的&#x200B;**[!UICONTROL 完成]**。
1. 在&#x200B;**[!UICONTROL Assets]**&#x200B;用户界面中，单击叠加图标，然后选择&#x200B;**[!UICONTROL Filter]**&#x200B;导航到&#x200B;**[!UICONTROL 过滤器]**&#x200B;面板。 将从面板中删除&#x200B;**[!UICONTROL 属性]**&#x200B;谓词。

   ![](assets/property-predicate-removed.png)
