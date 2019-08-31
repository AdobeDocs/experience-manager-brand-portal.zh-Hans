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
source-git-commit: c0169450c5cf1d8c99f8604df3bd2667445ff1ed

---


# 应用图像预设或动态演绎版 {#apply-image-presets-or-dynamic-renditions}

像宏一样，图像预设是一组预定义的大小调整和格式设置命令，保存在名称下。利用图像预设，AEM Assets Brand Portal能够动态地提供不同大小、格式和属性的图像。

图像预设用于生成可预览和下载的图像的动态演绎版。预览图像及其演绎版时，您可以选择预设，以将图像重新设置为管理员设置的规范。

要在Brand Portal中查看资产的动态演绎版，请确保其中间的tifid tiff再现存在于您发布到Brand Portal的AEM作者实例中。发布资产时，其PIFF演绎版也会发布到Brand Portal。无法从Brand Portal生成PIFF再现。

>[!NOTE]
>
>下载图像及其再现时，没有可从现有预设中进行选择的选项。您可以指定自定义图像预设的属性。有关更多信息，请参阅 [在下载图像](../using/brand-portal-image-presets.md#main-pars-text-1403412644)时应用图像预设。

有关创建图像预设时所需参数的更多信息，请参阅 [管理图像预设](https://docs.adobe.com/docs/en/AEM/6-0/administer/integration/dynamic-media/image-presets.html)。

## Create an image preset {#create-an-image-preset}

管理员可以创建在资产详细信息页面上显示为动态演绎版的图像预设。您可以从头开始创建图像预设，也可以保存现有的图像预设。创建图像预设时，请选择图像传送大小和格式命令。传送图像以供查看时，会根据所选命令优化其外观。
请注意，只有管理员才能在Brand Portal中创建图像预设。

请注意，只有管理员才能在Brand Portal中创建图像预设。

>[!NOTE]
>
>为提供PTIFF的资产创建动态演绎版。因此，如果资产没有在AEM上创建的Presid TIFF演绎版并将其发布到Brand Portal，则只能导出其系统再现，但动态演绎版会作为一个选项呈现。
必须在AEM(作者)上启用Dynamic Media混合模式才能创建资产的中间tiff(ptiff)。将此类资产发布到Brand Portal时，将应用图像预设并显示动态演绎版。

1. 在顶部的AEM工具栏中，单击Adobe徽标以访问管理工具。

2. 从管理工具面板中，单击 **[!UICONTROL 图像预设]**。

   ![](assets/admin-tools-panel-4.png)

3. 在图像预设页面中，单击 **[!UICONTROL 创建]**。

   ![](assets/image_preset_homepage.png)

4. 在 **[!UICONTROL 编辑图像预设]** 页面中，根据需要为 **[!UICONTROL 基本]** 和 **[!UICONTROL 高级]** 选项卡输入值，包括名称。有关各个选项的概述，请参阅[图像预设选项](https://docs.adobe.com/docs/en/AEM/6-0/administer/integration/dynamic-media/image-presets.html#Image%20preset%20options)。各项预设将出现在左侧窗格中，并且可以快速用于其他资产。

   ![](assets/image_preset_create.png)

   >[!NOTE]
   >
   >您还可以使用 **[!UICONTROL “编辑图像预设]** ”页面编辑现有图像预设的属性。要编辑图像预设，请从图像预设页面中选择该预设，然后单击 **[!UICONTROL 编辑]**。

5. Click **[!UICONTROL Save]**. 图像预设会在图像预设页面上创建并显示。
6. 要删除图像预设，请从图像预设页面中选择该预设，然后单击 **[!UICONTROL “删除]**”。在确认页面中，单击 **[!UICONTROL 删除]** 以确认删除。图像预设将从图像预设页面中删除。

## 预览图像时应用图像预设 {#apply-image-presets-when-previewing-images}

预览图像及其再现时，请从现有预设中进行选择，以将图像重新设置为管理员设置的规范。

1. 从Brand Portal界面中，单击图像以将其打开。
2. 单击左侧的叠加图标，然后选择 **[!UICONTROL 演绎版]**。

   ![](assets/image-preset-previewrenditions.png)

3. 从 **[!UICONTROL 演绎版]** 列表中，选择适当的动态演绎版，例如 **[!UICONTROL 缩略图]**。预览图像将根据您选择的演绎版进行渲染。

   ![](assets/image-preset-previewrenditionthumbnail.png)

## 下载图像时应用图像预设 {#apply-image-presets-when-downloading-images}

从Brand Portal下载图像及其再现时，您无法从现有图像预设中进行选择。但是，您可以根据要对图像重新设置格式的图像预设属性进行自定义。

1. 在Brand Portal界面中，执行下列操作之一：

   * 将鼠标指针悬停在要下载的图像上。从可用的快速操作缩略图中，单击 **[!UICONTROL 下载]** 图标。
   ![](assets/downloadsingleasset.png)

   * 选择要下载的图像。从顶部的工具栏中，单击 **[!UICONTROL 下载]** 图标。
   ![](assets/downloadassets.png)

2. 从 **[!UICONTROL “下载]** ”对话框中，选择所需的选项，具体取决于您是否要使用或不带演绎版下载资产。

   ![](assets/donload-assets-dialog.png)

3. 要下载资产的动态演绎版，请选择 **[!UICONTROL “动态演绎版”]** 选项。
4. 自定义图像预设属性，以便在下载过程中动态重新格式化图像及其演绎版。指定大小、格式、颜色空间、分辨率和图像修饰符。

   ![](assets/dynamicrenditions.png)

5. 单击 **[!UICONTROL “下载]**”。自定义动态演绎版将下载到ZIP文件中，以及您选择下载的图像和演绎版。但是，如果下载单个资源，则不会创建zip文件，这可以确保快速下载。
