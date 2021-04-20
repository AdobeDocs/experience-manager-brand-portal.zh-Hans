---
title: 应用图像预设或动态演绎版
seo-title: 应用图像预设或动态演绎版
description: '与宏一样，图像预设是一组预定义的大小调整和格式设置命令，这些命令以名称保存。 图像预设使AEM Assets Brand Portal能够动态传送不同大小、格式和属性的图像。 '
seo-description: '与宏一样，图像预设是一组预定义的大小调整和格式设置命令，这些命令以名称保存。 图像预设使AEM Assets Brand Portal能够动态传送不同大小、格式和属性的图像。 '
uuid: a3c8705c-5fbd-472c-8b61-f65b3e552c1b
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: a512dfa0-fef3-4c3f-a389-a0a3a7415bac
role: Administrator
translation-type: tm+mt
source-git-commit: 263653916e4bc183827c197c3beb137c9e59ccb1
workflow-type: tm+mt
source-wordcount: '872'
ht-degree: 4%

---


# 应用图像预设或动态演绎版 {#apply-image-presets-or-dynamic-renditions}

与宏一样，图像预设是一组预定义的大小调整和格式设置命令，这些命令以名称保存。 图像预设使AEM Assets Brand Portal能够动态传送不同大小、格式和属性的图像。

图像预设用于生成可预览和下载的图像的动态演绎版。 在预览图像及其演绎版时，您可以选择预设来根据管理员设置的规范重新设置图像的格式。

(*如果AEM作者实例在&#x200B;**Dynamic Media Hybrid mode***上运行)要在Brand Portal中视图资产的动态演绎版，请确保其Pyramid tiff再现存在于从中发布到Brand Portal的AEM作者实例中。 在您发布资产时，其PTIFF演绎版也会发布到Brand Portal。

>[!NOTE]
>
>下载图像及其演绎版时，无法从现有预设中进行选择。 您可以指定自定义图像预设的属性。 有关详细信息，请参阅[下载图像时应用图像预设](../using/brand-portal-image-presets.md#main-pars-text-1403412644)。


有关创建图像预设时所需参数的详细信息，请参阅[管理图像预设](https://docs.adobe.com/docs/en/AEM/6-0/administer/integration/dynamic-media/image-presets.html)。

## 创建图像预设{#create-an-image-preset}

AEM管理员可以创建图像预设，这些预设在资产详细信息页面上显示为动态演绎版。 您可以从头开始创建图像预设，也可以使用新名称保存现有图像预设。 创建图像预设时，请选择图像投放的大小和格式命令。 传送图像以供查看时，会根据所选命令优化其外观。

>[!NOTE]
>
>图像的动态演绎版是使用其金字塔TIFF创建的。 如果金字塔TIFF不适用于任何资产，则无法在Brand门户中获取该资产的动态演绎版。
>
>如果AEM作者实例在&#x200B;**Dynamic Media Hybrid mode**&#x200B;上运行，则会创建图像资产的金字塔TIFF演绎版并将其保存在AEM存储库中。
>
>但是，如果AEM作者实例在&#x200B;**Dynamic Media Scene 7 mode**&#x200B;上运行，则Scene 7服务器上存在图像资产的Pyramid TIFF演绎版。
>
>当此类资产发布到品牌门户时，会应用图像预设并显示动态演绎版。


1. 从顶部的AEM工具栏中，单击Adobe徽标以访问管理工具。

1. 在管理工具面板中，单击&#x200B;**[!UICONTROL 图像预设]**。

   ![](assets/admin-tools-panel-4.png)

1. 在图像预设页面中，单击&#x200B;**[!UICONTROL 创建]**。

   ![](assets/image_preset_homepage.png)

1. 在&#x200B;**[!UICONTROL 编辑图像预设]**&#x200B;页面中，根据需要在&#x200B;**[!UICONTROL 基本]**&#x200B;和&#x200B;**[!UICONTROL 高级]**&#x200B;选项卡中输入值，包括名称。 有关各个选项的概述，请参阅[图像预设选项](https://docs.adobe.com/docs/en/AEM/6-0/administer/integration/dynamic-media/image-presets.html#Image%20preset%20options)。预设显示在左窗格中，并可以与其他资产一起动态使用。

   ![](assets/image_preset_create.png)

   >[!NOTE]
   >
   >您还可以使用&#x200B;**[!UICONTROL 编辑图像预设]**&#x200B;页面编辑现有图像预设的属性。 要编辑图像预设，请从图像预设页面中选择它，然后单击&#x200B;**[!UICONTROL 编辑]**。

1. 单击&#x200B;**[!UICONTROL 保存]**。此时会创建图像预设并在图像预设页面上显示。
1. 要删除图像预设，请从图像预设页面中选择它，然后单击&#x200B;**[!UICONTROL 删除]**。 在确认页中，单击&#x200B;**[!UICONTROL 删除]**&#x200B;以确认删除。 图像预设将从图像预设页面中删除。

## 在预览图像{#apply-image-presets-when-previewing-images}时应用图像预设

在预览图像及其演绎版时，从现有预设中进行选择，以根据管理员设置的规范重新设置图像格式。

1. 从Brand Portal界面中，单击图像以将其打开。
1. 单击左侧的叠加图标，然后选择&#x200B;**[!UICONTROL 演绎版]**。

   ![](assets/image-preset-previewrenditions.png)

1. 从&#x200B;**[!UICONTROL 演绎版]**&#x200B;列表中，选择适当的动态演绎版，例如&#x200B;**[!UICONTROL 缩略图]**。 预览图像将根据您选择的再现进行渲染。

   ![](assets/image-preset-previewrenditionthumbnail.png)

## 下载图像{#apply-image-presets-when-downloading-images}时应用图像预设

从Brand Portal下载图像及其演绎版时，无法从现有图像预设中进行选择。 但是，您可以根据要重新设置图像格式的属性来自定义图像预设属性。

1. 从Brand Portal界面中，执行以下操作之一：

   * 将指针悬停在要下载的图像上。 从可用的快速操作缩略图中，单击&#x200B;**[!UICONTROL 下载]**&#x200B;图标。

   ![](assets/downloadsingleasset.png)

   * 选择要下载的图像。 在顶部的工具栏中，单击&#x200B;**[!UICONTROL 下载]**&#x200B;图标。

   ![](assets/downloadassets.png)

1. 从&#x200B;**[!UICONTROL 下载]**&#x200B;对话框中，根据是否要下载包含或不包含其演绎版的资产，选择所需的选项。

   ![](assets/donload-assets-dialog.png)

1. 要下载资产的动态演绎版，请选择&#x200B;**[!UICONTROL 动态演绎版]**&#x200B;选项。
1. 自定义图像预设属性，您可以在下载过程中根据这些属性动态地重新设置图像及其演绎版的格式。 指定大小、格式、色彩空间、分辨率和图像修饰符。

   ![](assets/dynamicrenditions.png)

1. 单击&#x200B;**[!UICONTROL 下载]**。 自定义动态演绎版将与您选择下载的图像和演绎版一起下载到ZIP文件中。 但是，如果下载了单个资源，则不会创建zip文件，这可确保快速下载。
