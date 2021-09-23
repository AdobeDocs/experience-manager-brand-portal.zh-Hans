---
title: 来宾访问 Brand Portal
seo-title: Guest Access to Brand Portal
description: 允许来宾访问，无需身份验证即可载入大量用户。
seo-description: Allow guest access and save the effort to onboard numerous users without authentication.
uuid: edb4378d-1710-44a2-97a6-594d99f62fff
contentOwner: VG
topic-tags: introduction
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: b9e9fe7b-0373-42d1-851b-7c76b47657c2
exl-id: ecce0a45-abae-41c4-9ea7-5dfdcf19e5ea
source-git-commit: e7877973da87362c5fddd6c3aa8135719eff044a
workflow-type: tm+mt
source-wordcount: '998'
ht-degree: 1%

---

# 来宾访问 Brand Portal {#guest-access-to-brand-portal}

Experience ManagerAssets Brand Portal允许来宾访问门户。 来宾用户无需凭据即可进入门户，并且有权访问门户的公共资产（和收藏集）。 来宾会话中的用户可以将资产添加到Lightbox（专用收藏集）并下载相应资产，直到其会话持续存在为止，该会话从会话开始算起，为期2小时，除非来宾用户选择[[!UICONTROL 结束会话]](#exit-guest-session)。

来宾访问功能使组织能够快速地与目标受众大规模共享已批准的资产](../using/brand-portal-sharing-folders.md#how-to-share-folders)，而无需载入这些资产。 [从Brand Portal 6.4.2开始，已经准备好为多个并发来宾用户提供服务，这是每个组织总用户配额的10%。 允许来宾访问可节省时间来管理和在Brand Portal上部署功能有限的用户的分数。\
使用管理工具面板中的&#x200B;**[!UICONTROL 访问]**&#x200B;设置中的&#x200B;**[!UICONTROL 允许来宾访问]**&#x200B;选项，组织可以启用（或禁用）组织Brand Portal帐户上的来宾访问。

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## 开始来宾会话 {#begin-guest-session}

要匿名进入Brand Portal，请选择&#x200B;**[!UICONTROL Click here]**&#x200B;对应于&#x200B;**[!UICONTROL Guest Access?]** 在Brand Portal欢迎屏幕上。输入验证码安全检查以授予使用Brand Portal的访问权限。

![](assets/bp-login-screen.png)

## 来宾会话持续时间 {#guest-session-duration}


来宾用户会话保持活动状态15分钟。
这意味着从会话开始时间开始， **[!UICONTROL Lightbox]**&#x200B;的状态将保留15分钟，并在此之后，当前来宾会话将重新启动，因此Lightbox状态将丢失。

例如，来宾用户于15时00分登录Brand Portal，并将资产添加到&#x200B;**[!UICONTROL Lightbox]**，以便在15:05时下载。 如果用户在15:15小时（在登录后15分钟内）之前未下载&#x200B;**[!UICONTROL Lightbox]**&#x200B;收藏集（或其资产），则用户必须重新启动会话。 **[!UICONTROL Lightbox]**&#x200B;为空，这意味着如果会话丢失，则上传的资产将不再可用。

## 允许的并发来宾会话数 {#concurrent-guest-sessions-allowed}

并发来宾会话数限制为每个组织用户配额总数的10%。 这意味着，对于用户配额为200的组织，最多可以同时使用20个来宾用户。 第21个用户被拒绝访问，并且仅当20个活动来宾用户中任何一个的会话结束时，才能以来宾身份访问。

## 来宾用户与Brand Portal的交互 {#guest-user-interaction-with-brand-portal}

### 来宾UI导航

以来宾身份进入Brand Portal后，用户可以公开或仅与来宾用户共享](../using/brand-portal-sharing-folders.md#sharefolders)的所有[资产和文件夹。 此视图是仅限内容的视图，它以卡片、列表或列布局的形式显示资产。

![](assets/disabled-folder-hierarchy1.png)

但是，如果管理员已启用[启用文件夹层次结构](../using/brand-portal-general-configuration.md#main-pars-header-1621071021)配置，来宾用户在登录Brand Portal时会看到文件夹树（从根文件夹开始）以及在其各自父文件夹内排列的共享文件夹。

这些父文件夹是虚拟文件夹，不能对其执行任何操作。 您可以使用锁定图标识别这些虚拟文件夹。

与共享文件夹不同，在&#x200B;**[!UICONTROL 卡片视图]**&#x200B;中悬停或选择操作任务时，不显示任何操作任务。 **** 在列视图和列表视图中选择虚拟文件 **[!UICONTROL 夹时，]** 会显示 **[!UICONTROL “概述”按钮]**。

>[!NOTE]
>
>虚拟文件夹的默认缩略图是第一个共享文件夹的缩略图。

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

**[!UICONTROL “视]** 图设置”选项允许来宾用户调整“卡片视图”或“列 **[!UICONTROL ”中]** 的卡片大小，以在“列表视 **[!UICONTROL 图”中显示]**。

![](assets/nav-guest-user.png)

**[!UICONTROL 内容树]**&#x200B;允许您在资产层次结构中移动。

![](assets/guest-login-ui.png)

Brand Portal提供了&#x200B;**[!UICONTROL 概述]**&#x200B;选项，以来宾用户查看选定资产/文件夹的&#x200B;**[!UICONTROL 资产属性]**。 **[!UICONTROL Overview]**&#x200B;选项可见：

* 在顶部的工具栏中，选择资产/文件夹。
* 在下拉菜单中，选择边栏选择器。

在选择资产/文件夹时，选择&#x200B;**[!UICONTROL 概述]**&#x200B;选项后，用户可以查看资产创建的标题、路径和时间。 然而，在资产详细信息页面上选择&#x200B;**[!UICONTROL 概述]**&#x200B;选项，则用户可以查看资产的元数据。

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)

**** 左边栏中的导航选项允许从文件导航到收藏集，然后在来宾会话中返回，以便用户可以浏览文件或收藏集中的资产。

**** 过滤器允许来宾用户使用管理员设置的搜索谓词过滤资产文件和文件夹。

### 来宾用户功能

来宾用户可以访问Brand Portal上的公共资产，并且像进一步讨论的那样几乎没有限制。

**来宾用户可以**:

* 访问所有适用于Brand Portal用户的所有公共文件夹和收藏集。
* 浏览成员、详细信息页面，并拥有所有公共文件夹和收藏集成员的完整资产视图。
* 在公共文件夹和收藏集中搜索资产。
* 将资产添加到Lightbox收藏集。 对集合所做的这些更改会在会话期间持续保留。
* 直接或通过Lightbox收藏集下载资产。

**来宾用户不能**:

* 创建收藏集和保存的搜索，或进一步共享它们。
* 访问文件夹和收藏集设置。
* 将资产共享为链接。

### 在来宾会话中下载资产

来宾用户可以直接在Brand Portal上下载公共或专门与来宾用户共享的资产。 来宾用户还可以将资产添加到&#x200B;**[!UICONTROL Lightbox]**（公共收藏集），并在其会话过期之前下载&#x200B;**[!UICONTROL Lightbox]**&#x200B;收藏集。

要下载资产和收藏集，请使用下面的下载图标：

* 快速操作缩略图，将鼠标悬停在资产或收藏集上时显示
* 顶部的工具栏，用于选择资产或收藏集

![](assets/download-on-guest.png)

选择&#x200B;**[!UICONTROL 在[!UICONTROL 下载]对话框中启用下载加速]**&#x200B;可让您[提高下载性能](../using/accelerated-download.md)。

## 退出来宾会话 {#exit-guest-session}

要退出来宾会话，请从标头中可用的选项中使用&#x200B;**[!UICONTROL 结束会话]**。 但是，如果用于来宾会话的浏览器选项卡不活动，则该会话在处于不活动状态两小时后自动过期。

![](assets/end-guest-session.png)

## 监控来宾用户活动 {#monitoring-guest-user-activities}

管理员可以监控来宾用户与Brand Portal的交互。 在Brand Portal中生成的报表可以对来宾用户活动提供关键分析。 例如，**[!UICONTROL Download]**&#x200B;报表可用于跟踪来宾用户下载的资产计数。 **[!UICONTROL 用户]** 登录报表可以通知来宾用户上次登录门户的时间以及指定时间段内的登录频率。
