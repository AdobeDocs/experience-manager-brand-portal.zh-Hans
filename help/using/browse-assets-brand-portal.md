---
title: 在Brand Portal上浏览资源
description: 使用Brand Portal上的其他查看选项和UI元素来浏览资源、遍历资源层次结构和搜索资源。
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: introduction
exl-id: 405d7861-a140-44b1-ae1f-4f0839f05033
source-git-commit: ff51a49a958d43c98443d816a92276faae5e9569
workflow-type: tm+mt
source-wordcount: '1015'
ht-degree: 7%

---

# 在Brand Portal上浏览资源 {#browsing-assets-on-brand-portal}

Experience Manager Assets Brand Portal提供了各种功能和用户界面元素，以便使用不同的视图选项轻松浏览资源、导航资源层次结构和搜索资源。

顶部的工具栏中的Experience Manager徽标可方便管理员用户访问管理工具面板。

![](assets/aemlogo.png)

![](assets/admin-tools-panel-2.png)

![](assets/bp_subheader.png)

Brand Portal左上角的边栏选择器下拉菜单显示了用于导航到资源层次结构、简化搜索和显示资源的选项。

![](assets/siderail-1.png)

您可以使用Brand Portal的视图选择器中的任何可用视图（卡片、列和列表）来查看、导航和选择资源。

![](assets/viewselector.png)

## 查看和选择资源 {#viewing-and-selecting-resources}

从概念上讲，所有视图中的查看、导航和选择每个视图的方式都相同，只是操作方法根据您使用的视图而略有差异。

您可以在任何可用视图中查看、导航和选择资源（以便执行进一步操作）：

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

您可以通过单击卡片在层次结构中向下导航（注意避免快速操作），或使用标题](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/sites/authoring/essentials/basic-handling)中的[痕迹导航再次向上导航。

![](assets/cardquickactions.png)

#### 非管理员用户的卡片视图

文件夹信息卡在信息卡视图中，向非管理员用户（编辑者、查看者和访客用户）显示文件夹层次结构信息。 此功能使用户知道他们访问的文件夹相对于父层次结构的位置。

文件夹层次结构信息对于区分名称与从不同文件夹层次结构共享的其他文件夹类似的文件夹特别有用。 如果非管理员用户不知道与其共享的资产所属的文件夹结构，则名称类似的资产/文件夹会显得混乱。

* 相应卡上显示的路径将被截断以适合卡的大小。 但是，通过将鼠标悬停在截断的路径上，用户可以查看完整路径作为工具提示。

![](assets/folder-hierarchy1.png)

**用于查看资源属性的概述选项**

概述选项可供非管理员用户（编辑者、查看者、来宾用户）查看选定资产/文件夹的资产属性。 “概述”选项可见：

* 在顶部的工具栏中，选择资产/文件夹时。
* 在下拉列表的边栏选择器中。

在选择资产/文件夹的同时选择&#x200B;**[!UICONTROL 概述]**&#x200B;选项时，用户可以查看资产创建的标题、路径和时间。 而在资源详细信息页面上，选择概述选项可让用户查看资源的元数据。

![](assets/overview-option.png)

![](assets/overview-rail-selector.png)

#### 在信息卡视图中查看设置

通过从视图选择器中选择&#x200B;**[!UICONTROL 视图设置]**，将打开&#x200B;**[!UICONTROL 视图设置]**&#x200B;对话框。 它允许您在卡片视图中调整资源缩略图的大小。 这样，您就可以个性化视图，并控制显示的缩略图数量。

![](assets/cardviewsettings.png)

### 列表视图

![](assets/list-view.png)

列表视图显示每个资源在当前级别的信息。 “列表”视图提供以下详细信息：

* 资产的缩略图图像
* 名称
* 标题
* 区域设置
* 类型
* 维度
* 大小
* 评分
* 显示资源层次结构的文件夹路径
* 在Brand Portal上发布资源的日期

通过路径列，您可以轻松识别文件夹层次结构中的资源位置。 您可以通过单击资源名称向下导航到层次结构，并使用标题](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/sites/authoring/essentials/basic-handling)中的[痕迹导航再次导航。

<!--
Comment Type: draft lastmodifiedby="mgulati" lastmodifieddate="2018-08-17T03:12:05.096-0400" type="annotation">Removed:- "Selecting assets in list view To select all items in the list, use the checkbox at the upper left of the list. When all items in the list are selected, this check box appears checked. To deselect all, click or tap the checkbox. When only some items are selected, it appears with a minus sign. To select all, click or tap the checkbox. To deselect all, click or tap the checkbox again. You can change the order of items using the dotted vertical bar at the far right of each item in the list. Click the vertical selection bar and drag the item to a new position in the list."
 -->

### 在列表视图中查看设置

默认情况下，“列表”视图将资源&#x200B;**[!UICONTROL Name]**&#x200B;显示为第一列。 此外，还会显示其他信息，例如资源&#x200B;**[!UICONTROL 标题]**、**[!UICONTROL 区域设置]**、**[!UICONTROL 类型]**、**[!UICONTROL Dimension]**、**[!UICONTROL 大小]**、**[!UICONTROL 评级]**、发布状态。 但是，您可以使用&#x200B;**[!UICONTROL 视图设置]**&#x200B;选择要显示的列。

![](assets/list-view-setting.png)

### 列视图

![](assets/column-view.png)

使用列视图可在一系列级联列中导航内容树。 此视图可帮助您可视化并遍历资源层次结构。

在第一列（最左侧）中选择资源会在右侧的第二列中显示子资源。 在第二列中选择资源会在右侧的第三列中显示子资源，依此类推。

您可以在树中向上和向下导航。 单击资源名称或资源名称右侧的V形。

* 资源名称和 V 形标记在被点按或单击时会突出显示。
* 点按或单击缩略图将选择资源。
* 选中后，缩略图上将叠加一个复选标记，并且资源名称会高亮显示。
* 最后的列中会显示选定资源的详细信息。

在列视图中选择资产时，资产的可视表示形式连同以下详细信息一起显示在最后一列：

* 标题
* 名称
* 尺寸
* 将资源从AEM发布到Brand Portal的日期和时间
* 大小
* 类型
* 与资源的详细信息页面一起使用的“更多详细信息”选项

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

要打开树视图，请单击左上角的边栏选择器，然后从菜单中选择&#x200B;**[!UICONTROL 内容树]**。

![](assets/contenttree.png)

在内容层次结构中，导航到所需的资源。

![](assets/content-tree.png)

## 资源详情 {#asset-details}

使用资源详细信息页面，可以查看资源、下载、共享资源的链接、将资源移动到收藏集或查看其属性页面。 它还允许您连续导航同一文件夹的其他资产的详细信息页面。

![](assets/asset-detail.png)

要查看资源的元数据或查看其各种演绎版，请使用资源详细信息页面上的边栏选择器。

![](assets/asset-overview.png)

您可以在资源详细信息页面上查看资源的所有可用演绎版，并从&#x200B;**[!UICONTROL 演绎版]**&#x200B;面板中选择演绎版以进行预览。

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

要打开资产属性页面，请使用顶部栏中的&#x200B;**[!UICONTROL 属性(p)]**&#x200B;选项。

![](assets/asset-properties.png)

您还可以在资产的属性页面上查看其所有相关资产(AEM上的源或派生资产)的列表，因为资产关系也会从AEM发布到Brand Portal。
