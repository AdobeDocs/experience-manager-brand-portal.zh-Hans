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
source-git-commit: 3abf39161febc536f431206c2f098e7d61a10846
workflow-type: tm+mt
source-wordcount: '1080'
ht-degree: 4%

---

# 在Brand Portal上浏览资产 {#browsing-assets-on-brand-portal}

Experience Manager Assets Brand Portal提供了各种功能和用户界面元素，有助于在使用不同视图选项时浏览资源、遍历资产层次结构和搜索资产。

Experience Manager顶部工具栏中的徽标有助于管理员用户访问管理工具面板。

![](assets/aemlogo.png)

![](assets/admin-tools-panel-2.png)

![](assets/bp_subheader.png)

Brand Portal左上角的边栏选择器下拉列表，用于显示用于导航到资产层次结构的选项、简化搜索并显示资源。

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

* 资产/文件夹的可视表示形式。
* 类型
* 标题
* 名称
* 资产从AEM发布到Brand Portal的日期和时间
* 大小
* 尺寸

您可以通过点按/单击卡片对层次结构进行向下导航（注意避免快速操作），或使用 [标题中的痕迹导航](https://experienceleague.adobe.com/docs/experience-manager-65/authoring/essentials/basic-handling.html).

![](assets/cardquickactions.png)

#### 非管理员用户的卡片视图

文件夹卡片在卡片视图中向非管理员用户（编辑者、查看者和来宾用户）显示文件夹层次结构信息。 通过此功能，用户可以了解文件夹的位置以及他们正在访问的文件夹相对于父层次结构的位置。
文件夹层次结构信息在区分名称与从其他文件夹层次结构共享的其他文件夹相似的文件夹时特别有用。 如果非管理员用户不知道与他们共享的资产的文件夹结构，则名称相似的资产/文件夹似乎会令人困惑。

* 相应卡片上显示的路径会被截断以适合卡片大小。 但是，用户可以将完整路径视为将鼠标悬停在截断路径上的工具提示。

![](assets/folder-hierarchy1.png)

**查看资产属性的概述选项**

非管理员用户（编辑者、查看者、来宾用户）可以使用概述选项来查看选定资产/文件夹的资产属性。 概述选项可见：

* （位于顶部的工具栏中）。
* 在下拉菜单中，选择边栏选择器。

在选择 **[!UICONTROL 概述]** 选项，用户可以查看资产创建的标题、路径和时间。 然而，在资产详细信息页面上选择概述选项，用户可以查看资产的元数据。

![](assets/overview-option.png)

![](assets/overview-rail-selector.png)

#### 在卡片视图中查看设置

**[!UICONTROL 查看设置]** 对话框在选择 **[!UICONTROL 查看设置]** 从视图选择器中。 它允许您在卡片视图中调整资产缩略图的大小。 这样，您就可以个性化视图并控制显示的缩略图数量。

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
* 显示资产层次结构的文件夹路径
* 在Brand Portal上发布资产的日期

通过“路径”列，您可以轻松地识别文件夹层次结构中的资产位置。 您可以通过点按/单击资源名称，在层次结构中向下导航，然后使用 [标题中的痕迹导航](https://experienceleague.adobe.com/docs/experience-manager-65/authoring/essentials/basic-handling.html).

<!--
Comment Type: draft lastmodifiedby="mgulati" lastmodifieddate="2018-08-17T03:12:05.096-0400" type="annotation">Removed:- "Selecting assets in list view To select all items in the list, use the checkbox at the upper left of the list. When all items in the list are selected, this check box appears checked. To deselect all, click or tap the checkbox. When only some items are selected, it appears with a minus sign. To select all, click or tap the checkbox. To deselect all, click or tap the checkbox again. You can change the order of items using the dotted vertical bar at the far right of each item in the list. Tap/click the vertical selection bar and drag the item to a new position in the list."
 -->

### 在列表视图中查看设置

列表视图显示资产 **[!UICONTROL 名称]** 默认情况下，作为第一列。 其他信息，如资产 **[!UICONTROL 标题]**, **[!UICONTROL 区域设置]**, **[!UICONTROL 类型]**, **[!UICONTROL Dimension]**, **[!UICONTROL 大小]**, **[!UICONTROL 评级]**，则也会显示发布状态。 但是，您可以使用 **[!UICONTROL 查看设置]**.

![](assets/list-view-setting.png)

### 列视图

![](assets/column-view.png)

使用列视图可在内容树中导航一系列级联列。 此视图可帮助您可视化和遍历资产层次结构。

在第一列（最左侧）中选择资源时，会在右侧第二列中显示子资源。 选择第二列中的资源会在右侧的第三列中显示子资源，依此类推。

您可以通过点按或单击资源名称或资源名称右侧的V形标记，在树中上下导航。

* 点按或单击资源名称和V形标记时，将突出显示。
* 点按或单击缩略图会选择资源。
* 选择后，缩略图上会叠加一个复选标记，并突出显示资源名称。
* 最终列中将显示选定资源的详细信息。

在列视图中选择资产后，该资产的可视化表示形式会与以下详细信息一起显示在最终列中：

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

除了这些视图之外，在您查看和选择所需的资产或文件夹时，还可以使用树视图向下展开资产层次结构。

要打开树视图，请点按/单击左上角的边栏选择器，然后选择 **[!UICONTROL 内容树]** 中。

![](assets/contenttree.png)

在内容层次结构中，导航到所需的资产。

![](assets/content-tree.png)

## 资源详细信息 {#asset-details}

资产详细信息页面允许您查看资产、下载资产、共享资产链接、将资产移动到收藏集或查看其属性页面。 它还允许您连续浏览同一文件夹中其他资产的详细信息页面。

![](assets/asset-detail.png)

要查看资产的元数据或查看其各种演绎版，请使用资产详细信息页面上的边栏选择器。

![](assets/asset-overview.png)

您可以在资产详细信息页面上查看资产的所有可用演绎版，然后从 **[!UICONTROL 演绎版]** 面板来预览。

![](assets/renditions.png)

>[!CAUTION]
>
>(**Experience Manager Assetsas a Cloud Service** 仅)在即将发布的版本中将修复以下已知问题：
>
>的 **[!UICONTROL 演绎版]** 面板不会列出2021年12月16日后发布到Brand Portal的所有资产的静态演绎版。
>
>的 **[!UICONTROL 演绎版]** 面板会列出资产的智能裁剪演绎版，但用户无法预览或下载智能裁剪演绎版。

要打开资产属性页面，请使用 **[!UICONTROL 属性(p)]** 选项。

![](assets/asset-properties.png)

您还可以在资产的属性页面上查看其所有相关资产(AEM上的源资产或派生资产)的列表，因为资产关系也会从AEM发布到Brand Portal。
