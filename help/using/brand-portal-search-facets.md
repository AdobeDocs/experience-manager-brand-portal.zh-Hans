---
title: 使用自定义搜索彩块化
description: 管理员可以将搜索谓词添加到“筛选器”面板以自定义搜索并使搜索功能通用。
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
role: Admin
exl-id: c07e1268-2c83-40ba-8dcd-5dade3a10141
source-git-commit: 4c701781e7dc62b9d2b018fd13b1ae9616bbb840
workflow-type: tm+mt
source-wordcount: '1351'
ht-degree: 7%

---

# 使用自定义搜索彩块化 {#use-custom-search-facets}

管理员可以将搜索谓词添加到[!UICONTROL 筛选器]面板以自定义搜索并使搜索功能通用。

Brand Portal支持[面向已批准品牌资产的细粒度搜索](../using/brand-portal-searching.md#search-using-facets-in-filters-panel)，这可能是由于&#x200B;[**筛选器**&#x200B;面板](../using/brand-portal-searching.md#search-using-facets-in-filters-panel)所致。 可通过管理工具中的&#x200B;**[!UICONTROL 搜索表单]**&#x200B;在筛选器面板上提供搜索Facet。 名为“资产管理员搜索边栏”的默认搜索表单存在于管理工具的“搜索Forms”页面中。 但是，管理员可以自定义默认的“筛选器”面板。 他们可以通过添加、编辑或删除搜索谓词来编辑默认搜索表单（资产管理员搜索边栏），从而使搜索功能变得通用。

您可以使用各种搜索谓词来自定义&#x200B;**[!UICONTROL 筛选器]**&#x200B;面板。 例如，添加属性谓词以搜索与您在此谓词中指定的单个属性匹配的资产。 添加选项谓词以搜索与您为特定属性指定的一个或多个值匹配的资源。 添加日期范围谓词以搜索在指定日期范围内创建的资源。

>[!NOTE]
>
>Experience Manager Assets允许组织[将自定义搜索表单从AEM Author](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal)发布到Brand Portal，而不是在Brand Portal上重新创建相同的表单。

## 将搜索谓词添加到“筛选器”面板 {#add-a-search-predicate}

1. 要访问管理工具，请单击顶部工具栏中的Experience Manager徽标。

   ![](assets/aemlogo.png)

1. 在“管理工具”面板中，单击&#x200B;**[!UICONTROL 搜索Forms]**。

   ![](assets/navigation-panel-1.png)

1. 在&#x200B;**[!UICONTROL 搜索Forms]**&#x200B;页面中，选择&#x200B;**[!UICONTROL Assets管理员搜索边栏]**。

   ![](assets/search-forms-page.png)

1. 在顶部显示的工具栏上，单击&#x200B;**[!UICONTROL 编辑]**&#x200B;以打开搜索表单以便进行编辑。

   ![](assets/edit-search-form-1.png)

1. 在[!UICONTROL 编辑搜索表单]页中，将谓词从[!UICONTROL 选择谓词]选项卡拖到主窗格。 例如，拖动&#x200B;**[!UICONTROL 属性谓词]**。

   **[!UICONTROL 属性]**&#x200B;字段显示在主窗格中，右侧的&#x200B;**[!UICONTROL 设置]**&#x200B;选项卡显示属性谓词。

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >**[!UICONTROL 设置]**&#x200B;选项卡中的标题标签标识您选择的谓词类型。

1. 在&#x200B;**[!UICONTROL 设置]**&#x200B;选项卡中，输入属性谓词的标签、占位符文本和说明。

   * 如果要根据指定的属性值允许对资产进行部分短语搜索（和通配符搜索），请选择&#x200B;**[!UICONTROL 部分搜索]**。 默认情况下，谓词支持全文搜索。
   * 如果希望基于属性值的资源搜索不区分大小写，请选择&#x200B;**[!UICONTROL 忽略大小写]**。 默认情况下，搜索筛选器中的属性值搜索是区分大小写的。

   >[!NOTE]
   >
   >选中&#x200B;**[!UICONTROL 部分搜索]**&#x200B;复选框时，默认情况下会选中&#x200B;**[!UICONTROL 忽略大小写]**。

1. 在&#x200B;**[!UICONTROL 属性名称]**&#x200B;字段中，打开属性选取器并选择执行搜索所依据的属性。 或者，输入属性的名称。 例如，输入 `jcr :content/metadata/dc:title` 或 `./jcr:content/metadata/dc:title`。

   >[!NOTE]
   >
   >在Brand Portal中，默认情况下，`dam:asset`的`jcrcontent/metadata`中的所有字符串属性（以`xmp`开头的属性除外）都会编制索引。 默认情况下，任何类型的所有其他自定义属性都不会编制索引。
   >
   >创建属性谓词时，可以使用任何已编制索引的属性。 如果配置了任何非索引属性，则非索引属性上的搜索查询可能不会提供任何搜索结果。

   ![](assets/title-prop.png)

1. 单击&#x200B;**[!UICONTROL 完成]**&#x200B;以保存设置。
1. 从[!UICONTROL Assets]用户界面中，单击叠加图标，然后选择&#x200B;**[!UICONTROL 筛选器]**&#x200B;以导航到&#x200B;**[!UICONTROL 筛选器]**&#x200B;面板。 **[!UICONTROL 属性]**&#x200B;谓词已添加到面板。

   ![](assets/property-filter-panel.png)

1. 在&#x200B;**[!UICONTROL 属性]**&#x200B;文本框中输入要搜索的资源的标题。 例如，“Adobe”。 执行搜索时，标题与“Adobe”匹配的资源将显示在搜索结果中。

## 搜索谓词列表 {#list-of-search-predicates}

与添加&#x200B;**[!UICONTROL 属性]**&#x200B;谓词类似，您可以将以下谓词添加到&#x200B;**[!UICONTROL 筛选器]**&#x200B;面板：

| **谓词名称** | **描述** | **属性** |
|-------|-------|----------|
| **[!UICONTROL 路径浏览器]** | 在特定位置搜索资产的搜索谓词。 **注意：** *对于已登录的用户，筛选器上的路径浏览器仅显示与该用户共享的文件夹（及其祖先）的内容结构。* <br>管理员用户可以使用路径浏览器导航到任何文件夹中的该文件夹，以搜索该文件夹中的资产。 <br>而非管理员用户则可以通过在路径浏览器中导航到某个文件夹（他们有权访问）来搜索该文件夹中的资产。 | <ul><li>字段标签</li><li>路径</li><li>描述</li></ul> |
| **[!UICONTROL 属性]** | 基于特定元数据属性搜索资源。 **注意：** *在选择部分搜索时，默认情况下会选择“忽略大小写”*。 | <ul><li>字段标签</li><li>占位符</li><li>属性名称</li><li>部分搜索</li><li>忽略大小写</li><li> 描述</li></ul> |
| **[!UICONTROL 多值属性]** | 与属性谓词类似，但允许使用多个输入值，各个输入值之间用分隔符（默认为逗号）隔开，这样就会在结果中返回与任何输入值匹配的资产。 | <ul><li>字段标签</li><li>占位符</li><li>属性名称</li><li>分隔符支持</li><li>忽略大小写</li><li>描述</li></ul> |
| **[!UICONTROL 标记]** | 用于根据标记搜索资产的搜索谓词。 您可以配置Path属性以填充“标记”列表中的各种标记。 管理员可能需要更改路径值，例如[!UICONTROL /`etc/tags/mac/<tenant_id>/<custom_tag_namespace>`]。 如果他们从AEM发布搜索表单，并且路径不包含租户信息（例如，[!UICONTROL `/etc/tags/<custom_tag_namespace>`]），则这是必需的。 | <ul><li>字段标签</li><li>属性名称</li><li>路径</li><li>描述</li></ul> |
| **[!UICONTROL 路径]** | 在特定位置搜索资产的搜索谓词。 | <ul><li>字段标签</li><li>路径</li><li>描述</li></ul> |
| **[!UICONTROL 相对日期]** | 根据资产的相对创建日期搜索资产的搜索谓词。 | <ul><li>字段标签</li><li>属性名称</li><li>相对日期</li></ul> |
| **[!UICONTROL 范围]** | 搜索谓词，用于搜索位于指定属性值范围内的资源。 在“筛选器”面板中，可以指定范围的最小和最大属性值。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 日期范围]** | 搜索谓词，用于搜索在指定范围内为日期属性创建的资源。 在“筛选器”面板中，您可以指定开始日期和结束日期。 | <ul><li>字段标签</li><li>占位符</li><li>属性名称</li><li>范围文本（自）</li><li>范围文本（至）</li><li>描述</li></ul> |
| **[!UICONTROL 日期]** | 基于日期属性的基于滑块的资源搜索的搜索谓词。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 文件大小]** | 用于根据资产的大小搜索资产的搜索谓词。 | <ul><li>字段标签</li><li>属性名称</li><li>路径</li><li>描述</li></ul> |
| **[!UICONTROL 上次修改的资产]** | 基于上次修改日期搜索资源的搜索谓词。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 审批状态]** | 搜索谓词，用于根据审批元数据属性搜索资源。 默认属性名称为&#x200B;**`dam:status`**。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 签出状态]** | 搜索谓词，用于在从AEM Assets发布资源时根据资源的签出状态搜索资源。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 签出者]** | 搜索谓词，用于根据已签出资源的用户搜索资源。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 到期状态]** | 用于根据到期状态搜索资产的搜索谓词。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| **[!UICONTROL 收藏集成员]** | 基于资产是否为收藏集一部分的搜索谓词。 | 描述 |
| **[!UICONTROL 隐藏]** | 此谓词对最终用户不可见，用于通常用于将搜索结果类型限制为&#x200B;**`dam:Asset`**&#x200B;的任何隐藏约束。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |

>[!NOTE]
>
>* 请勿使用&#x200B;**[!UICONTROL 选项谓词]**、**[!UICONTROL Publish状态谓词]**&#x200B;和&#x200B;**[!UICONTROL 评级谓词]**，因为这些谓词在Brand Portal中不起作用。
>* Brand Portal不支持文件夹类型谓词`(nt:folder type)`，这可能导致性能问题。 如果它存在于已发布的自定义搜索表单中，则可通过编辑搜索表单将其删除。

## 删除搜索谓词 {#delete-a-search-predicate}

要删除搜索谓词，请执行以下步骤：

1. 单击Adobe徽标可访问管理工具。

   ![](assets/aemlogo.png)

1. 在“管理工具”面板中，单击&#x200B;**[!UICONTROL 搜索Forms]**。

   ![](assets/navigation-panel-2.png)

1. 在&#x200B;**[!UICONTROL 搜索Forms]**&#x200B;页面中，选择&#x200B;**[!UICONTROL Assets管理员搜索边栏]**。

   ![](assets/search-forms-page.png)

1. 在顶部显示的工具栏上，单击&#x200B;**[!UICONTROL 编辑]**&#x200B;以打开搜索表单以便进行编辑。

   ![](assets/edit-search-form-2.png)

1. 在[!UICONTROL 编辑搜索表单]页面中，从主窗格中选择要删除的谓词。 例如，选择&#x200B;**[!UICONTROL 属性谓词]**。

   右侧的&#x200B;**[!UICONTROL 设置]**&#x200B;选项卡显示属性谓词字段。

1. 要删除属性谓词，请单击框图标。 在&#x200B;**[!UICONTROL 删除字段]**&#x200B;对话框中，单击&#x200B;**[!UICONTROL 删除]**&#x200B;以确认删除操作。

   **[!UICONTROL 属性谓词]**&#x200B;字段已从主窗格中删除，**[!UICONTROL 设置]**&#x200B;选项卡变为空。

   ![](assets/search-form-delete-predicate.png)

1. 要保存更改，请单击工具栏中的&#x200B;**[!UICONTROL 完成]**。
1. 从&#x200B;**[!UICONTROL Assets]**&#x200B;用户界面中，单击叠加图标，然后选择&#x200B;**[!UICONTROL 筛选器]**&#x200B;以导航到&#x200B;**[!UICONTROL 筛选器]**&#x200B;面板。 **[!UICONTROL 属性]**&#x200B;谓词已从面板中删除。

   ![](assets/property-predicate-removed.png)
