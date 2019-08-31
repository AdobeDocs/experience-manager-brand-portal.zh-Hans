---
title: 使用元数据架构表单
seo-title: 使用元数据架构表单
description: 元数据架构描述了属性页面的布局以及为使用特定架构的资产显示的元数据属性。应用于资产的架构会确定显示在其“属性”页面上的元数据字段。
seo-description: 元数据架构描述了属性页面的布局以及为使用特定架构的资产显示的元数据属性。应用于资产的架构会确定显示在其“属性”页面上的元数据字段。
uuid: a944a3b-5152-425f-b1 ea-bfe3331 de928
content-type: 引用
products: SG_ EXPERIENCE MANAGER/Brand_ Portal
topic-tags: administration
discoiquuid: 500b46da-ef67-46a0-a069-192f4 b1 a0 a0 ca
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# 使用元数据架构表单 {#use-the-metadata-schema-form}

元数据架构描述了属性页面的布局以及为使用特定架构的资产显示的元数据属性。应用于资产的架构会确定显示在其“属性”页面上的元数据字段。

每个资产的 **[!UICONTROL “属性]** ”页面包括默认元数据属性，具体取决于资产的MIME类型。管理员可以使用元数据架构编辑器修改现有架构或添加自定义元数据架构。AEM Assets Brand Portal为各种MIME类型的资产提供默认表单。但是，您还可以为此类资产添加自定义表单。

## Add a metadata schema form {#add-a-metadata-schema-form}

要创建新的元数据架构表单，请执行以下操作：

1. 在顶部的AEM工具栏中，单击Adobe徽标以访问管理工具。

   ![](assets/aemlogo.png)

2. 从管理工具面板中，单击 **[!UICONTROL 元数据架构]**。

   ![](assets/navigation-panel.png)

3. 在 **[!UICONTROL 元数据架构表单]** 页面上，单击 **[!UICONTROL 创建]**。

   ![](assets/create-metadata-schema-form.png)

4. 在 **[!UICONTROL 创建架构表单]** 对话框中，指定架构表单的标题，然后单击 **[!UICONTROL 创建]** 以完成表单创建过程。

   ![](assets/create-schema-form.png)

## Edit a metadata schema form {#edit-a-metadata-schema-form}

您可以编辑新添加的或现有的元数据架构表单。元数据架构表单包含从其父项派生的内容，包括选项卡中的选项卡和表单项目。您可以将这些表单项目映射或配置为元数据节点内的字段。

可以向元数据架构表单中添加新的选项卡或表单项目。（从父表单）派生的选项卡和表单项目处于锁定状态。无法从子级别更改它们。

要编辑元数据架构表单，请执行以下操作：

1. 在顶部的AEM工具栏中，单击Adobe徽标以访问管理工具。

   ![](assets/aemlogo.png)

2. 从管理工具面板中，单击 **[!UICONTROL 元数据架构]**。
3. 从 **[!UICONTROL 元数据架构表单]** 页面中，选择架构表单以编辑其属性，例如 **[!UICONTROL 集合]**。

   ![](assets/metadata-schema-forms.png)

   >[!NOTE]
   >
   >未编辑的模板前面会显示一个锁定符号。如果您自定义任何模板，则模板前面的锁符号会消失。

4. 在顶部的工具栏中，单击 **[!UICONTROL 编辑]**。

   **[!UICONTROL 此时将打开元数据架构编辑器]** 页面，左侧将 **[!UICONTROL 打开基本]** 选项卡，右侧将 **[!UICONTROL 打开“构建表单]** ”选项卡。

5. In the **[!UICONTROL Metadata Schema Editor]** page, customize the **[!UICONTROL Properties]** page of the asset by dragging one or more components from a list of component types in the **[!UICONTROL Build Form]** tab to the **[!UICONTROL Basic]** tab.

   ![](assets/metadata-schemaeditor-page.png)

6. To configure a component, select it and modify its properties in the **[!UICONTROL Settings]** tab.

### Components in the Build Form tab {#components-in-the-build-form-tab}

**[!UICONTROL 构建表单]** 选项卡列出了可在架构表单中使用的项目。**[!UICONTROL 设置]** 选项卡提供您在 **[!UICONTROL 构建表单]** 选项卡中选择的每个项目的属性。The following table lists the form items available in the **[!UICONTROL Build Form]** tab:

| 组件名称 | 描述 |
|---------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL 章节标题] | 为常见组件列表添加章节标题。 |
| [!UICONTROL 单行文本] | 添加单行文本属性。它存储为字符串。 |
| [!UICONTROL 多值文本] | 添加多值文本属性。它将作为字符串数组存储。 |
| [!UICONTROL 数字] | 添加数字组件。 |
| [!UICONTROL 日期] | 添加日期组件。 |
| [!UICONTROL 下拉列表] | 添加下拉列表。 |
| [!UICONTROL 标准标记] | 添加标记. **注意：** 管理员可能需要更改路径值(例如， `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`如果他们从AEM发布元数据架构表单，则路径不包括租户信息，例如，) `/etc/tags/<custom_tag_namespace>`。 |
| [!UICONTROL 智能标记] | 如果您已购买并配置AEM智能标记加载项，则自动检测到标记。 |
| [!UICONTROL 隐藏字段] | 添加隐藏字段。保存资产时，它将作为POST参数发送。 |
| [!UICONTROL 资产引用对象] | 添加此组件可查看资产引用的资产列表。 |
| [!UICONTROL 资产引用] | 添加以显示引用该资产的资产列表。 |
| [!UICONTROL 资产评级] | 在将AEM资产发布到Brand Portal之前，从AEM资产添加的平均评级。 |
| [!UICONTROL 上下文元数据] | 添加以控制资产“属性”页面中其他元数据选项卡的显示。 |

>[!NOTE]
>
>请勿使用 **[!UICONTROL 产品引用]**，因为它不起作用。

#### 编辑元数据组件 {#edit-the-metadata-component}

要在表单上编辑元数据组件的属性，请单击相应的组件，然后在&#x200B;**[!UICONTROL 设置]选项卡中编辑其属性。**

* **[!UICONTROL 字段标签]**：资产的属性页面上显示的元数据属性的名称。

* **[!UICONTROL 映射到属性]**：此属性的值提供资产节点在 CRX 存储库中保存的相对路径/名称。该值以“**./**”开头，因为这表示该路径位于资产的节点下。

以下是此属性的有效值：

-- [!UICONTROL `./jcr:content/metadata/dc:title`]: Stores the value at the asset's metadata node as the property [!UICONTROL `dc:title`].

-- [!UICONTROL `./jcr:created`]: Displays the jcr property at the asset's node. 如果您对查看属性配置这些属性，我们建议您将它们标记为“禁用编辑”，因为它们是受保护的属性。否则，当您保存资产的属性时，系统会出现“无法修改资产”错误。

* **[!UICONTROL 占位符]**：使用此属性可向用户提供有关元数据属性的任何相关信息。
* **[!UICONTROL 必需]**：使用此属性可在“属性”页面上将元数据属性标记为必需。
* **[!UICONTROL 禁用编辑]**：使用此属性可让“属性”页面上的元数据属性变得不可编辑。
* **[!UICONTROL 在只读模式下显示空字段]**：标记此属性可使没有值的元数据属性显示在“属性”页面上。默认情况下，当元数据属性没有值时，不会在“属性”页面上将其列出。
* **[!UICONTROL 描述]**：使用此属性可添加对元数据组件的简短描述。
* **[!UICONTROL 删除图标]**：单击此图标可从架构表单中删除组件。

![](assets/delete_icon_editmetadataschemaform.png)

>[!NOTE]
>
>所有元数据字段都是资产的元数据编辑器表单中的只读字段。由于资产元数据必须在AEM资产中进行编辑，然后资产才会发布到Brand Portal。

#### 在架构表单中添加或删除选项卡 {#add-or-delete-a-tab-in-the-schema-form}

The default schema form includes the **[!UICONTROL Basic]** and **[!UICONTROL Advanced]** tabs. 通过架构编辑器，可以添加或删除选项卡。

![](assets/add_delete_tabs_metadataschemaform.png)

* To add a new tab on a schema form, click **[!UICONTROL +]**. 默认情况下，新选项卡的名称为“未命名-1”。You can modify the name from the **[!UICONTROL Settings]** tab.

![](assets/add-tab-metadata-form.png)

* 要删除选项卡，请单击 **[!UICONTROL “x]**”。Click **[!UICONTROL Save]** to save the changes.

## 将元数据架构应用到文件夹 {#apply-a-metadata-schema-to-a-folder}

Brand Portal允许您自定义和控制元数据架构，以便资产的 [!UICONTROL “属性] ”页面仅显示您选择显示的特定信息。要控制 [!UICONTROL “属性] ”页面中显示的元数据，请从元数据架构表单中删除所需的元数据，并将其应用到特定文件夹。

要将元数据架构表单应用到文件夹，请执行以下操作：

1. 在顶部的AEM工具栏中，单击Adobe徽标以访问管理工具。

   ![](assets/aemlogo.png)

2. 从管理工具面板中，单击 **[!UICONTROL 元数据架构]**。

3. 从 **[!UICONTROL 元数据架构表单]** 页面中，选择要应用于资产的架构表单，例如 [!UICONTROL 服装。]

   ![](assets/apply-metadata-schema-form-to-folder.png)

4. 在顶部的工具栏中，单击 **[!UICONTROL “应用到文件夹]**”。

5. 从 **[!UICONTROL “选择文件夹”]** 页面，导航到您要应用 **[!UICONTROL 服装]** 元数据架构的文件夹， **[!UICONTROL 例如，Glags]**。

   ![](assets/apply_metadata_schemaformtofoldergloves.png)

6. 单击 **[!UICONTROL “应用]** ”以将元数据架构表单应用到文件夹。

   **[!UICONTROL 服装]** 元数据架构表单中的元数据将应用于 **[!UICONTROL Glaves]** 文件夹，并显示在该文件夹的 **[!UICONTROL “属性]** ”页面中。

   ![](assets/folder_metadata_properties.png)

>[!NOTE]
>
>如果将包含嵌套架构的架构应用于包含视频文件的文件夹，则视频文件的元数据属性可能无法正确呈现。要确保正确渲染元数据属性，请删除嵌套架构，并仅应用父架构到文件夹。

## Delete a metadata schema form {#delete-a-metadata-schema-form}

Brand Portal只允许您删除自定义架构表单。您无法删除默认的架构表单/模板。但是，您可以删除对这些表单所做的任何自定义更改。

要删除某个表单，请选择该表单，然后单击&#x200B;**[!UICONTROL 删除]图标。**

![](assets/delete_icon_metadataschemaeditorform.png)

>[!NOTE]
>
>After you delete the custom changes made to a default form, the **[!UICONTROL Lock]** symbol reappears before the form name on the Metadata Schema interface to indicate that the form is reverted to its default state.

## Schema forms for MIME TYPES {#schema-forms-for-mime-types}

### 为 MIME 类型添加新表单 {#adding-new-forms-for-mime-types}

除了默认表单之外，您还可以为各种MIME类型的资产添加自定义表单，或根据相应的表单类型创建新表单。For example, to add a new template for the **[!UICONTROL image/png]** subtype, create the form under the "image" forms. 架构表单的标题为子类型名称。在这种情况下，标题为“png”。

#### 为各种 MIME 类型使用现有架构模板 {#using-an-existing-schema-template-for-various-mime-types}

You can use an existing template for a different MIME type. For example, use the **image/jpeg** form for assets of MIME type **image/png**.

In this case, create a new node at [!UICONTROL `/etc/dam/metadataeditor/mimetypemappings`] in the CRX repository. 指定节点的名称并定义以下属性：

| **名称** | **类型** | **值** |
|---|---|---|
| exposedmimetype | 字符串 | image/jpeg |
| mimetypes | String[] | image/png |

* **exposedmimetype**：要映射的现有表单的名称
* **mimetypes**：使用 **exposedmimetype** 属性中定义的表单的MIME类型列表

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
| video/avi | video/avi、video/msvideo、video/x-msvideo |
| video/wmv | video/x-ms-wmv |
| video/flv | video/x-flv |

下面是默认元数据属性的列表：

* jcr:content/metadata/cq:tags
* jcr:content/metadata/dc:format
* jcr:content/metadata/dam:status
* jcr：content/metadata/videoCodec
* jcr：content/metadata/AudioCodec
* jcr：content/metadata/dc：title
* jcr：content/metadata/dc：description
* jcr：content/metadata/xmpMM：socialID
* jcr：content/metadata/xmpMM：DocumentID
* jcr：content/metadata/dam：sha1
* jcr：content/metadata/dam：解决方案Context
* jcr：content/metadata/videoItate
* jcr：content/metadata/audiobitRate
* jcr：content/uses/usedby
* jcr:content/jcr:lastModified
* jcr:content/metadata/prism:expirationDate
* jcr：content/onTime
* jcr：content/offtime
* jcr:content/metadata/dam:size
* jcr：content/metadata/tiff：imageWidth
* jcr：content/metadata/tiff：ImageLength
