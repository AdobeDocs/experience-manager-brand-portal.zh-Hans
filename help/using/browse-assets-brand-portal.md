---
title: 在Brand Portal上浏览资源
seo-title: Browse assets on Brand Portal
description: 使用Brand Portal上的不同视图选项和UI元素，浏览资源、遍历资源层次结构和搜索资源。
seo-description: Browse through assets, traverse asset hierarchies, and search assets, using different view options and UI elements on Brand Portal.
uuid: 178ce217-0050-4922-a204-f4539d46f539
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: introduction
discoiquuid: a70ce694-81d1-4829-9e61-b6412e013e5c
exl-id: 405d7861-a140-44b1-ae1f-4f0839f05033
source-git-commit: a219adc020d63897b10dca83d9ce31fd3ebf847c
workflow-type: tm+mt
source-wordcount: '1018'
ht-degree: 4%

---

# 在Brand Portal上浏览资源 {#browsing-assets-on-brand-portal}

Experience Manager Assets Brand Portal提供了各种功能和用户界面元素，在使用不同的视图选项时，这些功能和元素有助于浏览资源、遍历资源层次结构和搜索资源。

顶部工具栏中的Experience Manager徽标可方便管理员用户访问“管理工具”面板。

![](assets/aemlogo.png)

![](assets/admin-tools-panel-2.png)

![](assets/bp_subheader.png)

Brand Portal左上角的“边栏”选择器下拉菜单可显示用于导航到资产层次结构、简化搜索和显示资源的选项。

![](assets/siderail-1.png)

您可以使用Brand Portal右上角视图选择器中的任何可用视图（卡片、列和列表）来查看、导航和选择资源。

![](assets/viewselector.png)

## 查看和选择资源 {#viewing-and-selecting-resources}

从概念上讲，所有视图中的查看、导航和选择每个视图的方式都相同，但根据您使用的视图，操作方式略有不同。

您可以通过任何可用视图查看、导航和选择资源（以便执行进一步操作）：

* 列视图
* 信息卡视图
* 列表视图

### 信息卡视图

![](assets/card-view.png)

信息卡视图显示各个项目在当前级别的信息信息卡。这些卡片提供以下详细信息：

* 资产/文件夹的可视表示形式。
* 类型
* 标题
* 名称
* 将资源从AEM发布到Brand Portal的日期和时间
* 大小
* 尺寸

您可以通过点按/单击卡片对层次结构进行向下导航（注意避免快速操作），或使用再次向上导航 [标题中的痕迹导航](https://experienceleague.adobe.com/docs/experience-manager-65/authoring/essentials/basic-handling.html).

![](assets/cardquickactions.png)

#### 非管理员用户的卡片视图

文件夹信息卡在信息卡视图中，向非管理员用户（编辑者、查看者和来宾用户）显示文件夹层次结构信息。 此功能可让用户了解他们访问的文件夹相对于父层次结构的位置。
文件夹层次结构信息对于区分名称与从不同文件夹层次结构共享的其他文件夹类似的文件夹特别有用。 如果非管理员用户不知道与他们共享的资产的文件夹结构，则名称类似的资产/文件夹似乎令人困惑。

* 相应卡上显示的路径将被截断以适合卡的大小。 但是，将鼠标悬停在截断的路径上时，用户可以查看完整路径作为工具提示。

![](assets/folder-hierarchy1.png)

**用于查看资产属性的概述选项**

概述选项可供非管理员用户（编辑者、查看者、来宾用户）查看选定资产/文件夹的资产属性。 “概述”选项可见：

* ，位于顶部的工具栏中选择资产/文件夹。
* ，用于选择边栏选择器。

选择 **[!UICONTROL 概述]** 选项选中某个资源/文件夹后，用户可以查看资源创建的标题、路径和时间。 而在资源详细信息页面上，选择概述选项可让用户查看资源的元数据。

![](assets/overview-option.png)

![](assets/overview-rail-selector.png)

#### 在信息卡视图中查看设置

**[!UICONTROL 查看设置]** 对话框在选择时打开 **[!UICONTROL 查看设置]** 从视图选择器中。 它允许您在“信息卡”视图中调整资产缩略图的大小。 这样，您就可以个性化视图，并控制显示的缩略图数量。

![](assets/cardviewsettings.png)

### 列表视图

![](assets/list-view.png)

列表视图显示当前级别上每个资源的信息。 列表视图提供以下详细信息：

* 资产的缩略图图像
* 名称
* 标题
* 区域设置
* 类型
* Dimension
* 大小
* 评分
* 显示资源层次结构的文件夹路径
* 在Brand Portal上发布资源的日期

通过路径列，您可以轻松识别文件夹层次结构中的资源位置。 您可以通过点按/单击资源名称在层次结构中向下导航，然后使用 [标题中的痕迹导航](https://experienceleague.adobe.com/docs/experience-manager-65/authoring/essentials/basic-handling.html).

<!--
Comment Type: draft lastmodifiedby="mgulati" lastmodifieddate="2018-08-17T03:12:05.096-0400" type="annotation">Removed:- "Selecting assets in list view To select all items in the list, use the checkbox at the upper left of the list. When all items in the list are selected, this check box appears checked. To deselect all, click or tap the checkbox. When only some items are selected, it appears with a minus sign. To select all, click or tap the checkbox. To deselect all, click or tap the checkbox again. You can change the order of items using the dotted vertical bar at the far right of each item in the list. Tap/click the vertical selection bar and drag the item to a new position in the list."
 -->

### 在列表视图中查看设置

列表视图显示资源 **[!UICONTROL 名称]** 默认作为第一列。 其他信息，如资产 **[!UICONTROL 标题]**， **[!UICONTROL 区域设置]**， **[!UICONTROL 类型]**， **[!UICONTROL Dimension]**， **[!UICONTROL 大小]**， **[!UICONTROL 评级]**，则也会显示发布状态。 但是，您可以使用以下方式选择要显示的列 **[!UICONTROL 查看设置]**.

![](assets/list-view-setting.png)

### 列视图

![](assets/column-view.png)

使用列视图可在一系列级联列中导航内容树。 此视图可帮助您可视化并遍历资源层次结构。

在第一列（最左侧）中选择资源会在右侧的第二列中显示子资源。 在第二列中选择资源会在右侧的第三列中显示子资源，依此类推。

您可以通过点按或单击资源名称或资源名称右侧的V形标记在树中向上和向下导航。

* 点按或单击时，资源名称和V形高亮显示。
* 点按或单击缩略图将选择资源。
* 选中后，缩略图上将叠加一个复选标记，并突出显示资源名称。
* 所选资源的详细信息将显示在最后一列。

在列视图中选择资产时，资产的可视表示形式连同以下详细信息一起显示在最后一列：

* 标题
* 名称
* 尺寸
* 将资源从AEM发布到Brand Portal的日期和时间
* 大小
* 类型
* “更多详细信息”选项，可转到资产的详细信息页面

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

除了这些视图之外，当您查看和选择所需的资源或文件夹时，还可以使用树视图向下钻取资源层次结构。

要打开树视图，请点按/单击左上方的边栏选择器，然后选择 **[!UICONTROL 内容树]** 从菜单中。

![](assets/contenttree.png)

在内容层次结构中，导航到所需的资源。

![](assets/content-tree.png)

## 资源详细信息 {#asset-details}

资产详细信息页面允许您查看资产、下载、共享资产的链接、将其移动到收藏集或查看其属性页面。 它还允许您连续浏览同一文件夹的其他资产的详细信息页面。

![](assets/asset-detail.png)

要查看资源的元数据或查看其各种演绎版，请使用资源详细信息页面上的边栏选择器。

![](assets/asset-overview.png)

您可以在资源详细信息页面上查看资源的所有可用演绎版，然后从中选择演绎版 **[!UICONTROL 演绎版]** 面板进行预览。

![](assets/renditions.png)

<!-- removed as it is fixed in 2022.02.0 release
>[!CAUTION]
>
>(**Experience Manager Assets as a Cloud Service** only) The following known issues will be fixed in the upcoming release:
>
>The **[!UICONTROL Renditions]** panel does not list all the static renditions of the assets that are published to Brand Portal after December 16, 2021.
>
>The **[!UICONTROL Renditions]** panel lists the smart crop renditions of the asset, however, the user cannot preview or download the smart crop renditions.
-->

要打开资产属性页面，请使用 **[!UICONTROL 属性(p)]** 选项。

![](assets/asset-properties.png)

您还可以在资产的属性页面上查看其所有相关资产(AEM上的源或派生资产)的列表，因为资产关系也会从AEM发布到Brand Portal。
