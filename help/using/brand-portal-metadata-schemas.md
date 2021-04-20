---
title: 使用元数据架构表单
seo-title: 使用元数据架构表单
description: 元数据模式描述了“属性”页面的布局以及为使用特定模式的资产显示的元数据属性。 您应用于资产的模式决定了在其“属性”页面上显示的元数据字段。
seo-description: 元数据模式描述了“属性”页面的布局以及为使用特定模式的资产显示的元数据属性。 您应用于资产的模式决定了在其“属性”页面上显示的元数据字段。
uuid: 1a944a3b-5152-425f-b1ea-bfe3331de928
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: administration
discoiquuid: 500b46da-ef67-46a0-a069-192f4b1a0eca
role: Administrator
translation-type: tm+mt
source-git-commit: 263653916e4bc183827c197c3beb137c9e59ccb1
workflow-type: tm+mt
source-wordcount: '1757'
ht-degree: 32%

---


# 使用元数据架构表单 {#use-the-metadata-schema-form}

元数据模式描述了“属性”页面的布局以及为使用特定模式的资产显示的元数据属性。 您应用于资产的模式决定了在其“属性”页面上显示的元数据字段。

每个资产的&#x200B;**[!UICONTROL 属性]**&#x200B;页面包含默认元数据属性，具体取决于资产的MIME类型。 管理员可以使用元数据模式编辑器修改现有模式或添加自定义元数据模式。 AEM Assets Brand Portal为各种MIME类型的资产提供默认表单。 但是，您也可以为此类资产添加自定义表单。

## 添加元数据模式表单{#add-a-metadata-schema-form}

要创建新的元数据模式表单，请执行以下操作：

1. 从顶部的AEM工具栏中，单击Adobe徽标以访问管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，单击&#x200B;**[!UICONTROL 元数据模式]**。

   ![](assets/navigation-panel.png)

1. 在&#x200B;**[!UICONTROL 元数据模式Forms]**&#x200B;页面上，单击&#x200B;**[!UICONTROL 创建]**。

   ![](assets/create-metadata-schema-form.png)

1. 在&#x200B;**[!UICONTROL 创建模式表单]**&#x200B;对话框中，指定模式表单的标题，然后单击&#x200B;**[!UICONTROL 创建]**&#x200B;以完成表单创建过程。

   ![](assets/create-schema-form.png)

## 编辑元数据模式表单{#edit-a-metadata-schema-form}

您可以编辑新添加的或现有的元数据模式表单。 元数据模式表单包含从其父表单派生的内容，包括选项卡和选项卡中的表单项。 您可以将这些表单项目映射或配置到元数据节点中的字段。

可以向元数据架构表单中添加新的选项卡或表单项目。（从父表单）派生的选项卡和表单项目处于锁定状态。无法从子级别更改它们。

要编辑元数据模式表单，请执行以下操作：

1. 从顶部的AEM工具栏中，单击Adobe徽标以访问管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，单击&#x200B;**[!UICONTROL 元数据模式]**。
1. 在&#x200B;**[!UICONTROL 元数据模式Forms]**&#x200B;页中，选择一个模式表单以编辑其属性，例如&#x200B;**[!UICONTROL 集合]**。

   ![](assets/metadata-schema-forms.png)

   >[!NOTE]
   >
   >未经编辑的模板前会显示一个锁符号。 如果自定义任何模板，则模板前的锁符号将消失。

1. 在顶部的工具栏中，单击&#x200B;**[!UICONTROL 编辑]**。

   此时将打开&#x200B;**[!UICONTROL 元数据模式编辑器]**&#x200B;页，其中左侧的&#x200B;**[!UICONTROL 基本]**&#x200B;选项卡打开，右侧的&#x200B;**[!UICONTROL 构建表单]**&#x200B;选项卡打开。

1. 在&#x200B;**[!UICONTROL 元数据模式编辑器]**&#x200B;页中，自定义资产的&#x200B;**[!UICONTROL 属性]**&#x200B;页，方法是将&#x200B;**[!UICONTROL 构建表单]**&#x200B;选项卡中组件类型列表中的一个或多个组件拖至&#x200B;**[!UICONTROL 基本]**&#x200B;选项卡。

   ![](assets/metadata-schemaeditor-page.png)

1. 要配置组件，请选择该组件并在&#x200B;**[!UICONTROL 设置]**&#x200B;选项卡中修改其属性。

### 构建表单选项卡{#components-in-the-build-form-tab}中的组件

**[!UICONTROL 构建表单]**&#x200B;选项卡列表了您可以在模式表单中使用的项目。 **[!UICONTROL 设置]**&#x200B;选项卡提供您在&#x200B;**[!UICONTROL 构建表单]**&#x200B;选项卡中选择的每个项目的属性。 下表列表了&#x200B;**[!UICONTROL 构建表单]**&#x200B;选项卡中可用的表单项：

| 组件名称 | 描述 |
|---------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **[!UICONTROL 章节标题]** | 添加一系列常用组件的章节标题。 |
| **[!UICONTROL 单行文本]** | 添加单行文本属性。它将作为字符串存储。 |
| **[!UICONTROL 多值文本]** | 添加多值文本属性。 它将作为字符串数组存储。 |
| **[!UICONTROL 数字]** | 添加数字组件。 |
| **[!UICONTROL 日期]** | 添加日期组件。 |
| **[!UICONTROL 下拉列表]** | 添加下拉列表。 |
| **[!UICONTROL 标准标记]** | 添加标记。**注意：** 管理员可能需要更改路径值，例如 `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`，如果他们从AEM发布元数据模式表单，而路径不包含租户信息，则需要更 `/etc/tags/<custom_tag_namespace>`改。 |
| **[!UICONTROL 智能标记]** | 如果您已购买并配置了AEM智能标记加载项，则会自动检测标记。 |
| **[!UICONTROL 隐藏字段]** | 添加隐藏字段。在保存资产时，该字段将作为 POST 参数发送。 |
| **[!UICONTROL 资产引用对象]** | 添加此组件可查看该资产所引用的其他资产的列表。 |
| **[!UICONTROL 资产引用]** | 添加此组件可显示引用该资产的其他资产的列表。 |
| **[!UICONTROL 资产评级]** | 从AEM Assets添加的资产在发布到Brand Portal之前的平均评级。 |
| **[!UICONTROL 上下文元数据]** | 添加此组件可控制资产属性页面中其他元数据选项卡的显示。 |

>[!NOTE]
>
>请勿使用&#x200B;**[!UICONTROL 产品引用]**，因为它无法正常工作。

#### 编辑元数据组件{#edit-the-metadata-component}

要在表单上编辑元数据组件的属性，请单击相应的组件，然后在&#x200B;**[!UICONTROL 设置]**&#x200B;选项卡中编辑其属性。

* **[!UICONTROL 字段标签]**:资产的“属性”页面上显示的元数据属性的名称。

* **[!UICONTROL 映射到属性]**：此属性的值提供资产节点在 CRX 存储库中保存的相对路径/名称。该值以“**./**”开头，因为这表示该路径位于资产的节点下。

以下是此属性的有效值：

— `./jcr:content/metadata/dc:title`:将该值作为属性[!UICONTROL `dc:title`]存储在资产的元数据节点。

— `./jcr:created`:在资产的节点上显示jcr属性。 如果您在视图属性上配置这些属性，我们建议您将这些属性标记为“禁用编辑”，因为它们是受保护属性。否则，在保存资产的属性时，会出现“资产修改失败”错误。

* **[!UICONTROL 占位符]**：使用此属性可向用户提供有关元数据属性的任何相关信息。
* **[!UICONTROL 必需]**：使用此属性可在“属性”页面上将元数据属性标记为必需。
* **[!UICONTROL 禁用编辑]**：使用此属性可让“属性”页面上的元数据属性变得不可编辑。
* **[!UICONTROL 在只读模式下显示空字段]**：标记此属性可使没有值的元数据属性显示在“属性”页面上。默认情况下，当元数据属性没有值时，不会在“属性”页面上将其列出。
* **[!UICONTROL 描述]**：使用此属性可添加对元数据组件的简短描述。
* **[!UICONTROL 删除图标]**:单击此图标可从模式表单中删除组件。

![](assets/delete_icon_editmetadataschemaform.png)

>[!NOTE]
>
>所有元数据字段在资产的元数据编辑器表单中都是只读的。 由于资产的元数据必须在AEM Assets中进行编辑，才能将资产发布到Brand Portal。

#### 在模式表单{#add-or-delete-a-tab-in-the-schema-form}中添加或删除选项卡

默认模式表单包括&#x200B;**[!UICONTROL Basic]**&#x200B;和&#x200B;**[!UICONTROL Advanced]**&#x200B;选项卡。 通过架构编辑器，可以添加或删除选项卡。

![](assets/add_delete_tabs_metadataschemaform.png)

* 要在模式表单上添加新选项卡，请单击&#x200B;**[!UICONTROL +]**。 默认情况下，新选项卡的名称为“未命名–1”。 您可以从&#x200B;**[!UICONTROL 设置]**&#x200B;选项卡中修改该名称。

![](assets/add-tab-metadata-form.png)

* 要删除选项卡，请单击&#x200B;**[!UICONTROL x]**。 单击&#x200B;**[!UICONTROL 保存]**&#x200B;以保存更改。

## 将元数据模式应用到文件夹{#apply-a-metadata-schema-to-a-folder}

Brand Portal允许您自定义和控制元数据模式，以便资产的&#x200B;**[!UICONTROL 属性]**&#x200B;页面仅显示您选择显示的特定信息。 要控制在&#x200B;**[!UICONTROL 属性]**&#x200B;页面中显示的元数据，请从元数据模式表单中删除所需的元数据，并将其应用到特定文件夹。

要将元数据模式表单应用到文件夹，请执行以下操作：

1. 从顶部的AEM工具栏中，单击Adobe徽标以访问管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，单击&#x200B;**[!UICONTROL 元数据模式]**。

1. 在&#x200B;**[!UICONTROL 元数据模式Forms]**&#x200B;页面中，选择要应用于资产的模式表单，例如&#x200B;**[!UICONTROL clothing]**。

   ![](assets/apply-metadata-schema-form-to-folder.png)

1. 在顶部的工具栏中，单击&#x200B;**[!UICONTROL 应用到文件夹]**。

1. 在&#x200B;**[!UICONTROL 选择文件夹]**&#x200B;页面中，导航到要应用&#x200B;**[!UICONTROL clothing]**&#x200B;元数据模式的文件夹，例如&#x200B;**[!UICONTROL Gloves]**。

   ![](assets/apply_metadata_schemaformtofoldergloves.png)

1. 单击&#x200B;**[!UICONTROL 应用]**&#x200B;将元数据模式表单应用到文件夹。

   **[!UICONTROL clothing]**&#x200B;元数据模式表单中可用的元数据应用于&#x200B;**[!UICONTROL Gloves]**&#x200B;文件夹，并可在文件夹的&#x200B;**[!UICONTROL 属性]**&#x200B;页面中看到。

   ![](assets/folder_metadata_properties.png)

>[!NOTE]
>
>如果将包含嵌套模式的模式应用到包含视频文件的文件夹，则视频文件的元数据属性可能无法正确呈现。 要确保元数据属性正确呈现，请删除嵌套模式，并仅将父模式应用到文件夹。

## 删除元数据模式表单{#delete-a-metadata-schema-form}

Brand Portal仅允许您删除自定义模式表单。 您无法删除默认的架构表单/模板。但是，您可以删除对这些表单所做的任何自定义更改。

要删除某个表单，请选择该表单，然后单击&#x200B;**[!UICONTROL 删除]**&#x200B;图标。

![](assets/delete_icon_metadataschemaeditorform.png)

>[!NOTE]
>
>删除对默认表单所做的自定义更改后，**[!UICONTROL 锁定]**&#x200B;符号将重新显示在元数据模式界面上的表单名称前，以指示表单已恢复为默认状态。

## 模式MIME类型{#schema-forms-for-mime-types}的表单

### 为 MIME 类型添加新表单 {#adding-new-forms-for-mime-types}

除了默认表单之外，您还可以为各种MIME类型的资产添加自定义表单，或在适当的表单类型下创建新表单。 例如，要为 **[!UICONTROL image/png]** 子类型添加新模板，请在“image”表单下创建表单。架构表单的标题是子类型名称。在这种情况下，标题为“png”。

#### 为各种 MIME 类型使用现有架构模板 {#using-an-existing-schema-template-for-various-mime-types}

您可以将现有模板用于其他MIME类型。例如，对于MIME类型为&#x200B;**image/png**&#x200B;的资产，请使用&#x200B;**image/jpeg**&#x200B;表单。

在这种情况下，请在CRX存储库中的[!UICONTROL `/etc/dam/metadataeditor/mimetypemappings`]处创建新节点。 指定节点的名称并定义以下属性：

| **名称** | **类型** | **值** |
|---|---|---|
| exposedmimetype | 字符串 | image/jpeg |
| mimetypes | String[] | image/png |

* **exposedmimetype**:要映射的现有表单的名称
* **mimetypes**:列表使用exposedmimetypeattribute中定义的表单的MIME类 **** 型

Brand Portal映射以下MIME类型和模式表单：

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
| video/avi | video/avi、video/msvideo、video/x-msvideo |
| video/wmv | video/x-ms-wmv |
| video/flv | video/x-flv |

以下是默认元数据属性的列表:

* jcr:content/metadata/cq:tags
* jcr:content/metadata/dc:format
* jcr:content/metadata/dam:status
* jcr:content/metadata/videoCodec
* jcr:content/metadata/audioCodec
* jcr:content/metadata/dc:title
* jcr:content/metadata/dc:description
* jcr:content/metadata/xmpMM:InstanceID
* jcr:content/metadata/xmpMM:DocumentID
* jcr:content/metadata/dam:sha1
* jcr:content/metadata/dam:solutionContext
* jcr:content/metadata/videoBitrate
* jcr:content/metadata/audioBitrate
* jcr:content/usages/usedBy
* jcr:content/jcr:lastModified
* jcr:content/metadata/prism:expirationDate
* jcr:content/onTime
* jcr:content/offTime
* jcr:content/metadata/dam:size
* jcr:content/metadata/tiff:ImageWidth
* jcr:content/metadata/tiff:ImageLength
