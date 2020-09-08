---
title: 在Brand Portal上浏览资产
seo-title: 在Brand Portal上浏览资产
description: 在Brand Portal上使用不同的视图选项和UI元素浏览资产、遍历资产层次结构和搜索资产。
seo-description: 在Brand Portal上使用不同的视图选项和UI元素浏览资产、遍历资产层次结构和搜索资产。
uuid: 178ce217-0050-4922-a204-f4539d46f539
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: introduction
discoiquuid: a70ce694-81d1-4829-9e61-b6412e013e5c
translation-type: tm+mt
source-git-commit: ca60fe1b76c6e99d835457627fcc4bf402b6bd87
workflow-type: tm+mt
source-wordcount: '1039'
ht-degree: 4%

---


# Browse assets on Brand Portal {#browsing-assets-on-brand-portal}

AEM Assets品牌门户提供各种功能和用户界面元素，便于在使用不同视图选项时浏览资源、遍历资产层次结构和搜索资产。

顶部的AEM工具栏中的AEM徽标方便管理员用户访问管理工具面板。

![](assets/aemlogo.png)

![](assets/admin-tools-panel-2.png)

![](assets/bp_subheader.png)<br />

品牌门户中左上角的边栏选择器下拉，可显示用于导航到资产层次结构、简化搜索和显示资源的选项。

![](assets/siderail-1.png)

您可以使用品牌门户右上角的视图选择器中的任何可用视图(卡片、列和列表)视图、导航和选择资产。

![](assets/viewselector.png)

## 查看和选择资源 {#viewing-and-selecting-resources}

从概念上讲，所有视图的查看、导航和选择操作都相同，但操作方式根据所使用的视图而略有不同。

您可以使用任何可用视图视图、导航和选择资源（以对其执行进一步操作）:

* 列视图
* 卡片视图
* 列表视图

### 卡片视图

![](assets/card-view.png)

卡片视图显示各个项目在当前级别的信息卡片。这些卡提供以下详细信息：

* 资产／文件夹的可视表示形式。
* 类型
* 标题
* 名称
* 资产从AEM发布到Brand Portal的日期和时间
* 大小
* 尺寸

You can navigate down the hierarchy by tapping/clicking cards (taking care to avoid the quick actions) or up again by using the [breadcrumbs in the header](https://helpx.adobe.com/experience-manager/6-5/sites/authoring/using/basic-handling.html#TheHeader).

![](assets/cardquickactions.png)

#### 非管理员用户的卡视图

文件夹的卡片在卡片视图中向非管理员用户（编辑者、查看者和客人用户）显示文件夹层次结构信息。 此功能可让用户了解他们访问的文件夹相对于父层次结构的位置。
文件夹层次结构信息对于区分名称与从其他文件夹层次结构共享的其他文件夹相似的文件夹尤为有用。 如果非管理员用户不知道与他们共享的资产的文件夹结构，则名称相似的资产／文件夹似乎会令人混淆。

* 相应卡上显示的路径会被截断以适合卡大小。 但是，用户在将指针悬停在截断的路径上时，可以将完整路径视为工具提示。

![](assets/folder-hierarchy1.png)

**视图资产属性的概述选项**

概述选项对非管理员用户（编辑者、查看者、客人用户）可用，用于视图选定资产／文件夹的资产属性。 概览选项可见：

* 工具栏中，选择资产／文件夹。
* 在下拉菜单中选择边栏选择器。

在选择资 **[!UICONTROL 产]** /文件夹时选择概述选项，用户可以查看资产创建的标题、路径和时间。 但是，在资产详细信息页面上，选择概述选项可让用户查看资产的元数据。

![](assets/overview-option.png)

![](assets/overview-rail-selector.png)

#### 视图卡视图中的设置

**[!UICONTROL 视图设置]** ”对话框在从视图选 **[!UICONTROL 择器中选择]** 视图设置时打开。 它允许您在卡片视图中调整资产缩略图大小。 这样，您就可以个性化视图并控制显示的缩略图数量。

![](assets/cardviewsettings.png)

### 列表视图

![](assets/list-view.png)

列表视图显示当前级别上每个资源的信息。 列表视图提供以下详细信息：

* 资产的缩略图
* 名称
* 标题
* 区域设置
* 类型
* Dimension
* 大小
* 评级
* 显示资产层次结构的文件夹路径<sup>*</sup>
* 在Brand Portal上发布资产的日期

通过“路径”列，您可以轻松地在文件夹层次结构中标识资产位置。 You can navigate down the hierarchy by tapping/clicking the resource name, and back up by using the [breadcrumbs in the header](https://helpx.adobe.com/experience-manager/6-5/sites/authoring/using/basic-handling.html#TheHeader).

<!--
Comment Type: draft lastmodifiedby="mgulati" lastmodifieddate="2018-08-17T03:12:05.096-0400" type="annotation">Removed:- "Selecting assets in list view To select all items in the list, use the checkbox at the upper left of the list. When all items in the list are selected, this check box appears checked. To deselect all, click or tap the checkbox. When only some items are selected, it appears with a minus sign. To select all, click or tap the checkbox. To deselect all, click or tap the checkbox again. You can change the order of items using the dotted vertical bar at the far right of each item in the list. Tap/click the vertical selection bar and drag the item to a new position in the list."
 -->

### 视图列表视图中的设置

列表视图默认 **[!UICONTROL 情况下]** ，资产名称显示为第一列。 还会显示其他信息，如 **[!UICONTROL 资产]**、 **[!UICONTROL 区域设置]**、类 **[!UICONTROL 型、]** Dimension标 ************&#x200B;题、大小、、评级、发布状态等。 However, you can select the columns to be shown using **[!UICONTROL View Settings]**.

![](assets/list-view-setting.png)

### 列视图

![](assets/column-view.png)

使用列视图可以在内容树中浏览一系列级联列。 此视图可帮助您可视化和遍历资产层次结构。

在第一列（最左侧）中选择资源后，在右侧第二列中显示子资源。 选择第二列中的资源后，在右侧的第三列中显示子资源，依此类推。

通过点按或单击资源名称或资源名称右侧的V形标记，可以在树中上下导航。

* 点按或单击资源名称和V形标记时，资源名称和V形标记将高亮显示。
* 点按或单击缩略图会选择资源。
* 选中后，缩略图上会叠加一个复选标记，并突出显示资源名称。
* 最后一列显示选定资源的详细信息。

当在列视图中选择资产时，资产的可视呈现形式会显示在最后的列中，并包含以下详细信息：

* 标题
* 名称
* 尺寸
* 资产从AEM发布到Brand Portal的日期和时间
* 大小
* 类型
* 更多详细信息选项，转到资产的详细信息页面

<!--
Comment Type: draft

<h3>Selecting Resources</h3>
-->

<!--
Comment Type: draft

<p>Selecting a specific resource depends on a combination of the view and the device:</p>
-->

<!--
Comment Type: draft

<table border="1" cellpadding="1" cellspacing="0" width="100%">
<tbody>
<tr>
<td> </td>
<td>Select</td>
<td>Deselect</td>
</tr>
<tr>
<td>Column View<br /> </td>
<td>
<ul>
<li>Desktop:<br /> Mouseover, then use the check mark quick action</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
<td>
<ul>
<li>Desktop:<br /> Click the thumbnail</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
</tr>
<tr>
<td>Card View<br /> </td>
<td>
<ul>
<li>Desktop:<br /> Mouseover, then use the check mark quick action</li>
<li>Mobile device:<br /> Tap-and-hold the card</li>
</ul> </td>
<td>
<ul>
<li>Desktop:<br /> Click the card</li>
<li>Mobile device:<br /> Tap the card</li>
</ul> </td>
</tr>
<tr>
<td>List View</td>
<td>
<ul>
<li>Desktop:<br /> Mouseover, then use the check mark quick action</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
<td>
<ul>
<li>Desktop:<br /> Click the thumbnail</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
</tr>
</tbody>
</table>
-->

<!--
Comment Type: draft

Deselecting All
-->

<!--
Comment Type: draft

<p>In all cases, as you select items the count of the items selected is displayed at the upper right of the toolbar.</p>
<p>You can deselect all items and exit selection mode by clicking or tapping the X next to the count.</p>
-->

<!--
Comment Type: draft

<p>In all views, all items can be deselected by tapping escape on the keyboard if you are using a desktop device.</p>
-->

## 内容树 {#content-tree}

除了这些视图之外，在您视图和选择所需的资产或文件夹时，还可以使用树视图向下展开资产层次结构。

要打开树视图，请点按／单击左上角的边栏选择器，然后从菜 **[!UICONTROL 单中选择]** “内容树”。

![](assets/contenttree.png)

在内容层次结构中，导航到所需的资产。

![](assets/content-tree.png)

## 资源详细信息 {#asset-details}

通过资产详细信息页面，您可以视图资产、下载、共享资产的链接、将资产移动到集合或视图其属性页面。 它还允许您连续浏览同一文件夹中其他资产的详细信息页面。

![](assets/asset-detail.png)

要视图资产的元数据或视图其各种演绎版，请使用资产详细信息页面上的边栏选择器。

![](assets/asset-overview.png)

您可以在资产详细信息页面上视图资产的所有可用演绎版，然后选择一个演绎版以对其进行预览。

![](assets/renditions.png)

要打开资产属性页面，请 **[!UICONTROL 使用顶部栏中的]** “属性”(p)选项。

![](assets/asset-properties.png)

您还可以在资产的属性页面上视图其所有相关资产(AEM上的源资产或派生资产)的列表，因为资产关系也会从AEM发布到品牌门户。
