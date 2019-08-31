---
title: 使用自定义搜索彩块化
seo-title: 使用自定义搜索彩块化
description: 管理员可以将搜索谓词添加到“过滤器”面板以自定义搜索，并使搜索功能变得拼贴。
seo-description: 管理员可以将搜索谓词添加到“过滤器”面板以自定义搜索，并使搜索功能变得拼贴。
uuid: 986fba5a-fac5-4128-ac75-d04 da5 b52 d45
content-type: 引用
topic-tags: administration
products: SG_ EXPERIENCE MANAGER/Brand_ Portal
discoiquuid: 19faa028-246b-42c7-869f-97c95c7a1349
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# 使用自定义搜索彩块化 {#use-custom-search-facets}

管理员可以将搜索谓词添加到 [!UICONTROL “过滤器] ”面板以自定义搜索，并使搜索功能变得拼贴。

Brand Portal支持 [彩块化搜索](../using/brand-portal-searching.md#search-using-facets-in-filters-panel) 以精细搜索已批准的品牌资产，这是 [**由于筛选器** 面板](../using/brand-portal-searching.md#search-using-facets-in-filters-panel)提供的。在“过滤器”面板中，搜索彩块化通过管理工具中 **[!UICONTROL 的搜索表单]** 提供。管理工具中的搜索表单页面中存在名为“资产管理搜索边栏”的默认搜索表单。但是，管理员可以通过添加、修改或删除搜索谓词来自定义默认的“筛选器”面板(资产管理搜索边栏)，从而使搜索功能多样化，从而实现搜索功能的多样化。

您可以使用各种搜索谓词自定义 **[!UICONTROL 筛选器]** 面板。例如，添加属性谓词以搜索与您在此谓词中指定的单个属性匹配的资产。添加用于搜索资产的选项，这些资产与您为特定属性指定的一个或多个值相匹配。添加日期范围谓词，以搜索在指定日期范围内创建的资产。

>[!NOTE]
>
>AEM允许组织将自定义的搜索表单从AEM作者 [](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal) 发布到Brand Portal，而不是在Brand Portal上重新创建同一表单。

## 添加搜索谓词 {#add-a-search-predicate}

要将搜索谓词添加到 **[!UICONTROL “过滤器]** ”面板，请执行以下操作：

1. 要访问管理工具，请单击顶部工具栏中的AEM徽标。

   ![](assets/aemlogo.png)

2. 从管理工具面板中，单击 **[!UICONTROL 搜索表单]**。

   ![](assets/navigation-panel-1.png)

3. 在 **[!UICONTROL 搜索表单]** 页面中，选择 **[!UICONTROL 资产管理搜索边栏]**。

   ![](assets/search-forms-page.png)

4. 在顶部显示的工具栏上，单击 **[!UICONTROL 编辑]** 以打开编辑搜索表单。

   ![](assets/edit-search-form-1.png)

5. In the [!UICONTROL Edit Search Form] page, drag a predicate from the [!UICONTROL Select Predicate] tab to the main pane. For example, drag **[!UICONTROL Property Predicate]**.

   **[!UICONTROL 属性]** 字段将显示在主窗格中，右侧的 **[!UICONTROL “设置]** ”选项卡将显示谓词。

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >**[!UICONTROL 设置]选项卡中的标题标签标识您选择的谓词类型。**

6. 在&#x200B;**[!UICONTROL 设置]选项卡中，输入属性谓词的标签、占位符文本和描述。**

   * 如果您希望基于指定的属性值允许资产的部分短语搜索(和通配符搜索)，请选择 **[!UICONTROL 部分搜索]**。默认情况下，谓词支持全文搜索。
   * 如果您希望基于属性值的资产搜索不区分大小写，请选择 **[!UICONTROL “忽略大小写]**”。默认情况下，搜索筛选器中的属性值区分大小写。
   >[!NOTE]
   >
   >选择 **[!UICONTROL “部分搜索]** ”复选框时， [!UICONTROL 默认情况下会选中“忽略大小写] ”。

7. 在 [!UICONTROL 属性名称] 字段中，打开属性选取器并选择执行搜索的属性。或者，输入属性的名称。例如，输入 [!UICONTROL `  jcr :content/metadata/dc:title`] 或 [!UICONTROL `./jcr:content/metadata/dc:title`].

   ![](assets/title-prop.png)

8. 单击&#x200B;**[!UICONTROL 完成]以保存设置。**
9. 从 [!UICONTROL 资产] 用户界面中，单击叠加图标，然后选择 **[!UICONTROL 筛选器]** 以导航到 **[!UICONTROL 筛选器]** 面板。**[!UICONTROL 属性]** 谓词将添加到面板。

   ![](assets/property-filter-panel.png)

10. Enter a title for the asset to be searched in the **[!UICONTROL Property]** text box. 例如，“Adobe”。执行搜索时，搜索结果中会显示标题与“Adobe”匹配的资产。

## 搜索谓词列表 {#list-of-search-predicates}

与添加 **[!UICONTROL 属性]** 谓词的方式相似，您可以将以下谓词添加到 **[!UICONTROL “过滤器]** ”面板：

| **谓词名称** | **描述** | **属性** |
|-------|-------|----------|
| [!UICONTROL 路径浏览器] | 此搜索谓词用于在某个特定位置搜索资产. **注意：***对于登录用户，“过滤器”上的路径浏览器仅显示与该用户共享的文件夹(及其上级)的内容结构。*<br> 管理员用户可以使用路径浏览器导航到该文件夹，从而在任何文件夹中搜索资产。<br> 但是，非管理员用户可以通过在路径浏览器中导航到该文件夹来在文件夹中搜索资产(可访问)。 | <ul><li>字段标签</li><li>路径</li><li>描述</li></ul> |
| [!UICONTROL 属性] | 根据特定元数据属性搜索资产。**注意：***选择“部分搜索”时，默认情况下将选择“忽略大小写*”。 | <ul><li>字段标签</li><li>占位符</li><li>属性名称</li><li>部分搜索</li><li>忽略大小写</li><li> 描述</li></ul> |
| [!UICONTROL 多值属性] | 与属性谓词相似，但允许多个输入值(默认为COMA[，])与任何输入值相匹配的多个输入值在结果中返回。 | <ul><li>字段标签</li><li>占位符</li><li>属性名称</li><li>分隔符支持</li><li>忽略大小写</li><li>描述</li></ul> |
| [!UICONTROL 标记] | 此搜索谓词用于根据标记搜索资产。您可以配置“路径”属性，以在“标记”列表中填充各种标记。*注意：管理员可能需要更改路径值(例如， [!UICONTROL `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`]如果他们从AEM发布搜索表单，则路径不包括租户信息，例如，) [!UICONTROL `/etc/tags/<custom_tag_namespace>`]。 | <ul><li>字段标签</li><li>属性名称</li><li>路径</li><li>描述</li></ul> |
| [!UICONTROL 路径] | 此搜索谓词用于在某个特定位置搜索资产. | <ul><li>字段标签</li><li>路径</li><li>描述</li></ul> |  |
| [!UICONTROL 相对日期] | 此搜索谓词用于根据创建资产的相对日期搜索资产. | <ul><li>字段标签</li><li>属性名称</li><li>相对日期</li></ul> |
| [!UICONTROL 范围] | 此搜索谓词用于搜索位于特定范围的属性值内的资产。在“过滤器”面板中，您可以为范围指定最小和最大属性值。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| [!UICONTROL 日期范围] | 此搜索谓词用于搜索在日期属性的指定范围内创建的资产。在“过滤器”面板中，您可以指定开始日期和结束日期。 | <ul><li>字段标签</li><li>占位符</li><li>属性名称</li><li>范围文本（始于）</li><li>范围文本（止于）</li><li>描述</li></ul> |
| [!UICONTROL 日期] | 此搜索谓词用于根据日期属性进行基于滑块的资产搜索。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| [!UICONTROL 文件大小] | 此搜索谓词用于根据资产的大小搜索资产. | <ul><li>字段标签</li><li>属性名称</li><li>路径</li><li>描述</li></ul> |
| [!UICONTROL 上次修改的资源] | 此搜索谓词用于根据上次修改的日期搜索资产。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| [!UICONTROL 批准状态] | 此搜索谓词用于根据批准元数据属性搜索资产。默认属性名称为 **dam：状态**。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| [!UICONTROL 签出状态] | 此搜索谓词用于根据资产从AEM资产发布时的注销状态搜索资产。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| [!UICONTROL 签出方] | 此搜索谓词用于根据已注销资产的用户搜索资产。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| [!UICONTROL 到期状态] | 此搜索谓词用于根据过期状态搜索资产。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |
| [!UICONTROL 集合成员] | 此搜索谓词用于根据资产是否是集合的一部分搜索资产。 | 描述 |
| [!UICONTROL 隐藏] | 此谓词不对最终用户明显可见，并且通常用于限制将搜索结果类型限制 **为DAM的任何隐藏约束：资产**。 | <ul><li>字段标签</li><li>属性名称</li><li>描述</li></ul> |

>[!NOTE]
>
>请勿在Brand Portal中使用 **[!UICONTROL 选项谓词]**、 **[!UICONTROL Publish Status谓词]**&#x200B;和 **[!UICONTROL 评级谓词]** 等谓词谓词。

## 删除搜索谓词 {#delete-a-search-predicate}

要删除搜索谓词，请执行以下步骤：

1. 单击Adobe徽标可访问管理工具。

   ![](assets/aemlogo.png)

2. 从管理工具面板中，单击 **[!UICONTROL 搜索表单]**。

   ![](assets/navigation-panel-2.png)

3. 在 **[!UICONTROL 搜索表单]** 页面中，选择 **[!UICONTROL 资产管理搜索边栏]**。

   ![](assets/search-forms-page.png)

4. 在顶部显示的工具栏上，单击 **[!UICONTROL 编辑]** 以打开编辑搜索表单。

   ![](assets/edit-search-form-2.png)

5. 在 [!UICONTROL 编辑搜索表单] 页面的主窗格中，选择要删除的谓词。For example, select **[!UICONTROL Property Predicate]**.

   右侧的 **[!UICONTROL “设置]** ”选项卡显示谓词字段。

6. 要删除属性谓词，请单击bin图标。在 **[!UICONTROL 删除字段]** 对话框中，单击 **[!UICONTROL 删除]** 以确认删除操作。

   **[!UICONTROL 属性谓词]** 字段将从主窗格中删除， **[!UICONTROL 设置]** 选项卡将变为空。

   ![](assets/search-form-delete-predicate.png)

7. 要保存更改，请在工具栏中单击 **[!UICONTROL 完成]** 。
8. 从 **[!UICONTROL 资产]** 用户界面中，单击叠加图标，然后选择 **[!UICONTROL 筛选器]** 以导航到 **[!UICONTROL 筛选器]** 面板。**[!UICONTROL 将从面板中删除属性]** 谓词。

   ![](assets/property-predicate-removed.png)
