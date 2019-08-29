---
title: 应用图像预设或动态演绎版
seo-title: 应用图像预设或动态演绎版
description: '像宏一样，图像预设是一组预定义的大小调整和格式设置命令，保存在名称下。利用图像预设，AEM Assets Brand Portal能够动态地提供不同大小、格式和属性的图像。 '
seo-description: '像宏一样，图像预设是一组预定义的大小调整和格式设置命令，保存在名称下。利用图像预设，AEM Assets Brand Portal能够动态地提供不同大小、格式和属性的图像。 '
uuid: a3c8705c-5fbd-472c-8b61-f65 b3 e552 c1 b
content-type: 引用
topic-tags: administration
products: SG_ EXPERIENCE MANAGER/Brand_ Portal
discoiquuid: a512dfa0-fef3-4c3 f-a389-a0 a3 a7415 bac
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# 应用图像预设或动态演绎版 {#apply-image-presets-or-dynamic-renditions}

Like a macro, an image preset is a predefined [!UICONTROL collection] of sizing and formatting commands saved under a name. 图像预设使 [!DNL AEM] 资产 [!DNL Brand Portal] 能够动态地传送不同大小、格式和属性的图像。

图像预设用于生成可预览和下载的图像的动态演绎版。预览图像及其演绎版时，您可以选择预设，以将图像重新设置为管理员设置的规范。

要查看其中 [!DNL Brand Portal]某个资产的动态演绎版，请确保其PIFF再现存在 [!DNL AEM] 于您发布到 [!DNL Brand Portal]的创作实例中。当您发布资产时，其PTIFF演绎版也会发布到 [!DNL Brand Portal]。无法从中生成PTIFF演绎版 [!DNL Brand Portal]。

>[!NOTE]
>
>下载图像及其再现时，没有可从现有预设中进行选择的选项。您可以指定自定义图像预设的属性。有关更多信息，请参阅 [在下载图像](../using/brand-portal-image-presets.md#main-pars-text-1403412644)时应用图像预设。

有关创建图像预设时所需参数的更多信息，请参阅 [管理图像预设](https://docs.adobe.com/docs/en//6-0/administer/integration/dynamic-media/image-presets.html)[!DNL AEM]。

## Create an image preset {#create-an-image-preset}

管理员可以创建在资产详细信息页面上显示为动态演绎版的图像预设。您可以从头开始创建图像预设，也可以保存现有的图像预设。创建图像预设时，请选择图像传送大小和格式命令。传送图像以供查看时，会根据所选命令优化其外观。
请注意，只有管理员才能在 [!DNL Brand Portal]中创建图像预设。

请注意，只有管理员才能在 [!DNL Brand Portal]中创建图像预设。

>[!NOTE]
>
>为提供PTIFF的资产创建动态演绎版。因此，如果资产没有在上 [!DNL AEM] 创建和发布的Presid TIFF演绎版， [!DNL Brand Portal]则只能导出其系统再现，但动态演绎版会作为选项呈现。
必须启用Dynamic Media混合模式( [!DNL AEM] 作者)才能创建资产的中间tiff(ptiff)。将此类资产发布到 [!DNL Brand Portal]后，将应用图像预设并显示动态演绎版。

1. 在顶部的 [!DNL AEM] 工具栏中，单击Adobe徽标以访问管理工具。

   !![](assets/[!DNL AEM]logo. png)

2. 从管理工具面板中，单击 **图像预设**。

   ![](assets/admin-tools-panel-4.png)

3. 在图像预设页面中，单击 **创建**。

   ![](assets/image_preset_homepage.png)

4. 在 **编辑图像预设** 页面中，根据需要为 **基本** 和 **高级** 选项卡输入值，包括名称。这些选项在 [图像预设选项](https://docs.adobe.com/docs/en//6-0/administer/integration/dynamic-media/image-presets.html#Image%20preset%20options)[!DNL AEM]中提供。各项预设将出现在左侧窗格中，并且可以快速用于其他资产。

   ![](assets/image_preset_create.png)

   >[!NOTE]
   >
   >您还可以使用 **“编辑图像预设** ”页面编辑现有图像预设的属性。要编辑图像预设，请从图像预设页面中选择该预设，然后单击 **编辑**。

5. 单击&#x200B;**保存**。图像预设会在图像预设页面上创建并显示。
6. 要删除图像预设，请从图像预设页面中选择该预设，然后单击 **“删除**”。在确认页面中，单击 **删除** 以确认删除。图像预设将从图像预设页面中删除。

## 预览图像时应用图像预设 {#apply-image-presets-when-previewing-images}

预览图像及其再现时，请从现有预设中进行选择，以将图像重新设置为管理员设置的规范。

1. 在 [!DNL Brand Portal] 界面中，单击图像以将其打开。
2. 单击左侧的叠加图标，然后选择 **演绎版**。

   ![](assets/image-preset-previewrenditions.png)

3. 从 **演绎版** 列表中，选择适当的动态演绎版，例如 **缩略图**。预览图像将根据您选择的演绎版进行渲染。

   ![](assets/image-preset-previewrenditionthumbnail.png)

## 下载图像时应用图像预设 {#apply-image-presets-when-downloading-images}

从中下载图像及其再现时，您无法 [!DNL Brand Portal]从现有的图像预设中进行选择。但是，您可以根据要对图像重新设置格式的图像预设属性进行自定义。

1. 在 [!DNL Brand Portal] 界面中，执行下列操作之一：

   * 将鼠标指针悬停在要下载的图像上。从可用的快速操作缩略图中，单击 **下载** 图标。
   ![](assets/downloadsingleasset.png)

   * 选择要下载的图像。从顶部的工具栏中，单击 **下载** 图标。
   ![](assets/downloadassets.png)

2. 从 **“下载** ”对话框中，选择所需的选项，具体取决于您是否要使用或不带演绎版下载资产。

   ![](assets/donload-assets-dialog.png)

3. 要下载资产的动态演绎版，请选择 **“动态演绎版”** 选项。
4. 自定义图像预设属性，以便在下载过程中动态重新格式化图像及其演绎版。指定大小、格式、颜色空间、分辨率和图像修饰符。

   ![](assets/dynamicrenditions.png)

5. 单击 **“下载**”。自定义动态演绎版将下载到ZIP文件中，以及您选择下载的图像和演绎版。但是，如果下载单个资源，则不会创建zip文件，这可以确保快速下载。