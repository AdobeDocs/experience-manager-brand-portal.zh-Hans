---
title: 在Brand Portal上浏览资产
seo-title: Browse assets on Brand Portal
description: 在Brand Portal上使用不同的视图选项和UI元素浏览资产、遍历资产层次结构并搜索资产。
seo-description: Browse through assets, traverse asset hierarchies, and search assets, using different view options and UI elements on Brand Portal.
uuid: 178ce217-0050-4922-a204-f4539d46f539
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: introduction
discoiquuid: a70ce694-81d1-4829-9e61-b6412e013e5c
exl-id: 405d7861-a140-44b1-ae1f-4f0839f05033
source-git-commit: e7545344a0fc6dd5e0176705a16625c2976e0de6
workflow-type: tm+mt
source-wordcount: '1014'
ht-degree: 4%

---

# 在Brand Portal上浏览资产 {#browsing-assets-on-brand-portal}

Experience Manager Assets Brand Portal provides various capabilities and user interface elements that facilitate browsing through resources, traversing asset hierarchies, and searching assets while using different view options.

Experience Manager顶部工具栏中的徽标有助于管理员用户访问管理工具面板。

![](assets/aemlogo.png)

![](assets/admin-tools-panel-2.png)

![](assets/bp_subheader.png)

Rail selector at the upper left in Brand Portal drops-down to expose options to navigate into asset hierarchies, streamline your search, and display resources.

![](assets/siderail-1.png)

您可以使用Brand Portal右上角的视图选择器中的任意可用视图（卡片视图、列视图和列表视图）查看、导航和选择资产。

![](assets/viewselector.png)

## 查看和选择资源 {#viewing-and-selecting-resources}

从概念上讲，所有视图中的查看、导航和选择操作都相同，只是操作方法根据所使用的视图而略有差异。

您可以使用以下任何可用视图查看、导航和选择资源（以对其执行进一步操作）：

* 列视图
* 卡片视图
* 列表视图

### 卡片视图

![](assets/card-view.png)

卡片视图显示各个项目在当前级别的信息卡片。这些卡片提供了以下详细信息：

* A visual representation of the asset/folder.
* 类型
* 标题
* 名称
* 资产从AEM发布到Brand Portal的日期和时间
* 大小
* 尺寸

您可以通过点按/单击卡片对层次结构进行向下导航（注意避免快速操作），或使用标题](https://experienceleague.adobe.com/docs/experience-manager-65/authoring/essentials/basic-handling.html)中的[痕迹导航再次向上导航。

![](assets/cardquickactions.png)

#### Card view for non-admin users

文件夹卡片在卡片视图中向非管理员用户（编辑者、查看者和来宾用户）显示文件夹层次结构信息。 通过此功能，用户可以了解文件夹的位置以及他们正在访问的文件夹相对于父层次结构的位置。
文件夹层次结构信息在区分名称与从其他文件夹层次结构共享的其他文件夹相似的文件夹时特别有用。 If the non-admin users are not aware of the folder structure of the assets shared with them, assets /folders with similar names seem confusing.

* 相应卡片上显示的路径会被截断以适合卡片大小。 但是，用户可以将完整路径视为将鼠标悬停在截断路径上的工具提示。

![](assets/folder-hierarchy1.png)

**查看资产属性的概述选项**

Overview option is available to non-admin users (Editors, Viewers, Guest users) to view Asset Properties of selected assets/folders. 概述选项可见：

* （位于顶部的工具栏中）。
* 在下拉菜单中，选择边栏选择器。

在选择资产/文件夹时，选择&#x200B;**[!UICONTROL 概述]**&#x200B;选项后，用户可以查看资产创建的标题、路径和时间。 然而，在资产详细信息页面上选择概述选项，用户可以查看资产的元数据。

![](assets/overview-option.png)

![](assets/overview-rail-selector.png)

#### 在卡片视图中查看设置

**[!UICONTROL 查看]** 设置对话框在从视图选择器 **[!UICONTROL 中选择]** 查看设置时打开。它允许您在卡片视图中调整资产缩略图的大小。 这样，您就可以个性化视图并控制显示的缩略图数量。

![](assets/cardviewsettings.png)

### 列表视图

![](assets/list-view.png)

列表视图显示每个资源在当前级别的信息。 列表视图提供以下详细信息：

* 资产的缩略图
* 名称
* 标题
* 区域设置
* 类型
* Dimension
* 大小
* 评级
* Folder path showing asset hierarchy
* 在Brand Portal上发布资产的日期

Path column lets you easily identify asset location in the folder hierarchy. 您可以通过点按/单击资源名称对层次结构进行向下导航，然后使用标题](https://experienceleague.adobe.com/docs/experience-manager-65/authoring/essentials/basic-handling.html)中的[痕迹导航再次向上导航。

<!--
Comment Type: draft lastmodifiedby="mgulati" lastmodifieddate="2018-08-17T03:12:05.096-0400" type="annotation">Removed:- "Selecting assets in list view To select all items in the list, use the checkbox at the upper left of the list. When all items in the list are selected, this check box appears checked. To deselect all, click or tap the checkbox. When only some items are selected, it appears with a minus sign. To select all, click or tap the checkbox. To deselect all, click or tap the checkbox again. You can change the order of items using the dotted vertical bar at the far right of each item in the list. Tap/click the vertical selection bar and drag the item to a new position in the list."
 -->

### 在列表视图中查看设置

List view shows asset **[!UICONTROL Name]** as the first column by default. 此外，还显示资产&#x200B;**[!UICONTROL 标题]**、**[!UICONTROL 区域设置]**、**[!UICONTROL 类型]**、**[!UICONTROL Dimension]**、**[!UICONTROL 大小]**、**[!UICONTROL 评级]**、发布状态等其他信息。 但是，您可以使用&#x200B;**[!UICONTROL 查看设置]**&#x200B;选择要显示的列。

![](assets/list-view-setting.png)

### 列视图

![](assets/column-view.png)

使用列视图可在内容树中导航一系列级联列。 此视图可帮助您可视化和遍历资产层次结构。

在第一列（最左侧）中选择资源时，会在右侧第二列中显示子资源。 选择第二列中的资源会在右侧的第三列中显示子资源，依此类推。

您可以通过点按或单击资源名称或资源名称右侧的V形标记，在树中上下导航。

* 点按或单击资源名称和V形标记时，将突出显示。
* 点按或单击缩略图会选择资源。
* 选择后，缩略图上会叠加一个复选标记，并突出显示资源名称。
* The details of the selected resource are shown in the final column.

在列视图中选择资产后，该资产的可视化表示形式会与以下详细信息一起显示在最终列中：

* 标题
* 名称
* 尺寸
* 资产从AEM发布到Brand Portal的日期和时间
* 大小
* 类型
* More Details option, to go on the details page of the asset

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

除了这些视图之外，在您查看和选择所需的资产或文件夹时，还可以使用树视图向下展开资产层次结构。

To open the tree view, tap/click the rail selector at upper left and select the **[!UICONTROL Content tree]** from the menu.

![](assets/contenttree.png)

From the content hierarchy, navigate to the desired asset.

![](assets/content-tree.png)

## 资源详细信息 {#asset-details}

资产详细信息页面允许您查看资产、下载资产、共享资产链接、将资产移动到收藏集或查看其属性页面。 It also allows you to navigate through the details page of other assets of the same folder in succession.

![](assets/asset-detail.png)

To view the asset&#39;s metadata, or view its various renditions, use the rail selector on asset detail page.

![](assets/asset-overview.png)

您可以在资产详细信息页面上查看资产的所有可用演绎版，然后选择一个演绎版以进行预览。

![](assets/renditions.png)

要打开资产属性页面，请使用顶部栏中的&#x200B;**[!UICONTROL 属性(p)]**&#x200B;选项。

![](assets/asset-properties.png)

您还可以在资产的属性页面上查看其所有相关资产(AEM上的源资产或派生资产)的列表，因为资产关系也会从AEM发布到Brand Portal。
