---
title: 应用图像预设或动态演绎版
seo-title: Apply image presets or dynamic renditions
description: 与宏一样，图像预设是预先定义的名称下保存的大小和格式设置命令集合。 图像预设使Experience Manager Assets Brand Portal能够动态交付不同大小、格式和属性的图像。
seo-description: Like a macro, an image preset is a predefined collection of sizing and formatting commands saved under a name. Image presets enable Experience Manager Assets Brand Portal to dynamically deliver images of different sizes, formats, and properties.
uuid: a3c8705c-5fbd-472c-8b61-f65b3e552c1b
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: a512dfa0-fef3-4c3f-a389-a0a3a7415bac
role: Admin
exl-id: 212a1b3a-686f-4250-be06-b679b6039887
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '814'
ht-degree: 3%

---

# 应用图像预设或动态演绎版 {#apply-image-presets-or-dynamic-renditions}

与宏一样，图像预设是预先定义的名称下保存的大小和格式设置命令集合。 图像预设使Experience Manager Assets Brand Portal能够动态交付不同大小、格式和属性的图像。

图像预设用于生成可预览和下载的图像动态演绎版。 在预览图像及其演绎版时，您可以选择预设，根据管理员设置的规范重新格式化图像。

(*如果Experience Manager Assets创作实例正在运行&#x200B;**Dynamic Media混合模式***)要在Brand Portal中查看资源的动态演绎版，请确保其金字塔tiff演绎版存在于您发布到Brand Portal的Experience Manager Assets创作实例中。 发布资源时，也会将资源的PTIFF演绎版发布到Brand Portal。

>[!NOTE]
>
>在下载图像及其演绎版时，没有选项可以从现有预设中进行选择。 相反，您可以指定自定义图像预设的属性。 有关更多信息，请参阅 [下载图像时应用图像预设](../using/brand-portal-image-presets.md#main-pars-text-1403412644).


有关创建图像预设时所需的参数的更多信息，请参阅 [管理图像预设](../using/brand-portal-image-presets.md).

## 创建图像预设 {#create-an-image-preset}

Experience Manager Assets管理员可以创建在资源详细信息页面上显示为动态演绎版的图像预设。 您可以从头开始创建图像预设，也可以使用新名称保存现有图像预设。 创建图像预设时，请选择用于图像投放的大小和格式设置命令。 当传送图像供查看时，根据选择的命令优化其外观。

>[!NOTE]
>
>图像的动态演绎版使用其金字塔TIFF创建。 如果金字塔TIFF不适用于任何资源，则无法在Brand Portal中获取该资源的动态演绎版。
>
>如果Experience Manager Assets创作实例正在运行 **Dynamic Media混合模式**&#x200B;之后，将创建图像资源的金字塔TIFF演绎版并将其保存在Experience Manager Assets存储库中。
>
>但是，如果Experience Manager Assets创作实例正在运行 **Dynamic Media Scene 7模式**，则图像资源的金字塔TIFF演绎版存在于Scene 7服务器上。
>
>将此类资产发布到Brand Portal时，会应用图像预设并显示动态演绎版。


1. 在顶部的工具栏中，单击Experience Manager徽标以访问管理工具。

1. 在管理工具面板中，单击 **[!UICONTROL 图像预设]**.

   ![](assets/admin-tools-panel-4.png)

1. 在图像预设页面中，单击 **[!UICONTROL 创建]**.

   ![](assets/image_preset_homepage.png)

1. 在 **[!UICONTROL 编辑图像预设]** 页面中，将值输入到 **[!UICONTROL 基本]** 和 **[!UICONTROL 高级]** 选项卡，包括名称。 预设显示在左窗格中，并可以与其他资产一起动态使用。

   ![](assets/image_preset_create.png)

   >[!NOTE]
   >
   >您还可以使用 **[!UICONTROL 编辑图像预设]** 页面，以编辑现有图像预设的属性。 要编辑图像预设，请从图像预设页面中选择它，然后单击 **[!UICONTROL 编辑]**.

1. 单击“**[!UICONTROL 保存]**”。图像预设随即创建并显示在图像预设页面上。
1. 要删除图像预设，请从图像预设页面中选择它，然后单击 **[!UICONTROL 删除]**. 在确认页面中，单击 **[!UICONTROL 删除]** 以确认删除。 图像预设将从图像预设页面中删除。

## 预览图像时应用图像预设  {#apply-image-presets-when-previewing-images}

预览图像及其演绎版时，从现有预设中选择，以将图像重新格式化为管理员设置的规范。

1. 在Brand Portal界面中，单击图像以将其打开。
1. 单击左侧的叠加图标，然后选择 **[!UICONTROL 演绎版]**.

   ![](assets/image-preset-previewrenditions.png)

1. 从 **[!UICONTROL 演绎版]** 列表中，选择相应的动态演绎版，例如， **[!UICONTROL 缩略图]**. 预览图像会根据您选择的演绎版进行渲染。

   ![](assets/image-preset-previewrenditionthumbnail.png)

## 下载图像时应用图像预设 {#apply-image-presets-when-downloading-images}

从Brand Portal下载图像及其演绎版时，无法从现有图像预设中进行选择。 但是，您可以根据要重新设置图像格式的位置来自定义图像预设属性。

1. 在Brand Portal界面中，执行以下操作之一：

   * 将指针悬停在要下载的图像上。 在可用的快速操作缩略图中，单击 **[!UICONTROL 下载]** 图标。

   ![](assets/downloadsingleasset.png)

   * 选择要下载的图像。 在顶部的工具栏中，单击 **[!UICONTROL 下载]** 图标。

   ![](assets/downloadassets.png)

1. 从 **[!UICONTROL 下载]** 对话框，请根据您想要下载带有还是不带其演绎版的资源，选择所需的选项。

   ![](assets/donload-assets-dialog.png)

1. 要下载资源的动态演绎版，请选择 **[!UICONTROL 动态演绎版]** 选项。
1. 根据您要在下载期间动态重新格式化图像及其演绎版的方式，自定义图像预设属性。 指定大小、格式、颜色空间、分辨率和图像修饰符。

   ![](assets/dynamicrenditions.png)

1. 单击&#x200B;**[!UICONTROL 下载]**。自定义动态演绎版以及您选择下载的图像和演绎版下载为ZIP文件。 但是，如果下载了单个资产，则不会创建zip文件，这可以确保快速下载。
