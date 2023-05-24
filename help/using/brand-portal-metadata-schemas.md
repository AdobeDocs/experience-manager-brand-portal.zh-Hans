---
title: 使用元数据架构表单
seo-title: Use the metadata schema form
description: 元数据架构描述了“属性”页面的布局，以及针对使用特定架构的资源显示的元数据属性。 应用于资源的架构决定了其属性页面上显示的元数据字段。
seo-description: A metadata schema describes the layout of the Properties page and the metadata properties displayed for assets that use the particular schema. The schema that you apply to an asset determines the metadata fields that appear on its Properties page.
uuid: 1a944a3b-5152-425f-b1ea-bfe3331de928
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: administration
discoiquuid: 500b46da-ef67-46a0-a069-192f4b1a0eca
role: Admin
exl-id: fbedff90-a6cb-4175-8308-817cc9f5b450
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '1718'
ht-degree: 10%

---

# 使用元数据架构表单 {#use-the-metadata-schema-form}

元数据架构描述了“属性”页面的布局，以及针对使用特定架构的资源显示的元数据属性。 应用于资源的架构决定了其属性页面上显示的元数据字段。

此 **[!UICONTROL 属性]** 每个资源的页面包含默认元数据属性，具体取决于资源的MIME类型。 管理员可以使用元数据架构编辑器修改现有架构或添加自定义元数据架构。 Experience Manager Assets Brand Portal为各种MIME类型的资源提供默认表单。 但是，您还可以为此类资源添加自定义表单。

## 添加元数据架构表单 {#add-a-metadata-schema-form}

要创建新的元数据架构表单，请执行以下操作：

1. 在顶部的工具栏中，单击Experience Manager徽标以访问管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，单击 **[!UICONTROL 元数据架构]**.

   ![](assets/navigation-panel.png)

1. 在 **[!UICONTROL 元数据架构Forms]** 页面，单击 **[!UICONTROL 创建]**.

   ![](assets/create-metadata-schema-form.png)

1. 在 **[!UICONTROL 创建架构表单]** 对话框中，指定“架构”表单的标题，然后单击 **[!UICONTROL 创建]** 以完成表单创建过程。

   ![](assets/create-schema-form.png)

## 编辑元数据架构表单 {#edit-a-metadata-schema-form}

您可以编辑新添加或现有的元数据架构表单。 元数据架构表单包含从其父级派生的内容，包括选项卡和选项卡中的表单项。 您可以将这些表单项映射或配置到元数据节点中的字段。

您可以将新选项卡或表单项添加到元数据架构表单。 派生选项卡和表单项目（来自父项）处于锁定状态。 不能在子级别更改它们。

要编辑元数据架构表单，请执行以下操作：

1. 在顶部的工具栏中，单击Experience Manager徽标以访问管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，单击 **[!UICONTROL 元数据架构]**.
1. 从 **[!UICONTROL 元数据架构Forms]** 页面上，选择一个架构表单以编辑其属性，例如， **[!UICONTROL 收藏集]**.

   ![](assets/metadata-schema-forms.png)

   >[!NOTE]
   >
   >未编辑的模板在它们之前显示一个锁定符号。 如果自定义任何模板，则模板前的“锁定”符号将消失。

1. 在顶部的工具栏中，单击 **[!UICONTROL 编辑]**.

   此 **[!UICONTROL 元数据架构编辑器]** 打开页面，其中包含 **[!UICONTROL 基本]** 在左侧打开选项卡，然后 **[!UICONTROL 构建表单]** 选项卡在右侧打开。

1. 在 **[!UICONTROL 元数据架构编辑器]** 页面，自定义 **[!UICONTROL 属性]** 页面，方法是从中的组件类型列表中拖动一个或多个组件 **[!UICONTROL 构建表单]** 按Tab键转到 **[!UICONTROL 基本]** 选项卡。

   ![](assets/metadata-schemaeditor-page.png)

1. 要配置组件，请选择该组件并在 **[!UICONTROL 设置]** 选项卡。

### “构建表单”选项卡中的组件 {#components-in-the-build-form-tab}

此 **[!UICONTROL 构建表单]** 选项卡中列出了可在架构表单中使用的项目。 此 **[!UICONTROL 设置]** 选项卡提供您在选项中选择的每个项目的属性。 **[!UICONTROL 构建表单]** 选项卡。 下表列出了中可用的表单项目 **[!UICONTROL 构建表单]** 选项卡：

| 组件名称 | 描述 |
|---------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **[!UICONTROL 章节标题]** | 为常用组件列表添加章节标题。 |
| **[!UICONTROL 单行文本]** | 添加单行文本属性。 它以字符串形式存储。 |
| **[!UICONTROL 多值文本]** | 添加多值文本属性。 它存储为字符串数组。 |
| **[!UICONTROL 数字]** | 添加数字组件。 |
| **[!UICONTROL 日期]** | 添加日期组件。 |
| **[!UICONTROL 下拉列表]** | 添加下拉列表。 |
| **[!UICONTROL 标准标记]** | 添加标记. **注意：** 管理员可能需要更改路径值，例如， `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`，如果他们从Experience Manager Assets发布元数据架构表单，其中路径不包括租户信息，例如， `/etc/tags/<custom_tag_namespace>`. |
| **[!UICONTROL 智能标记]** | 如果您购买并配置了Experience Manager Assets智能标记加载项，则为自动检测到的标记。 |
| **[!UICONTROL 隐藏字段]** | 添加隐藏字段。 保存资源时，此参数将作为POST参数发送。 |
| **[!UICONTROL 资产引用对象]** | 添加此组件可查看资产引用的资产列表。 |
| **[!UICONTROL 资产引用]** | 添加以显示引用了资源的资源列表。 |
| **[!UICONTROL 资产评级]** | 在将资源发布到Brand Portal之前从Experience Manager Assets添加资源的平均评级。 |
| **[!UICONTROL 上下文元数据]** | 添加以控制其他元数据选项卡在资源的“属性”页面中的显示。 |

>[!NOTE]
>
>不使用 **[!UICONTROL 产品引用]**，因为它不起作用。

#### 编辑元数据组件 {#edit-the-metadata-component}

要编辑表单上元数据组件的属性，请单击该组件，然后在 **[!UICONTROL 设置]** 选项卡。

* **[!UICONTROL 字段标签]**：在资产的属性页面上显示的元数据属性的名称。

* **[!UICONTROL 映射到属性]**：此属性的值提供资产节点的相对路径/名称，资产节点保存在CRX存储库中。 它始于&quot;**./**“，因为指示路径在资产的节点下。

以下是此属性的有效值：

— `./jcr:content/metadata/dc:title`：将该值作为属性存储在资产的元数据节点中 [!UICONTROL `dc:title`].

— `./jcr:created`：在资产的节点显示jcr属性。 如果您在视图属性上配置这些属性，我们建议您将这些属性标记为“禁用编辑”，因为它们是受保护属性。否则，在保存资产的属性时，会出现“资产修改失败”错误。

* **[!UICONTROL 占位符]**：使用此属性可以向用户提供与元数据属性相关的任何信息。
* **[!UICONTROL 必需]**：使用此属性可在“属性”页面上将元数据属性标记为必需。
* **[!UICONTROL 禁用编辑]**：使用此属性可使metadata属性在“属性”页面上不可编辑。
* **[!UICONTROL 以只读方式显示空字段]**：标记此属性以在“属性”页面上显示元数据属性，即使它没有值也是如此。 默认情况下，当元数据属性没有值时，它不会列在属性页面上。
* **[!UICONTROL 描述]**：使用此属性可添加对元数据组件的简短描述。
* **[!UICONTROL “删除”图标]**：单击此图标可从架构表单中删除组件。

![](assets/delete_icon_editmetadataschemaform.png)

>[!NOTE]
>
>在资源的元数据编辑器表单中，所有元数据字段均为只读。 因为在将资源发布到Brand Portal之前，必须在Experience Manager Assets中编辑资源的元数据。

#### 在架构表单中添加或删除选项卡 {#add-or-delete-a-tab-in-the-schema-form}

默认架构表单包括 **[!UICONTROL 基本]** 和 **[!UICONTROL 高级]** 选项卡。 通过架构编辑器，可以添加或删除选项卡。

![](assets/add_delete_tabs_metadataschemaform.png)

* 要在架构表单上添加新选项卡，请单击 **[!UICONTROL +]**. 默认情况下，新选项卡的名称为“Unnamed-1”。 您可以从以下位置修改名称： **[!UICONTROL 设置]** 选项卡。

![](assets/add-tab-metadata-form.png)

* 要删除选项卡，请单击 **[!UICONTROL x]**. 单击 **[!UICONTROL 保存]** 以保存更改。

## 将元数据架构应用到文件夹 {#apply-a-metadata-schema-to-a-folder}

Brand Portal允许您自定义和控制元数据架构，以便 **[!UICONTROL 属性]** 资产的页面仅显示您选择显示的特定信息。 要控制中显示的元数据，请执行以下操作 **[!UICONTROL 属性]** 页面，从元数据架构表单中删除所需的元数据并将其应用到特定文件夹。

要将元数据架构表单应用于文件夹，请执行以下操作：

1. 在顶部的工具栏中，单击Experience Manager徽标以访问管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，单击 **[!UICONTROL 元数据架构]**.

1. 从 **[!UICONTROL 元数据架构Forms]** 页面上，选择要应用于资源的架构表单，例如， **[!UICONTROL 服装]**.

   ![](assets/apply-metadata-schema-form-to-folder.png)

1. 在顶部的工具栏中，单击 **[!UICONTROL 应用到文件夹]**.

1. 从 **[!UICONTROL 选择文件夹]** 页面上，导航到要应用的文件夹 **[!UICONTROL 服装]** 元数据架构，例如， **[!UICONTROL 手套]**.

   ![](assets/apply_metadata_schemaformtofoldergloves.png)

1. 单击 **[!UICONTROL 应用]** 以将元数据架构表单应用于文件夹。

   中可用的元数据 **[!UICONTROL 服装]** 元数据架构表单应用于 **[!UICONTROL 手套]** 文件夹中可见 **[!UICONTROL 属性]** 文件夹的URL页面。

   ![](assets/folder_metadata_properties.png)

>[!NOTE]
>
>如果将包含嵌套架构的架构应用于包含视频文件的文件夹，则可能无法正确呈现视频文件的元数据属性。 为确保元数据属性正确呈现，请删除嵌套架构并仅将父架构应用于文件夹。

## 删除元数据架构表单 {#delete-a-metadata-schema-form}

Brand Portal仅允许您删除自定义架构表单。 不允许删除默认架构表单/模板。 但是，您可以删除这些表单中的任何自定义更改。

要删除表单，请选择一个表单，然后单击 **[!UICONTROL 删除]** 图标。

![](assets/delete_icon_metadataschemaeditorform.png)

>[!NOTE]
>
>删除对默认表单所做的自定义更改后， **[!UICONTROL 锁定]** 符号会重新出现在元数据架构界面上的表单名称之前，以指示表单将恢复到其默认状态。

## MIME类型的架构表单 {#schema-forms-for-mime-types}

### 为MIME类型添加新表单 {#adding-new-forms-for-mime-types}

除了默认表单之外，您还可以为各种MIME类型的资产添加自定义表单，或在相应的表单类型下创建新表单。 例如，要为 **[!UICONTROL image/png]** 子类型添加新模板，请在“image”表单下创建表单。架构表单的标题是子类型名称。在本例中，标题为“png”。

#### 为各种MIME类型使用现有架构模板 {#using-an-existing-schema-template-for-various-mime-types}

您可以为其他MIME类型使用现有模板。 例如，使用 **image/jpeg** MIME类型资产的表单 **image/png**.

在这种情况下，请在 [!UICONTROL `/etc/dam/metadataeditor/mimetypemappings`] 在CRX存储库中。 指定节点名称并定义以下属性：

| **名称** | **类型** | **值** |
|---|---|---|
| exposedmimetype | 字符串 | image/jpeg |
| mimetypes | 字符串[] | image/png |

* **exposedmimetype**：要映射的现有表单的名称
* **mimetypes**：使用中定义的表单的MIME类型列表 **exposedmimetype** 属性

Brand Portal映射以下MIME类型和架构表单：

| **架构表单** | **MIME类型** |
|---|---|
| image/jpeg | image/pjpeg |
| image/tiff | image/x-tiff |
| application/pdf | application/postscript |
| application/x-ImageSet | Multipart/Related; type=application/x-ImageSet |
| application/x-SpinSet | Multipart/Related; type=application/x-SpinSet |
| application/x-MixedMediaSet | Multipart/Related; type=application/x-MixedMediaSet |
| video/quicktime | video/x-quicktime |
| video/mpeg4 | video/mp4 |
| video/avi | video/avi， video/msvideo， video/x-msvideo |
| video/wmv | video/x-ms-wmv |
| video/flv | video/x-flv |

以下是默认元数据属性的列表：

* jcr:content/metadata/cq:tags
* jcr:content/metadata/dc:format
* jcr:content/metadata/dam:status
* jcr：content/metadata/videoCodec
* jcr：content/metadata/audioCodec
* jcr：content/metadata/dc：title
* jcr：content/metadata/dc：description
* jcr：content/metadata/xmpMM：InstanceID
* jcr：content/metadata/xmpMM：DocumentID
* jcr：content/metadata/dam：sha1
* jcr：content/metadata/dam：solutionContext
* jcr：content/metadata/videoBitrate
* jcr：content/metadata/audioBitrate
* jcr：content/usages/usedBy
* jcr:content/jcr:lastModified
* jcr:content/metadata/prism:expirationDate
* jcr：content/onTime
* jcr：content/offTime
* jcr:content/metadata/dam:size
* jcr：content/metadata/tiff：ImageWidth
* jcr：content/metadata/tiff：ImageLength
