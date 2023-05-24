---
title: 使用自定义搜索 Facet
seo-title: Use custom search facets
description: 管理员可以将搜索谓词添加到“筛选器”面板以自定义搜索并使搜索功能通用。
seo-description: Administrators can add search predicates to the Filters panel to customize search and make the search functionality versatile.
uuid: 986fba5a-fac5-4128-ac75-d04da5b52d45
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 19faa028-246b-42c7-869f-97c95c7a1349
role: Admin
exl-id: c07e1268-2c83-40ba-8dcd-5dade3a10141
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '1279'
ht-degree: 9%

---

# 使用自定义搜索 Facet {#use-custom-search-facets}

管理员可以将搜索谓词添加到 [!UICONTROL 筛选器] 用于自定义搜索并使搜索功能通用的面板。

Brand Portal支持 [分面搜索](../using/brand-portal-searching.md#search-using-facets-in-filters-panel) 用于精细地搜索已批准的品牌资产，可能的原因是 [**筛选器** 面板](../using/brand-portal-searching.md#search-using-facets-in-filters-panel). 搜索Facet可通过以下方式在“筛选器”面板中提供 **[!UICONTROL 搜索表单]** （在管理工具中）。 管理工具的“搜索Forms”页面中存在一个名为资产管理员搜索边栏的默认搜索表单。 但是，管理员可以通过添加、修改或删除搜索谓词来编辑默认搜索表单（资产管理员搜索边栏），从而自定义默认的“筛选器”面板，从而使搜索功能变得通用。

您可以使用各种搜索谓词来自定义 **[!UICONTROL 筛选器]** 面板。 例如，添加属性谓词以搜索与您在此谓词中指定的单个属性匹配的资产。 添加选项谓词以搜索与您为特定属性指定的一个或多个值匹配的资产。 添加日期范围谓词以搜索在指定日期范围内创建的资源。

>[!NOTE]
>
>Experience Manager Assets允许组织 [从AEM作者发布自定义搜索表单](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal) Brand Portal ，而不是在Brand Portal上重新创建相同的表单。

## 添加搜索谓词 {#add-a-search-predicate}

将搜索谓词添加到 **[!UICONTROL 筛选器]** 面板：

1. 要访问管理工具，请单击顶部工具栏中的Experience Manager徽标。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，单击 **[!UICONTROL 搜索Forms]**.

   ![](assets/navigation-panel-1.png)

1. 在 **[!UICONTROL 搜索Forms]** 页面，选择 **[!UICONTROL 资产管理搜索边栏]**.

   ![](assets/search-forms-page.png)

1. 在顶部显示的工具栏上，单击 **[!UICONTROL 编辑]** 以打开“编辑搜索”表单。

   ![](assets/edit-search-form-1.png)

1. 在 [!UICONTROL 编辑搜索表单] 页面，从拖动谓词 [!UICONTROL 选择谓词] 制表符进入主窗格。 例如，拖动 **[!UICONTROL 属性谓词]**.

   此 **[!UICONTROL 属性]** 字段显示在主窗格中， **[!UICONTROL 设置]** 选项卡在右侧显示属性谓词。

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >中的标题标签 **[!UICONTROL 设置]** 选项卡标识您选择的谓词类型。

1. 在 **[!UICONTROL 设置]** 选项卡，输入属性谓词的标签、占位符文本和说明。

   * 选择 **[!UICONTROL 部分搜索]**，如果您要根据指定的属性值允许进行资产的部分短语搜索（和通配符搜索）。 默认情况下，谓词支持全文搜索。
   * 选择 **[!UICONTROL 忽略大小写]**，如果希望基于属性值的资源搜索不区分大小写。 默认情况下，搜索筛选器中的属性值搜索区分大小写。

   >[!NOTE]
   >
   >选择时 **[!UICONTROL 部分搜索]** 复选框， **[!UICONTROL 忽略大小写]** 默认情况下处于选中状态。

1. 在 **[!UICONTROL 属性名称]** 字段中，打开属性选取器，然后选择要执行搜索的属性。 或者，输入属性的名称。 例如，输入 `  jcr :content/metadata/dc:title` 或 `./jcr:content/metadata/dc:title`。

   >[!NOTE]
   >
   >在Brand Portal中，所有资产(以开始的 `xmp`)，位于 `jcrcontent/metadata` 之 `dam:asset` 默认情况下已编制索引。
   >
   >创建属性谓词时可以使用任何已编制索引的属性。 如果配置了任何非索引属性，则非索引属性上的搜索查询可能不会提供任何搜索结果。

   ![](assets/title-prop.png)

1. 单击 **[!UICONTROL 完成]** 以保存设置。
1. 从 [!UICONTROL 资产] 用户界面，单击叠加图标并选择 **[!UICONTROL 筛选条件]** 导航到 **[!UICONTROL 筛选器]** 面板。 此 **[!UICONTROL 属性]** 谓词将添加到面板。

   ![](assets/property-filter-panel.png)

1. 在中输入要搜索的资源的标题 **[!UICONTROL 属性]** 文本框。 例如，“Adobe”。 执行搜索时，标题与“Adobe”匹配的资源将显示在搜索结果中。

## 搜索谓词列表 {#list-of-search-predicates}

类似于添加 **[!UICONTROL 属性]** 谓词，可以将以下谓词添加到 **[!UICONTROL 筛选器]** 面板：

| **谓词名称** | **描述** | **属性** |
|-------|-------|----------|
| **[!UICONTROL 路径浏览器]** | 搜索谓词以搜索特定位置的资源。 **注意：** *对于已登录的用户，过滤器上的路径浏览器仅显示与该用户共享的文件夹（及其祖先）的内容结构。* <br> 管理员用户可以使用路径浏览器导航到任何文件夹中的该文件夹，以搜索该文件夹中的资产。 <br> 相反，非管理员用户可以通过在路径浏览器中导航到文件夹（他们有权访问）来搜索该文件夹中的资产。 | <ul><li>字段标签</li><li>路径</li><li>描述</li></ul> |
| **[!UICONTROL 属性]** | 根据特定的元数据属性搜索资源。 **注意：** *在选择“部分搜索”时，默认情况下会选中“忽略大小写”*. | <ul><li>字段标签</li><li>占位符</li><li>属性名称</li><li>部分搜索</li><li>忽略大小写</li><li> 描述</li></ul> |
| **[!UICONTROL 多值属性]** | 与属性谓词类似，但允许使用多个输入值，以分隔符分隔（默认值为COMMA）[，])在结果中返回与任何输入值匹配的资产。 | <ul><li>字段标签</li><li>占位符</li><li>属性名称</li><li>分隔符支持</li><li>忽略大小写</li><li>描述</li></ul> |
| **[!UICONTROL 标记]** | 搜索谓词，以基于标记搜索资产。 您可以配置Path属性以填充“标记”列表中的各种标记。 *注意：管理员可能需要更改路径值，例如 [!UICONTROL `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`]，如果它们从AEM发布搜索表单，其中路径不包括租户信息，例如， [!UICONTROL `/etc/tags/<custom_tag_namespace>`]. | <ul><li>字段标签</li><li>属性名称</li><li>路径</li><li>描述</li></ul> |
| **[!UICONTROL 路径]** | 搜索谓词以搜索特定位置的资源。 | <ul><li>字段标签</li><li>路径</li><li>描述</li></ul> |  |
| **[!UICONTROL 相对日期]** | 搜索谓词，以根据资产的相对创建日期搜索资产。 | <ul><li>字段标签</li><li>属性名称</li><li>相对日期</li></ul> |
| **[!UICONTROL 范围]** | 搜索谓词，可搜索位于指定属性值范围内的资产。 在“筛选器”面板中，您可以指定范围的最小和最大属性值。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 日期范围]** | 搜索谓词，以搜索在指定范围内为日期属性创建的资产。 在“筛选器”面板中，您可以指定开始日期和结束日期。 | <ul><li>字段标签</li><li>占位符</li><li>属性名称</li><li>范围文本（自）</li><li>范围文本（至）</li><li>描述</li></ul> |
| **[!UICONTROL 日期]** | 基于日期属性的资产基于滑块搜索的搜索谓词。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 文件大小]** | 搜索谓词，以根据资产的大小搜索资产。 | <ul><li>字段标签</li><li>属性名称</li><li>路径</li><li>描述</li></ul> |
| **[!UICONTROL 上次修改的资源]** | 搜索谓词，以根据上次修改日期搜索资源。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 审批状态]** | 搜索谓词，以根据审批元数据属性搜索资源。 默认属性名称为 **dam：status**. | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 签出状态]** | 搜索谓词，以在从AEM Assets发布资源时根据资源的签出状态搜索资源。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 签出方]** | 搜索谓词，以根据已签出资源的用户搜索资源。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 到期状态]** | 搜索谓词，以根据过期状态搜索资源。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 收藏集成员]** | 搜索谓词，用于根据资产是否为收藏集的一部分来搜索资产。 | 描述 |
| **[!UICONTROL 隐藏]** | 此谓词对最终用户不可见，用于任何隐藏的约束，通常用于将搜索结果类型限制为 **dam：Asset**. | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |

>[!NOTE]
>
>不使用 **[!UICONTROL 选项谓词]**， **[!UICONTROL 发布状态谓词]**、和 **[!UICONTROL 评级谓词]** 因为这些谓词在Brand Portal中不起作用。

## 删除搜索谓词 {#delete-a-search-predicate}

要删除搜索谓词，请执行以下步骤：

1. 单击Adobe徽标可访问管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，单击 **[!UICONTROL 搜索Forms]**.

   ![](assets/navigation-panel-2.png)

1. 在 **[!UICONTROL 搜索Forms]** 页面，选择 **[!UICONTROL 资产管理搜索边栏]**.

   ![](assets/search-forms-page.png)

1. 在顶部显示的工具栏上，单击 **[!UICONTROL 编辑]** 以打开“编辑搜索”表单。

   ![](assets/edit-search-form-2.png)

1. 在 [!UICONTROL 编辑搜索表单] 页上，从主窗格中选择要删除的谓词。 例如，选择 **[!UICONTROL 属性谓词]**.

   此 **[!UICONTROL 设置]** 选项卡的右侧显示属性谓词字段。

1. 要删除属性谓词，请单击框图标。 在 **[!UICONTROL 删除字段]** 对话框中，单击 **[!UICONTROL 删除]** 以确认删除操作。

   此 **[!UICONTROL 属性谓词]** 字段将从主窗格中删除，并且 **[!UICONTROL 设置]** 制表符将为空。

   ![](assets/search-form-delete-predicate.png)

1. 要保存更改，请单击 **[!UICONTROL 完成]** 工具栏中。
1. 从 **[!UICONTROL 资产]** 用户界面，单击叠加图标并选择 **[!UICONTROL 筛选条件]** 导航到 **[!UICONTROL 筛选器]** 面板。 此 **[!UICONTROL 属性]** 谓词将从面板中删除。

   ![](assets/property-predicate-removed.png)
