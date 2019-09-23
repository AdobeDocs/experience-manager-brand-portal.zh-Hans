---
title: 在Brand Portal上浏览资产
seo-title: 在Brand Portal上浏览资产
description: 使用Brand Portal上的不同视图选项和UI元素浏览资产、遍历资产层次结构和搜索资产。
seo-description: 使用Brand Portal上的不同视图选项和UI元素浏览资产、遍历资产层次结构和搜索资产。
uuid: 178ce217-0050-4922-a204-f4539d46f539
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: 引用
topic-tags: introduction
discoiquuid: a70ce694-81d1-4829-9e61-b6412e013e5c
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# 在Brand Portal上浏览资产 {#browsing-assets-on-brand-portal}

AEM Assets Brand Portal提供了各种功能和用户界面元素，便于在使用不同视图选项时浏览资源、遍历资产层次结构和搜索资产。

顶部AEM工具栏中的AEM徽标方便了管理员用户访问管理工具面板。

![](assets/aemlogo.png)

![](assets/admin-tools-panel-2.png)

![](assets/bp_subheader.png)

Brand Portal左上角的边栏选择器下拉，以显示可导航到资产层次结构、简化搜索和显示资源的选项。

![](assets/siderail-1.png)

您可以使用品牌门户右上角的视图选择器中的任意可用视图（卡片、列和列表）查看、导航和选择资产。

![](assets/viewselector.png)

## 查看和选择资源 {#viewing-and-selecting-resources}

从概念上讲，所有视图中的查看、导航和选择操作都相同，但操作方式根据所使用的视图而略有不同。

您可以使用以下任一可用视图查看、导航和选择资源（以对其执行进一步操作）:

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
* 从AEM将资产发布到Brand Portal的日期和时间
* 大小
* 尺寸

You can navigate down the hierarchy by tapping/clicking cards (taking care to avoid the quick actions) or up again by using the [breadcrumbs in the header](https://helpx.adobe.com/experience-manager/6-5/sites/authoring/using/basic-handling.html#TheHeader).

![](assets/cardquickactions.png)

#### 非管理员用户的卡片视图

文件夹的卡片在卡片视图中向非管理员用户（编辑者、查看者和客人用户）显示文件夹层次结构信息。 此功能可让用户了解文件夹的位置，以及他们访问的与父层次结构相关的文件夹。
文件夹层次结构信息对于区分名称与从不同文件夹层次结构共享的其他文件夹相似的文件夹特别有用。 如果非管理员用户不知道与他们共享的资产的文件夹结构，则名称相似的资产／文件夹似乎会令人混淆。

* 相应卡上显示的路径会被截断以适合卡的大小。 但是，用户在将鼠标悬停在被截断的路径上时，可以将完整路径看作工具提示。

![](assets/folder-hierarchy1.png)

**查看资产属性的概述选项**

“概述”选项对非管理员用户（编辑者、查看者、客人用户）可用，用于查看选定资产／文件夹的资产属性。 “概述”选项可见：

* 在顶部的工具栏中选择资产／文件夹。
* 在下拉框中，选择边栏选择器。

在选择资 [!UICONTROL 产] /文件夹时选择“概述”选项后，用户可以查看资产创建的标题、路径和时间。 但是，在资产详细信息页面上，选择“概述”选项可让用户查看资产的元数据。

![](assets/overview-option.png)

![](assets/overview-rail-selector.png)

#### 在卡片视图中查看设置

[!UICONTROL 在从视图选择器中选择] “查看设置”时， **[!UICONTROL 将打开“查看设置]** ”对话框。 它允许您在卡片视图中调整资产缩略图的大小。 This way, you can personalize your view and control the number of thumbnails that is displayed.

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

*路径列可让您轻松识别文件夹层次结构中的资产位置。 You can navigate down the hierarchy by tapping/clicking the resource name, and back up by using the [breadcrumbs in the header](https://helpx.adobe.com/experience-manager/6-5/sites/authoring/using/basic-handling.html#TheHeader).

<!--
Comment Type: draft lastmodifiedby="mgulati" lastmodifieddate="2018-08-17T03:12:05.096-0400" type="annotation">Removed:- "Selecting assets in list view To select all items in the list, use the checkbox at the upper left of the list. When all items in the list are selected, this check box appears checked. To deselect all, click or tap the checkbox. When only some items are selected, it appears with a minus sign. To select all, click or tap the checkbox. To deselect all, click or tap the checkbox again. You can change the order of items using the dotted vertical bar at the far right of each item in the list. Tap/click the vertical selection bar and drag the item to a new position in the list."
 -->

### 在列表视图中查看设置

“列表”视图默 [!UICONTROL 认将资产] “名称”显示为第一列。 此外，还会显示资产 [!UICONTROL Asset]、 [!UICONTROL Locale]、 [!UICONTROL DimensionsTitle]、 DimensionsSize、Type Status、Publish状态等其他信息。 However, you can select the columns to be shown using [!UICONTROL View Settings].

![](assets/list-view-setting.png)

### 列视图

![](assets/column-view.png)

使用列视图可在内容树中浏览一系列级联列。 此视图可帮助您可视化和遍历资产层次结构。

在第一列（最左侧）中选择资源后，将在右侧第二列中显示子资源。 选择第二列中的资源后，右侧第三列中将显示子资源，依此类推。

通过点按或单击资源名称或资源名称右侧的V形标记，可以在树中上下导航。

* 点按或单击资源名称和V形标记时将高亮显示。
* Tapping or clicking the thumbnail selects the resource.
* 选中后，缩略图上会叠加一个复选标记，并高亮显示资源名称。
* The details of the selected resource are shown in the final column.

在列视图中选择资产后，资产的可视表示形式将显示在最后一列，并显示以下详细信息：

* 标题
* 名称
* 尺寸
* 从AEM将资产发布到Brand Portal的日期和时间
* 大小
* 类型
* “更多详细信息”选项，转到资产的详细信息页面

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

<h4>Deselecting All</h4>
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

除了这些视图之外，在查看和选择所需的资产或文件夹时，还可以使用树视图向下展开资产层次结构。

要打开树视图，请点按／单击左上角的边栏选择器，然后从菜单中选 **[!UICONTROL 择内容树]** 。

![](assets/contenttree.png)

从内容层次结构中，导航到所需的资产。

![](assets/content-tree.png)

## 资源详细信息 {#asset-details}

通过资产详细信息页面，您可以查看资产、下载、共享资产的链接、将资产移至集合或查看其属性页面。 它还允许您连续浏览同一文件夹中其他资产的详细信息页面。

![](assets/asset-detail.png)

要查看资产的元数据或查看其各种演绎版，请使用资产详细信息页面上的边栏选择器。

![](assets/asset-overview.png)

您可以在资产详细信息页面上查看该资产的所有可用演绎版，然后选择一个演绎版进行预览。

![](assets/renditions.png)

要打开资产属性页面，请使 **[!UICONTROL 用顶栏中的属性(p)]** 选项。

![](assets/asset-properties.png)

您还可以在资产的属性页面上查看其所有相关资产（AEM上的源资产或派生资产）的列表，因为资产关系也会从AEM发布到Brand Portal。
