---
title: 使用自定义搜索 Facet
seo-title: 使用自定义搜索 Facet
description: 管理员可以向“筛选器”面板添加搜索谓词，以自定义搜索并使搜索功能具备多种用途。
seo-description: 管理员可以向“筛选器”面板添加搜索谓词，以自定义搜索并使搜索功能具备多种用途。
uuid: 986fba5a-fac5-4128-ac75-d04da5b52d45
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 19faa028-246b-42c7-869f-97c95c7a1349
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873

---


# 使用自定义搜索 Facet {#use-custom-search-facets}

管理员可以向“筛选器”面板添 [!UICONTROL 加搜索谓词] ，以自定义搜索并使搜索功能具备多种用途。

Brand Portal支持多 [面搜索](../using/brand-portal-searching.md#search-using-facets-in-filters-panel) ，以便对已批准的品牌资产进行精细搜索，这可能由于“筛选器”面 [**板而实现&#x200B;**](../using/brand-portal-searching.md#search-using-facets-in-filters-panel)。 搜索彩块化可通过管理工具中的搜索**[!UICONTROL &#x200B;表单]** ，在“筛选器”面板上使用。 在管理工具的“搜索表单”页面中，存在名为“资产管理员搜索边栏”的默认搜索表单。 但是，管理员可以通过添加、修改或删除搜索谓词来编辑默认的搜索表单（资产管理员搜索边栏），从而自定义默认的“筛选器”面板，从而使搜索功能具有通用性。

您可以使用各种搜索谓词自定义“筛 **[!UICONTROL 选器]**”面板。 例如，添加属性谓词以搜索与您在此谓词中指定的单个属性相匹配的资产。 添加选项谓词以搜索与您为特定属性指定的一个或多个值相匹配的资产。 添加日期范围谓词以搜索在指定日期范围内创建的资产。

>[!NOTE]
>
>AEM允许组织将 [自定义的搜索表单从AEM作者发布到Brand Portal](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal) ，而不是在Brand Portal上重新创建相同的表单。

## 添加搜索谓词 {#add-a-search-predicate}

要向“筛选器”面板添加搜索谓 **[!UICONTROL 词]**:

1. 要访问管理工具，请单击顶部工具栏中的AEM徽标。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，单击“ **[!UICONTROL 搜索表单”]**。

   ![](assets/navigation-panel-1.png)

1. 在“搜索 **[!UICONTROL 表单]**”页面中，选择“资**[!UICONTROL &#x200B;产管理员搜索边栏”]**。

   ![](assets/search-forms-page.png)

1. 在顶部显示的工具栏上，单击“编 **[!UICONTROL 辑]**”以打开编辑搜索表单。

   ![](assets/edit-search-form-1.png)

1. In the [!UICONTROL Edit Search Form] page, drag a predicate from the [!UICONTROL Select Predicate] tab to the main pane. For example, drag **[!UICONTROL Property Predicate]**.

   主窗 **[!UICONTROL 格中显示]**“属性”字段，右侧的“设**[!UICONTROL &#x200B;置]** ”选项卡显示属性谓词。

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >**[!UICONTROL 设置]**选项卡中的标题标签标识您选择的谓词类型。

1. 在&#x200B;**[!UICONTROL 设置]**选项卡中，输入属性谓词的标签、占位符文本和描述。

   * 如果 ****要允许基于指定属性值对资产进行部分短语搜索（和通配符搜索），请选择部分搜索。 默认情况下，此谓词支持全文搜索。
   * 如果 ****希望基于属性值的资产搜索不区分大小写，请选择忽略大小写。 默认情况下，搜索筛选器中的属性值搜索区分大小写。
   >[!NOTE]
   >
   >在选中“部 **[!UICONTROL 分搜索]**”复选框时，**[!UICONTROL &#x200B;默认情况下会选中“忽略大小写]** ”。

1. 在“属 **[!UICONTROL 性名称]**”字段中，打开属性选取器并选择执行搜索时所依据的属性。 或者，输入属性的名称。 例如，输入`  jcr :content/metadata/dc:title`或`./jcr:content/metadata/dc:title`。

   ![](assets/title-prop.png)

1. 单击&#x200B;**[!UICONTROL 完成]**以保存设置。
1. 在“资 [!UICONTROL 产] ”用户界面中，单击叠加图标并选择“筛选器” ****，以导航到“**[!UICONTROL &#x200B;筛选器]** ”面板。 The **[!UICONTROL Property]**predicate is added to the panel.

   ![](assets/property-filter-panel.png)

1. Enter a title for the asset to be searched in the **[!UICONTROL Property]**text box. 例如，“Adobe”。 执行搜索时，标题与“Adobe”匹配的资产会显示在搜索结果中。

## 搜索谓词列表 {#list-of-search-predicates}

与添加“属性”谓词的方 **[!UICONTROL 式类似]**，您可以向“筛选器”面板添加以下谓**[!UICONTROL &#x200B;词]** :

| **谓词名称** | **描述** | **属性** |
|-------|-------|----------|
| **[!UICONTROL 路径浏览器]** | 此搜索谓词用于在某个特定位置搜索资产. **** 注意：对 *于登录用户，“筛选器”上的路径浏览器仅显示与用户共享的文件夹（及其祖先）的内容结构。* 管 <br> 理员用户可以使用路径浏览器导航到任意文件夹中的资产，从而搜索该文件夹中的资产。 <br> 但是，非管理员用户可以通过在路径浏览器中导航到该文件夹来搜索文件夹中的资产（可供他们访问）。 | <ul><li>字段标签</li><li>路径</li><li>描述</li></ul> |
| **[!UICONTROL 属性]** | 根据特定元数据属性搜索资产。 **** 注意：在选 *择“部分搜索”时，默认情况下会选择“忽略大小写”*。 | <ul><li>字段标签</li><li>占位符</li><li>属性名称</li><li>部分搜索</li><li>忽略大小写</li><li> 描述</li></ul> |
| **[!UICONTROL 多值属性]** | 与属性谓词类似，但允许多个输入值以分隔符分隔(默认为COMMA[,])，这些值与任何输入值相匹配的资产将在结果中返回。 | <ul><li>字段标签</li><li>占位符</li><li>属性名称</li><li>分隔符支持</li><li>忽略大小写</li><li>描述</li></ul> |
| **[!UICONTROL 标记]** | 此搜索谓词用于根据标记搜索资产。您可以配置“路径”属性，以在“标记”列表中填充各种标记。*注意：例如，如果管理员从AEM发布搜索表单（其中路径不包括租户信息），则可能需要更改路径值，例如 [!UICONTROL `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`][!UICONTROL `/etc/tags/<custom_tag_namespace>`]。 | <ul><li>字段标签</li><li>属性名称</li><li>路径</li><li>描述</li></ul> |
| **[!UICONTROL 路径]** | 此搜索谓词用于在某个特定位置搜索资产. | <ul><li>字段标签</li><li>路径</li><li>描述</li></ul> |  |
| **[!UICONTROL 相对日期]** | 此搜索谓词用于根据创建资产的相对日期搜索资产. | <ul><li>字段标签</li><li>属性名称</li><li>相对日期</li></ul> |
| **[!UICONTROL 范围]** | 此搜索谓词用于搜索属性值指定范围内的资产。 在“滤镜”面板中，可指定范围的最小和最大属性值。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 日期范围]** | 此搜索谓词用于搜索在日期属性的指定范围内创建的资产。在“过滤器”面板中，可指定开始和结束日期。 | <ul><li>字段标签</li><li>占位符</li><li>属性名称</li><li>范围文本（始于）</li><li>范围文本（止于）</li><li>描述</li></ul> |
| **[!UICONTROL 日期]** | 此搜索谓词用于根据日期属性进行基于滑块的资产搜索。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 文件大小]** | 此搜索谓词用于根据资产的大小搜索资产. | <ul><li>字段标签</li><li>属性名称</li><li>路径</li><li>描述</li></ul> |
| **[!UICONTROL 上次修改的资源]** | 此搜索谓词用于根据上次修改日期搜索资产。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 批准状态]** | 此搜索谓词用于根据批准元数据属性搜索资产。 默认属性名称 **为dam:status**。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 签出状态]** | 此搜索谓词用于根据从AEM资产发布资产时资产的注销状态搜索资产。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 签出方]** | 此搜索谓词用于根据已注销资产的用户搜索资产。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 到期状态]** | 此搜索谓词用于根据到期状态搜索资产。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 集合成员]** | 此搜索谓词用于根据资产是否是集合的一部分来搜索资产。 | 描述 |
| **[!UICONTROL 隐藏]** | 此谓词未对最终用户显式可见，它用于任何隐藏约束，通常用于将搜索结果类型限制 **为dam:Asset**。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |

>[!NOTE]
>
>请勿使用“选 **[!UICONTROL 项谓词]**”、“发布状**[!UICONTROL &#x200B;态谓词”和“评级谓词]******”，因为这些谓词在Brand Portal中不起作用。

## 删除搜索谓词 {#delete-a-search-predicate}

要删除搜索谓词，请执行以下步骤：

1. 单击Adobe徽标以访问管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，单击“ **[!UICONTROL 搜索表单”]**。

   ![](assets/navigation-panel-2.png)

1. 在“搜索 **[!UICONTROL 表单]**”页面中，选择“资**[!UICONTROL &#x200B;产管理员搜索边栏”]**。

   ![](assets/search-forms-page.png)

1. 在顶部显示的工具栏上，单击“编 **[!UICONTROL 辑]**”以打开编辑搜索表单。

   ![](assets/edit-search-form-2.png)

1. 在“编 [!UICONTROL 辑搜索表单] ”页面的主窗格中，选择要删除的谓词。 For example, select **[!UICONTROL Property Predicate]**.

   右侧 **[!UICONTROL 的“设置]**”选项卡显示属性谓词字段。

1. 要删除属性谓词，请单击素材箱图标。 在“删 **[!UICONTROL 除字段]**”对话框中，单击“**[!UICONTROL &#x200B;删除]** ”以确认删除操作。

   属性 **[!UICONTROL 谓词字段将从主窗格中删除]**，并且设置选**[!UICONTROL &#x200B;项卡变]** 为空。

   ![](assets/search-form-delete-predicate.png)

1. 要保存更改，请单击工 **[!UICONTROL 具栏中]**的完成。
1. 在“资 **[!UICONTROL 产]**”用户界面中，单击叠加图标并选择“筛选器”**** ，以导航到“ **[!UICONTROL 筛选器]**”面板。 The**[!UICONTROL  Property]** predicate is removed from the panel.

   ![](assets/property-predicate-removed.png)
