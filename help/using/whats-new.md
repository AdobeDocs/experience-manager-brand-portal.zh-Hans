---
title: What's new in AEM Assets Brand Portal
seo-title: AEM Assets Brand Portal的新增功能
description: 了解6.4.5的新增功能和增强功能。
seo-description: 了解6.4.5的新增功能和增强功能。
uuid: 2c59d738-9b53-4f25-a205-13bf75c80b77
contentOwner: bdhar
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: 引用
topic-tags: introduction
discoiquuid: fec32ca3-142b-4a11-9b92-5113fc27277a
translation-type: tm+mt
source-git-commit: f5318420b4598ece27d8dfac4f4e7e0c5a02753d

---


# AEM Assets Brand Portal的新增功能 {#what-s-new-in-aem-assets-brand-portal}

Adobe Experience Manager (AEM) Assets Brand Portal helps you easily acquire, control, and securely distribute approved creative assets to external parties and internal business users across devices. It helps improve the efficiency of asset sharing, accelerates the time-to-market for assets, and reduces the risk of non-compliance and unauthorized access. Adobe is working to improve the overall Brand Portal experience. 抢先领略新增功能和增强功能。

## 6.4.5中的更改 {#what-changed-in-645}

Brand Portal 6.4.5是一个功能版本，它侧重于为Brand Portal用户（外部代理／团队）提供将内容上传到Brand Portal并发布到AEM资产的能力，而无需访问创作环境。 This feature is called **Asset Sourcing in Brand Portal**, and will improve customer experiences by providing a two-way mechanism for users to both contribute and share assets with other globally distributed Brand Portal users.

### Brand Portal中的资产来源补充 {#asset-sourcing-in-bp}

资产来源补充允许AEM管理员使用其他“资产贡献 **** ”属性创建新文件夹，从而确保创建的新文件夹可由Brand Portal用户打开以提交资产。 这会自动触发一个工作流，该工作流会在新创建的 **Contribution** 文件夹内创建另外两个子文件夹，称为NEW和SHARED。

然后，AEM管理员将应添加到贡献文件夹的资产类型以及一组基准资产的简介上传到 **SHARED** 文件夹，以确保BP用户拥有他们需要的参考信息，从而定义了要求。 然后，管理员可以在将新创建的Contribution文件夹发布到Brand Portal之前，向活动的Brand Portal用户授予对贡献文件 **夹的访问权** 。

用户完成在 **NEW** 文件夹中添加内容后，他们可以将贡献文件夹发布回AEM创作环境。 请注意，完成导入并反映AEM资产中新发布的内容可能需要几分钟时间。

此外，所有现有功能都保持不变。 Brand Portal用户可以从贡献文件夹以及其他允许的文件夹查看、搜索和下载资产。 管理员还可以进一步共享贡献文件夹、修改属性以及向集合添加资产。 请参阅最 [新的Brand Portal发行说明](brand-portal-release-notes.md)。

>[!NOTE]
>
>Brand Portal用户只能将内容／资产上传到 **NEW** 文件夹。

>[!NOTE]
>
>任何Brand Portal帐户／租户的最大上传限 **制为** 10 GB。



![](assets/asset-sourcing.png)

### 在Brand Portal中上传资产 {#upload-assets-in-bp}

Brand Portal用户在共享贡献文件夹时会自动收到脉冲／电子邮件通知，允许他们从 **SHARED** 文件夹下载简要文档和下载基准内容，以确保他们了解项目要求。

具有相应权限的Brand Portal用户可以将包含多个资产的多个资产或文件夹上传到贡献文件夹。 但是，请注意，Brand Portal用户只能将资产上传到 **NEW** 子文件夹。 The **SHARED** folder is meant for the distribution of project details and baseline assets.

![](assets/upload-asset6.png)

![](assets/upload-asset4.png)

>[!NOTE]
>
>Brand Portal users do not have permission to delete an uploaded asset.

### Publish contribution folder to AEM Assets {#publish-assets-to-aem}

Once upload is complete to the NEW folder, Brand Portal users can then publish the contribution folder back to AEM. **** It may take few minutes to import and reflect the published content/assets in AEM Assets.

The Brand Portal user and the AEM Administrator will receive pulse/email notifications both at the beginning and at the completion of the publish action, along with the job progress status (Queued/In-Progress/Success). AEM and Brand Portal administrators can also view the job status from their respective interfaces.

![](assets/upload-asset5.png)

## What changed in 6.4.4 {#what-changed-in-644}

Brand Portal 6.4.4 release focuses on enhancements to text search and top customer requests. See latest Brand Portal Release Notes.[](brand-portal-release-notes.md)

### Search enhancements {#search-enhancements}

从Brand Portal 6.4.4开始，支持对筛选窗格中的属性谓词进行部分文本搜索。 要允许部分文本搜索，您需要在搜索表单中 **的属性谓词中启用** “部分搜索”。

Read on to know more about partial text search and wildcard search.

#### 部分短语搜索 {#partial-phrase-search}

您现在可以通过在筛选窗格中仅指定搜索短语的一个或两个部分来搜索资产。

**用例部**&#x200B;分短语搜索在您不确定搜索的短语中出现的词语的确切组合时很有帮助。

例如，如果您在Brand Portal中的搜索表单使用属性谓词对资产标题进行部分搜索，则指定术语 **camp** 将返回标题短语中带有单词camp的所有资产。

![](assets/partialphrasesearch.png)

#### 通配符搜索 {#wildcard-search}

Brand Portal允许在搜索查询中使用星号(*)，并在搜索短语中使用部分单词。

**用例**&#x200B;如果您不确定搜索短语中出现的确切单词，可以使用通配符搜索来填补搜索查询中的空白。

For example, specifying climb* returns all the assets having words beginning with the characters climb in their title phrase if search form in Brand Portal uses Property Predicate for partial search on assets title.********

![](assets/wildcard-prop.png)

Similarly, specifying:

* ***climp** 返回所有单词以字符 **clamp** 结尾的资产。

* ***climb*** 返回所有包含词的资源，这些词的标题词 **中包含** “clipt”字符。

>[!NOTE]
>
>在选中“部 **分搜索** ”复选框时， **默认情况下会选中“忽略大小写** ”。

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-searching.md#facetedsearchbyapplyingfilterstosearch)

## 6.4.3中的更改 {#what-changed-in}

Brand Portal 6.4.3 release focuses on — providing organizations with an alternate alias in addition to their tenant ID in Brand Portal access URL, new folder hierarchy configuration, video support enhancements, scheduled publishing from AEM Author instance to Brand Portal, operational enhancements — and cateres to customer requests.

### 非管理员的文件夹层次结构导航

管理员现在可以配置文件夹在登录时向非管理员用户（编辑者、查看者和客人用户）显示的方式。 [“启用文件夹层次结构](../using/brand-portal-general-configuration.md) ”配置将添加在“ **常规设置**”中，位于管理工具面板中。 如果配置为：

* **启用**&#x200B;后，从根文件夹开始的文件夹树对非管理员用户可见。 因此，可授予他们类似于管理员的导航体验。
* **禁用**，登录页面上仅显示共享文件夹。

![](assets/enable-folder-hierarchy.png)
用**例**

启用 [文件夹层次结构功能](../using/brand-portal-general-configuration.md) （启用后）可帮助您区分名称与从不同层次结构共享的文件夹。 登录后，非管理员用户现在可以看到共享文件夹的虚拟父（和上级）文件夹。
![](assets/disabled-folder-hierarchy1-2.png) ![](assets/enabled-hierarchy1-2.png)

共享文件夹在虚拟文件夹的各个目录中进行组织。 您可以通过锁定图标识别这些虚拟文件夹。

请注意，虚拟文件夹的默认缩略图是第一个共享文件夹的缩略图。

![](assets/hierarchy1-nonadmin-2.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-general-configuration.md)

### 在特定文件夹层次结构或路径中搜索

**路径浏览器谓词** (Path Browser predicate is in the Search Form)在搜索表单中引入，以允许搜索特定目录中的资产。 路径浏览器的搜索谓词的默认搜索路径为 */content/dam/mac/&lt;tenant-id&gt;/*，可通过编辑默认搜索表单来配置该路径。

* 管理员用户可以使用路径浏览器导航到Brand Portal上的任意文件夹目录。
* Non-admin users can use Path Browser to navigate only to the folders (and navigate back to the parent folders) shared with them.
For example, /content/dam/mac/&lt;tenant-id&gt;/folderA/folderB/folderC is shared with a non-admin user. ** The user can search for assets within folderC using Path Browser. This user can also navigate to folderB and folderA (since they are ancestors of the folderC that is shared with the user).

![](assets/edit-search-form.png)

**The use case**

You can now restrict asset search within a specific folder you have browsed to, instead of beginning at the root folder.

Note that searching under these folders returns results only from the assets that have been shared with the user.

![](assets/filter-panel.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-search-facets.md#listofsearchpredicates)

### Dynamic Media video renditions support

AEM作者实例处于Dynamic media混合模式的用户除了可以预览和下载原始视频文件外，还可以预览和下载Dynamic media再现。

To allow preview and download of dynamic media renditions on specific tenant accounts, administrators need to specify Dynamic Media Configuration (video service URL (DM-Gateway URL) and registration ID to fetch the dynamic video) in Video configuration from admin tools panel.********

**The use case
Dynamic Media videos can be previewed on:**

* 资产详细信息页面
* 资产的卡片视图
* Link share preview page

Dynamic Media视频编码可从以下位置下载：

* 品牌门户
* Shared link

![](assets/edit-dynamic-media-config.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### 计划发布到Brand Portal

可以将资产（和文件夹）从 [AEM(6.4.2.0)](https://helpx.adobe.com/experience-manager/6-4/release-notes/sp-release-notes.html#main-pars_header_9658011) “作者”实例发布到Brand Portal的工作流安排在以后的日期、时间内。

同样，通过计划从Brand Portal中取消发布工作流，可以在以后的日期（时间）从门户中删除已发布的资产。

![](assets/schedule-publish.png)
![](assets/publishlater-workflow.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### URL中可配置的租户别名

Organizations can get their portal URL customized, by having an alternate prefix in the URL. 要在其现有门户URL中获取租户名称的别名，组织需要联系Adobe支持部门。

请注意，只能自定义品牌门户URL的前缀，而不能自定义整个URL。\
例如，具有现有域 **geometrix.brand-portal.adobe.com的组织可以获取** geometrixinc.brand-portal.adobe.com **** （根据请求创建）。

但是，AEM作者实例只能 [使用租户](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html) ID URL配置，而不能使用租户别名（备用）URL配置。

**用例组**&#x200B;织可以通过自定义门户URL而不是坚持Adobe提供的URL来满足其品牌需求。

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### 下载体验增强功能

该版本通过减少点击次数和警告次数提供简化的下载体验，具体内容如下：

* 选择仅下载演绎版（而非原始资产）。
* 当访问原始演绎版受限时，下载资产。

## 6.4.2中的更改 {#what-changed-in-1}

Brand Portal 6.4.2版本提供了一系列功能，可满足组织的资产分发需求，并帮助他们接触到通过客人访问和最佳下载体验在全球分布的大量用户。 Brand Portal还通过管理员的新配置、新添加的报告以及迎合客户请求为组织提供更大的控制。

### 客人访问

![](assets/bp-login-screen-1.png)

AEM Brand门户允许客人访问门户。 客人用户不需要凭据即可进入门户，并且可以访问和下载所有公共文件夹和集合。 客人用户可以将资产添加到其Lightbox（私人收藏集）并下载相同的资产。 他们还可以查看管理员设置的智能标记搜索和搜索谓词。 客人会话不允许用户创建集合和保存的搜索或进一步共享它们、访问文件夹和集合设置以及将资产共享为链接。

在组织中，允许多个并发客人会话，此会话限制为每个组织的用户配额总数的10%。

客人会话在两小时内保持活动状态。 因此，灯箱的状态也会保留到会话开始时间后的两小时。 两小时后，客人会话必须重新启动，因此lightbox状态会丢失。

### 加速下载

Brand Portal用户可以利用基于IBM Aspera connect的快速下载，将下载速度提高25倍，并享受无缝下载体验，无论他们位于全球哪个位置。 To download the assets faster from Brand Portal or the shared link, users need to select Enable Download Acceleration option in download dialog, provided download acceleration is enabled on their organization.****

![](assets/donload-assets-dialog-2.png)

要为组织启用基于IBM Aspera的加速下载，管理员可从管理工具面板的“常规设置”中启用“启用下载加速 **”选项(默** 认情况下为禁用状态) [](brand-portal-general-configuration.md#allow-download-acceleration) 。 To know more about prerequisites and troubleshooting steps for downloading asset files faster from Brand Portal and shared links, refer Guide to accelerate downloads from Brand Portal.[](../using/accelerated-download.md#main-pars-header)

### User Logins Report

A new report, to track user logins, has been introduced. The User Logins report can be instrumental in enabling organizations to audit and keep a check on the delegated administrators and other users of Brand Portal.****

The report logs display names, email IDs, personas (admin, viewer, editor, guest), groups, last login, activity status, and login count of each user from Brand Portal 6.4.2 deployment until the time of report generation. Administrators can export the report as .csv. Along with other reports, User Logins report enables organizations to more closely monitor user interactions with the approved brand resources, thereby ensuring conformance to corporate compliance offices.

![](assets/user-logins-1.png)

### Access to original renditions

Administrators can restrict user access to original image files (.jpeg, .tiff, .png, .bmp, .gif, .pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-graymap, x-portable-pixmap, x-rgb, x-xbitmap, x-xpixmap, x-icon, image/photoshop, image/x-photoshop, .psd, image/vnd.adobe.photoshop) and give access to low-resolution renditions which they download from Brand Portal or shared link. 此访问权限可以在用户组级别控制，该权限位于管理工具面板中“用户角色”页面的“组”选项卡中。

![](assets/access-original-rend-1.png)

* By default, all the users are able to download original renditions as the Access to Original is enabled for all.
* 管理员需要取消选中相应的复选框，以阻止一组用户访问原始演绎版。
* 如果用户是多个用户组的成员，但只有其中一个用户组具有限制，则这些限制适用于该用户。
* 这些限制不适用于管理员，即使管理员是受限用户组的成员。
* Permissions of the user sharing assets as link apply to the users who download assets using shared links.

### 卡片视图和列表视图上的文件夹层次结构路径

卡片视图中的文件夹卡现在向非管理员用户（编辑者、查看者和客人用户）显示文件夹层次结构信息。 此功能可让用户了解文件夹的位置，以及他们访问的与父层次结构相关的文件夹。

文件夹层次结构信息对于区分名称与从不同文件夹层次结构共享的其他文件夹相似的文件夹特别有用。 如果非管理员用户不知道与他们共享的资产的文件夹结构，则名称相似的资产／文件夹似乎会令人混淆。

* 相应卡上显示的路径会被截断以适合卡的大小。 但是，用户可以将鼠标悬停在截断路径上方时，将完整路径视为工具提示。

![](assets/folder-hierarchy1-1.png)

列表视图在列中显示资产向Brand Portal所有用户的路径。

![](assets/list-view-1.png)

### 查看资产属性的概述选项

Brand Portal为非管理员用户（编辑者、查看者、客人用户）提供“概述”选项，以查看选定资产／文件夹的资产属性。 “概述”选项可见：

1. 在顶部的工具栏中，选择资产／文件夹。
2. 在下拉菜单中，选择边栏选择器。

在选择资产／文件夹时选择“概述”选项后，用户可以查看资产创建的标题、路径和时间。 但是，在资产详细信息页面上，选择“概述”选项可让用户查看资产的元数据。

![](assets/overview-option-2.png)

![](assets/overview-rail-selector-2.png)

## 新配置

为管理员添加了六个新配置，以针对特定租户启用／禁用以下功能：

* 允许来宾访问
* 允许用户请求访问Brand Portal
* 允许管理员从Brand Portal中删除资产
* 允许创建公共集合
* 允许创建公共智能收藏集
* 允许下载加速

以上配置位于管理工具面板中的“访问”和“常规”设置下。

![](assets/access-configs-1.png)
![](assets/general-configs-1.png)
![](assets/admin-tools-panel-13.png)

### 用于配置身份验证集成的Adobe.io主机UI

Brand Portal 6.4.2 onwards uses Adobe.io https://legacy-oauth.cloud.adobe.io/ interface to create JWT application, which enables configuring oAuth integrations to allow AEM Assets integration with Brand Portal. [](https://legacy-oauth.cloud.adobe.io/)以前，用于配置OAuth集成的UI托管在https://marketing.adobe.com/developer/ [中](https://marketing.adobe.com/developer/)。 要了解有关将AEM资产与Brand Portal集成以将资产和集合发布到Brand Portal的更多信息，请参 [阅配置AEM资产与Brand Portal的集成](https://helpx.adobe.com/in/experience-manager/6-4/assets/using/brand-portal-configuring-integration.html)。

## Search Enhancements

Administrators can make the property predicates non-case sensitive by using the updated property predicate, which has a check for Ignore Case. This option is available for property predicate and multi-value property predicate.\
However, the non-case sensitive search is comparatively slower than default search for property predicate. If there are too many non-case sensitive predicates in the search filter, the search can slow down. It is, therefore, advised to use the non-case sensitive search judiciously.

## 6.4.1中的更改 {#what-changed-in-2}

Brand Portal 6.4.1是一个平台升级版本，它引入了多项新功能和重要增强功能，如浏览、搜索和性能增强，可以提供充分的客户体验。

### 浏览增强功能

* 新内容树边栏可快速导航资产层次结构。

![](assets/contenttree-2.png)

* 引入了新的键盘快捷键， _例如_ (p)用于导航到属性页面， _(e)用于编辑，_ 和(ctrl+c) __ 用于复制操作。
* Improved scrolling, lazy loading experience in card and list view for browsing large number of assets.
* 增强的卡片视图，支持基于视图设置的不同大小的卡片。

![](assets/cardviewsettings-1.png)

* 卡片视图现在可在将指针悬停在日期标签上方时显示日期／时间戳。

* 增强的列视图， **其中包含资产快照** 下的更多详细信息，您可以通过它导航到资产的详细信息页面。

![](assets/columnmoredetail.png)

* 列表视图现在默认显示第一列中资产的文件名以及区域设置、资产类型、尺寸、大小、评级和发布信息。 新 **的“视图设置** ”(View Settings)可用于配置要在“列表”视图中显示的详细程度。

* 改进了资产详细信息体验，能够使用新的导航按钮在资产之间来回导航，并查看资产计数。

![](assets/navbtn.png)

* 在资产的详细信息页面中预览从AEM上传的音频文件的新功能。
* 资产属性中提供的新相关资产功能。 与AEM上的其他源／派生资产相关并在Brand Portal上发布的资产现在在Brand Portal中保持其关系不变，并在属性页面上提供指向相关资产的链接。
* 已引入限制非管理员用户创建公共集合的新配置。 组织可以与Adobe支持团队合作，在特定帐户上配置此功能。

### 搜索增强功能

* 引入的功能可在导航到搜索项后返回到搜索结果中的同一位置，而无需再次运行搜索查询。
* 新的搜索结果计数用于显示已提供的搜索结果数。
* 改进的“文件类型搜索筛选器”能够根据细粒度的MIME类型（如。jpg、.png和。psd）筛选搜索结果，而之前的“图像”、“文档”和“多媒体”选项则不如此。
* 增强了集合的搜索筛选器，具有精确的时间戳而不是以前的时间滑块功能。
* 新的“访问类型”过滤器已引入，用于搜索公开或非公开的集合。

![](assets/accesstypefilter.png)

### 下载优化

* 直接下载单个大文件，无需创建zip文件，从而提高了速度和吞吐量。
* 链接共享功能的Zip下载限制从1GB增加到5GB。

* 用户现在可以选择仅下载自定义和原始文件，并防止开箱即用的再现，同时从Brand Portal或通过共享链接功能下载资产。

![](assets/excludeautorendition.png)

### 性能增强

* 资产下载速度提高了100%。
* 资产搜索响应提高40%。
* 浏览性能提高40%。

**注意**:根据实验室进行的测试，引用了一些改进。

### 增强的报告功能

**引入链接共享**&#x200B;报告为提供共享链接的相关信息，引入了新的报告。 “链接共享”报告列出在指定时间范围内与组织内部和外部用户共享的所有资产URL。 它还会通知链接何时共享、由谁共享以及何时过期。

![](assets/navigatereport.png)

**修改了访问使用情况报告的入口点**。使用情况报告现在与其他报告整合在一起，现在可以从资产报告控制台中查看。 要进入“资产报表”控制台，请从管理 **工具面板导航到创建／管理** “报表”。

![](assets/accessassetreport.png)

**通过Brand Portal上的报告** Reporting界面改进的用户体验变得更直观，并对组织实现更大的控制。 除了创建各种报告外，管理员现在还可以重新访问生成的报告并下载或删除它们，因为这些报告保存在Brand Portal中。

可通过添加或删除默认列来自定义所创建的每个报告。 此外，可以将自定义列添加到“下载”、“过期”和“发布”报表，以控制其粒度程度。

### 改进的管理工具

改进了元数据、搜索和报告管理工具中的属性选取器，该工具具有提前键入和浏览功能，可简化管理体验。

### 其他增强功能

* 现在，通过在AEM Assets Brand Portal复制对话框中标记“公共文件夹发布”复选框，可以将从AEM 6.3.2.1和6.4发布到Brand Portal的资产公开提供给Brand Portal的常规用户。

![](assets/public-folder-publish.png)

* 如果有人请求访问Brand Portal，则管理员将通过访问请求电子邮件获得通知，但Brand Portal通知区域中的通知除外。

## 6.3.2中的更改 {#what-changed-in-3}

Brand Portal 6.3.2包含面向热门客户请求的新增和增强功能以及一般性能增强。

### 请求对Brand Portal的访问权 {#request-access-to-brand-portal}

用户现在可以使用Brand Portal登录屏幕上新增的****需要访问功能请求对Brand Portal的访问权。

![](assets/bplogin_request_access.png)

根据用户是否具有Adobe ID，或是否需要创建Adobe ID，用户可以按照相应的工作流程提交请求。 Brand Portal产品管理员在其通知区域收到此类请求，并通过Adobe Admin Console授予访问权限。

有关详细信息，请参 [阅请求对Brand Portal的访问权](../using/brand-portal.md#requestaccesstobrandportal)。

### 资产下载报告中的增强功能 {#enhancement-in-the-assets-downloaded-report}

资产下载报告现在包括指定日期和时间范围内每位用户的资产下载计数。 用户可以以。csv格式下载此报告并编译数据，如许可资产的总下载计数。

![](assets/reports_download_downloaded_by.png)

有关详细信息，请参阅创建和管理其他报 [告中的步骤3和6](../using/brand-portal-reports.md#createandmanageadditionalreports)。

### Brand Portal维护通知 {#brand-portal-maintenance-notification}

Brand Portal现在在即将开展的维护活动前几天显示通知横幅。 示例通知：

![](assets/bp_maintenance_notification-1.png)

有关详细信息，请参阅 [Brand Portal维护通知](https://helpx.adobe.com/experience-manager/brand-portal/using/brand-portal.html#BrandPortalmaintenancenotification)。

### 使用链接共享功能增强共享的许可资源 {#enhancement-for-licensed-assets-shared-using-the-link-share-feature}

使用链接共享功能下载许可资产时，系统会提示您同意这些资产的许可协议。

![](assets/copyright_management.png)

有关详细信息，请参阅将资产作 [为链接共享中的步骤12](../using/brand-portal-link-share.md#shareassetsasalink)。

### 用户选取器增强功能 {#user-picker-enhancement}

用户选取器性能现已增强，以满足拥有大量用户群的客户的需求。

### Experience Cloud品牌变更 {#experience-cloud-branding-changes}

Brand Portal现在符合新的Adobe Experience Cloud品牌。

![](assets/bp_solution_switcher.png)

## 6.3.1中的更改 {#what-changed-in-4}

Brand Portal 6.3.1包含面向将Brand Portal与AEM协调的新增和增强功能。

### 升级的用户界面 {#upgraded-user-interface}

要使Brand Portal用户体验与AEM保持一致，Adobe将过渡到Coral 3用户界面。 此更改增强了整体可用性，包括导航和外观。

#### 增强的导航体验 {#enhanced-navigational-experience}

* 通过新的Adobe徽标快速访问管理工具：

![](assets/aemlogo-3.png)

* 通过叠加进行产品导航：

![](assets/overlay_navigation.png)

* 快速导航到父文件夹：

![](assets/navigationparentfolders.png)

* 快速搜索并导航到所需的内容和工具：

![](assets/omnisearchicon.png)

### 增强的浏览体验 {#enhanced-browsing-experience}

* 用于浏览嵌套文件夹的新列视图：

![](assets/millercolumnnavigation.png) ![](assets/multi-columnview.png)

* 在文件夹中的资产列表中，最新上传的资产将显示在顶部。

### 增强的搜索体验 {#enhanced-search-experience}

* 全新的Omni搜索功能便于您在键入搜索关键字时通过自动建议快速访问相关内容、功能或标记。 Omni搜索功能适用于所有搜索功能。

![](assets/omnisearch_whatsnew.png)

* 您还可以向Omni搜索添加搜索筛选器，以进一步缩小搜索范围并加快搜索速度。

![](assets/omnisearch_withfilters.png)

* 通过基于评级的新资产搜索功能，您可以搜索从AEM资产中发布的具有评级的资产。
* 新的多值搜索功能通过AND运算符接受多个关键字以更快地发现资源。
* 新的搜索提升功能可让您提高搜索相关性，以便特定资产显示在搜索结果的顶部。
* 使用基于路径的新搜索功能，您可以提供嵌套文件夹的路径，以便能够搜索该文件夹中的资产。

#### 基于智能标记的全新搜索 {#new-smart-tags-based-search}

如果具有智能标记的图像从AEM资产发布到Brand Portal，则可以在Brand Portal中使用智能标记名称作为搜索关键字搜索这些图像。 此功能仅对文件可用。

### 增强的下载体验 {#enhanced-downloading-experience}

下载嵌套文件夹后，您可以保留原始文件夹层次结构。 嵌套文件夹内的资源可以下载到单个文件夹中，而不是可以下载到单独的文件夹中。

### 改进的性能 {#improved-performance}

浏览、搜索和下载功能中的增强功能显着提高了Brand Portal的性能。

### 新的资产数字版权管理 {#new-digital-rights-management-for-assets}

管理员可以在共享资产之前设置资产的到期日期和时间。 资产过期后，查看者和编辑者可看到该资产，但无法下载。 当资产过期时，管理员会收到通知。

### 增强的资源排序 {#enhanced-asset-sorting}

在列表视图中对文件夹中的资产排序不再局限于在第一页上显示的资产数量。 无论是否在第一页中列出所有资产，都会对文件夹中的所有资产进行排序。

### 增强的报告功能 {#reporting-capabilities}

管理员可以创建和管理三种类型的报告——已下载、已过期和已发布的资产。 还可以配置报告中的列，并将报告导出为CSV格式。

![](assets/newreport.png)

### 其他元数据 {#additional-metadata}

Brand Portal 6.3.1引入了其他元数据，与AEM Assets 6.3相同。您可以使用架构编辑器表单控制应在资产属性页面上显示的元数据。 资产元数据对于外部链接共享用户不可见，他们只能使用链接共享URL预览和下载资产。

![](assets/additionsinmetadata.png)

### 管理员的其他功能 {#additional-capabilities-for-administrators}

* 在完成对登录屏幕墙纸的自定义设置之前，管理员可以预览更改。

![](assets/wallpaperpreview.png)

* 管理员添加新用户后，他们无需接受邀请即可添加到Brand Portal，而是会自动添加这些用户。

### AEM Assets 6.3中的新发布功能 {#new-publishing-capabilities-in-aem-assets}

* AEM管理员可以使用AEM 6.3 SP 1-CFP 1(6.3.1.1)将元数据架构从AEM资产发布到Brand Portal，该架构将在2017年第4季度发布。

![](assets/publish_metadataschemaaemassets.png)

* AEM管理员可以使用AEM 6.2 SP1-CFP7和AEM 6.3 SP 1-CFP 1(6.3.1.1)将所有标记从AEM资产发布到Brand Portal。

![](assets/publish_tags_aemassets.png)

* 从AEM资产中，您可以发布具有标记（包括智能标记）的资产和收藏集。 然后，您可以在Brand Portal中使用这些标记作为搜索关键字搜索这些资产或集合。

## Frequently asked questions {#frequently-asked-questions}

**Ques. 我是否将失去对我创建的任何现有资产、功能或配置的访问权？**
安**斯。** 您的所有现有功能和配置均保持不变。 您的最终用户不会受到影响，您的内容将保持不变。

**Ques. 我何时将转向新版本的Brand Portal?**
安**斯。** Brand Portal 6.4.4已于2019年2月发布至生产。 下一个Brand Portal版本预计将在2019年第3季度发布。

>[!NOTE]
>
>发布时间表是暂定的，并且可能会更改。 请联系您的Adobe客户经理或客户支持以获取更新的发行计划。

**Ques. 我的用户是否会受到影响？**
安**斯。** 此更改仅在Brand Portal中进行，因此不会对最终用户产生影响。

**Ques. 我是否需要执行任何操作？**
安**斯。** 管理员不需要执行任何操作。 访问新的Brand Portal后，请参阅文档以查看所有的技巧和口哨。

**Ques. 如有疑问，应与谁联系？**
安**斯。** 联系您的Adobe客户经理或客户支持。