---
title: 来宾访问Brand Portal
description: 允许来宾访问，无需身份验证即可轻松载入大量用户。
contentOwner: VG
topic-tags: introduction
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
exl-id: ecce0a45-abae-41c4-9ea7-5dfdcf19e5ea
source-git-commit: 4c701781e7dc62b9d2b018fd13b1ae9616bbb840
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 0%

---

# 来宾访问Brand Portal {#guest-access-to-brand-portal}

Experience Manager Assets Brand Portal允许Guest访问门户。 来宾用户无需凭据即可进入门户，并且有权访问门户的公共资产（和收藏集）。 来宾会话中的用户可以向Lightbox（专用收藏集）添加资产并下载这些资产，直到其会话持续或来宾用户选择[[!UICONTROL 结束会话]](#exit-guest-session)为止。 访客用户会话保持活动状态15分钟。

来宾访问功能使组织能够快速[与预期受众共享](../using/brand-portal-sharing-folders.md#how-to-share-folders)已批准的资产，而无需加入这些受众。 从Brand Portal 6.4.2开始，已配备多个并发访客用户，这相当于每个组织总用户配额的10%。 允许来宾访问可节省在Brand Portal上管理和板载功能有限的用户所需的时间。\
组织可以使用“管理工具”面板中&#x200B;**[!UICONTROL 访问]**&#x200B;设置的&#x200B;**[!UICONTROL 允许来宾访问]**&#x200B;选项，启用（或禁用）对该组织的Brand Portal帐户的来宾访问。

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## 开始来宾会话 {#begin-guest-session}

要匿名进入Brand Portal，请在Brand Portal的欢迎屏幕上选择与&#x200B;**[!UICONTROL `Guest Access?`]**&#x200B;对应的&#x200B;**[!UICONTROL 单击此处]**。 输入captcha安全检查以授予使用Brand Portal的权限。

![](assets/bp-login-screen.png)

## 来宾会话持续时间 {#guest-session-duration}

访客用户会话保持活动状态15分钟。
此过程将**[!UICONTROL Lightbox]**&#x200B;的状态从会话开始时间保留15分钟。 之后，当前来宾会话重新启动，导致Lightbox状态丢失。

例如，访客用户在1500小时登录到Brand Portal，并在15:05小时将资源添加到&#x200B;**[!UICONTROL Lightbox]**&#x200B;以供下载。 如果用户未在15:15小时（登录后15分钟内）之前下载&#x200B;**[!UICONTROL Lightbox]**&#x200B;收藏集（或其资产），则用户必须重新启动会话。 **[!UICONTROL Lightbox]**&#x200B;为空，这意味着如果会话丢失，则上传的资源不再可用。

## 允许的并发来宾会话 {#concurrent-guest-sessions-allowed}

每个组织的并发来宾会话数限制为总用户配额的10%。 这意味着对于用户配额为200的组织，最多可同时工作20个访客用户。 第21位用户被拒绝访问，只有在20位活动来宾用户的会话结束时，才可以来宾身份访问。

>[!NOTE]
>
>如果获得许可的用户数量超过合同约定的值（配额），Brand Portal将不会发送通知。 此外，它不会限制许可用户的任何活动。

## 来宾用户与Brand Portal的交互 {#guest-user-interaction-with-brand-portal}

### 来宾UI导航

以访客身份进入Brand Portal时，用户可以查看公开或与访客用户独占共享的所有[资源和文件夹](../using/brand-portal-sharing-folders.md#sharefolders)。 此视图是“仅内容”视图，该视图以卡片、列表或列布局显示资产。

![](assets/disabled-folder-hierarchy1.png)


如果管理员启用[启用文件夹层次结构](../using/brand-portal-general-configuration.md#main-pars-header-1621071021)，则来宾用户在登录到Brand Portal后，会从父文件夹中的根文件夹和共享文件夹看到文件夹树。

这些父文件夹是虚拟文件夹，无法对它们执行任何操作。 您可以使用锁图标来识别这些虚拟文件夹。

与共享文件夹不同，在&#x200B;**[!UICONTROL 卡片视图]**&#x200B;中悬停或选择操作任务时不会显示任何操作任务。 在&#x200B;**[!UICONTROL 列视图]**&#x200B;和&#x200B;**[!UICONTROL 列表视图]**&#x200B;中选择虚拟文件夹时显示&#x200B;**[!UICONTROL 概述]**&#x200B;按钮。

>[!NOTE]
>
>虚拟文件夹的默认缩略图是第一个共享文件夹的缩略图图像。

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

**[!UICONTROL 视图设置]**&#x200B;选项允许来宾用户在&#x200B;**[!UICONTROL 卡片视图]**&#x200B;中调整卡片大小，或者在&#x200B;**[!UICONTROL 列表视图]**&#x200B;中调整要显示的列大小。

![](assets/nav-guest-user.png)

**[!UICONTROL 内容树]**&#x200B;允许您在资源层次结构中移动。

![](assets/guest-login-ui.png)

Brand Portal为来宾用户提供了&#x200B;**[!UICONTROL 概述]**&#x200B;选项以查看选定资源/文件夹的&#x200B;**[!UICONTROL 资源属性]**。 **[!UICONTROL 概述]**&#x200B;选项可见：

* 在顶部的工具栏中，选择资源或文件夹时。
* 在下拉列表中选择边栏选择器。

如果选择了&#x200B;**[!UICONTROL 概述]**&#x200B;选项（在选择某个资源或文件夹时），用户可以查看资源创建的标题、路径和时间。 而在资源详细信息页面上，选择&#x200B;**[!UICONTROL 概述]**&#x200B;选项可让用户查看资源的元数据。

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)

左侧边栏中的&#x200B;**[!UICONTROL 导航]**&#x200B;选项允许从文件导航到收藏集，并在来宾会话中返回，以便用户可以浏览文件或收藏集中的资产。

通过&#x200B;**[!UICONTROL 筛选器]**&#x200B;选项，来宾用户可以使用管理员设置的搜索谓词筛选资源文件和文件夹。

### 来宾用户功能

访客用户可以访问Brand Portal上的公共资源，并且几乎没有限制，具体如下所述。

**来宾用户可以**：

* 访问适用于所有Brand Portal用户的所有公共文件夹和收藏集。
* 浏览成员、详细信息页面，并拥有所有公共文件夹和收藏集成员的完整资产视图。
* 在公共文件夹和收藏集中搜索资产。
* 将资产添加到Lightbox收藏集。 对收藏集的这些更改将在会话期间保留。
* 直接或通过Lightbox收藏集下载资产。

**来宾用户不能**：

* 创建收藏集和保存的搜索，或进一步共享它们。
* 访问文件夹和收藏集设置。
* 将资源作为链接共享。

### 在来宾会话中下载资产

访客用户可以直接下载在Brand Portal上公开或专门与访客用户共享的资源。 来宾用户还可以在会话过期之前将资产添加到&#x200B;**[!UICONTROL Lightbox]**（公共收藏集），并下载&#x200B;**[!UICONTROL Lightbox]**&#x200B;收藏集。

要下载资产和收藏集，请使用以下位置的下载图标：

* 快速操作缩略图，当鼠标悬停在资产或收藏集上时显示
* 顶部的工具栏，在选择资产或收藏集时显示

![](assets/download-on-guest.png)

在[!UICONTROL 下载]对话框中选择&#x200B;**[!UICONTROL 启用下载加速]**&#x200B;可让您[增强下载性能](../using/accelerated-download.md)。

## 退出来宾会话 {#exit-guest-session}

若要退出来宾会话，请使用标头中可用选项中的&#x200B;**[!UICONTROL 结束会话]**。 但是，如果用于来宾会话的浏览器选项卡处于非活动状态，则会话将在处于非活动状态两小时后自动过期。

![](assets/end-guest-session.png)

## 监视来宾用户活动 {#monitoring-guest-user-activities}

管理员可以监测访客用户与Brand Portal的交互。 在Brand Portal中生成的报表可提供有关访客用户活动的关键见解。 例如，**[!UICONTROL Download]**&#x200B;报表可用于跟踪来宾用户下载的资源计数。 **[!UICONTROL 用户登录]**&#x200B;报告可以通知访客用户上次登录门户的时间以及指定持续时间内登录的频率。
