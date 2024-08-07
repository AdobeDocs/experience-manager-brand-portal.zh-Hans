---
title: 加快Brand Portal下载速度
description: 增强从Brand Portal和共享链接下载的性能。
contentOwner: Vishabh Gupta
topic-tags: download-install, download assets
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
exl-id: cf28df58-c6dd-4b12-8279-01351892009f
source-git-commit: f931f6576c05d82cea61bda00322425abc9e8d43
workflow-type: tm+mt
source-wordcount: '1009'
ht-degree: 3%

---

# 加快Brand Portal下载速度 {#guide-to-accelerate-downloads-from-brand-portal}

<!-- This topic is woefully out of date. It talks at length about using a third party application whose URLs have a variety of problems. Topic should either be deleted or updated entirely to not talk about a specific third party application that Adobe has no control over. It also appears that the third party app is NOT free anymore. -->

Adobe Experience Manager Assets Brand Portal允许通过与IBM® Aspera Connect（按需安装应用程序）集成来增强大型资源文件的下载性能。 该应用程序使用专有技术消除TCP开销，并帮助提高资产文件的传输速度。 此集成确保增强的下载体验。

>[!NOTE]
>
>下载速度因用户而异，因为它取决于网络带宽、服务器延迟和客户端的地理位置等因素。

默认情况下，**[!UICONTROL 快速下载]**&#x200B;配置处于启用状态，这可以显着减少从Brand Portal下载所需资源文件所需的时间。

![](assets/download-settings-new.png)

## 加速文件下载的先决条件 {#prerequisites-to-accelerate-file-download}

要更快地下载文件，请确保满足以下条件：

* 导航到&#x200B;**[!UICONTROL 工具]** > **[!UICONTROL 下载]**，并验证&#x200B;**[!UICONTROL 下载设置]**&#x200B;中是否启用了&#x200B;**[!UICONTROL 快速下载]**&#x200B;配置。
* 确保在防火墙上打开端口33001（TCP和UDP）。
* 使用管理员权限([IBM® Aspera Connect下载](https://www.ibm.com/support/fixcentral/swg/selectFixes?parent=ibm%7EOther%20software&amp;product=ibm/Other+software/IBM+Aspera+Connect&amp;release=3.9.9&amp;platform=All&amp;function=all))在浏览器的扩展中安装IBM® Aspera Connect 3.9.9 **。**

>[!NOTE]
>
>IBM® Aspera Connect存在已知问题。 快速下载不适用于IBM® Aspera Connect版本3.10及更高版本。

## 下载域 {#download-domains}

以下是不同地理位置的下载域：

| 区域代码 | 域 |
|---|---|
| NA或1 | downloads-na1.brand-portal.adobe.com |
| NA VA5 | downloads-na2.brand-portal.adobe.com |
| 欧洲、中东和非洲地区LON5 | downloads-emea1.brand-portal.adobe.com |
| APAC SIN2 | downloads-apac1.brand-portal.adobe.com |

## 使用文件加速器的示例下载性能 {#expected-download-performance-using-file-accelerator}

下表显示了使用Aspera Connect文件下载加速器下载2 GB文件的性能：

*考虑到Brand Portal服务器位于俄勒冈州（美国），由于网络带宽、服务器延迟和客户端位置等因素，观察到的结果会有所不同。*

| 客户端位置 | 客户端与服务器之间的延迟（毫秒） | Aspera Connect File Transfer Accelerator (MBps)的速度 | 使用Aspera File Transfer Accelerator下载2 GB的文件所需的时间（秒） |
|---------------------------|-----------------------------------|---------------------------------------------|-------------------------------------------------------------------------|
| 美国西部（北加利福尼亚） | 18 | 36 | 57 |
| 美国西部（俄勒冈州） | 42 | 36 | 57 |
| 美国东部（北弗吉尼亚州） | 85 | 35 | 58 |
| APAC （东京） | 124 | 36 | 57 |
| 诺伊达（印度） | 275 | 13.36 | 153 |
| 悉尼 | 175 | 29 | 70 |
| 伦敦 | 179 | 35 | 58 |
| 新加坡 | 196 | 34 | 60 |

## 下载资源 {#download-assets}

要更快地从Brand Portal下载资源，请执行以下操作：

1. 登录到您的Brand Portal租户。 默认情况下，**[!UICONTROL 文件]**&#x200B;视图打开，其中包含所有已发布的资源和文件夹。

   执行下列操作之一：

   * 选择要下载的资源或文件夹。 从顶部的工具栏中，单击&#x200B;**[!UICONTROL 下载]**&#x200B;图标。

     ![选择多个资源](assets/select-assets-new.png)

   * 要下载资源的特定资源演绎版，请将指针悬停在资源上，然后单击快速操作缩略图中显示的&#x200B;**[!UICONTROL 下载]**&#x200B;图标。

     ![select-asset](assets/select-asset.png)

1. 将打开列出所有选定资产的&#x200B;**[!UICONTROL 下载]**&#x200B;对话框。

   要在下载资源时保留Brand Portal文件夹层次结构，请选中&#x200B;**[!UICONTROL `Create separate folder for each asset`]**&#x200B;复选框。

   下载按钮反映选定项目的计数。 应用完规则后，单击&#x200B;**[!UICONTROL 下载项目]**。 要了解有关如何应用规则的更多信息，请参阅[下载资源](../using/brand-portal-download-assets.md#download-assets)。

   ![下载对话框](assets/download-dialog-box-new.png)

1. 默认情况下，**[!UICONTROL 下载设置]**&#x200B;中启用了&#x200B;**[!UICONTROL 快速下载]**&#x200B;设置。 因此，会显示一个确认框，用于使用IBM® Aspera Connect下载资源。

   如果您是首次下载资源，并且浏览器中未安装IBM® Aspera Connect，则会提示您安装它。 如果现有版本已过期，系统还会提示您安装[Aspera下载加速器](https://www.ibm.com/support/fixcentral/swg/selectFixes?parent=ibm%7EOther%20software&amp;product=ibm/Other+software/IBM+Aspera+Connect&amp;release=3.9.9&amp;platform=All&amp;function=all)。

   ![](assets/aspera-not-launched.png)

1. **安装Aspera Connect客户端**

   要安装IBM® Aspera Connect客户端安装程序，请从IBM® Aspera Connect客户端应用程序的.msi文件运行安装程序，然后按照安装向导进行操作。

   ![](assets/aspera-download-1.png)

1. 成功安装客户端后，请刷新浏览器页面并再次启动下载步骤。

1. 若要继续使用&#x200B;**[!UICONTROL 快速下载]**，请单击&#x200B;**[!UICONTROL 允许]**。 使用IBM® Aspera Connect将所有选定的呈现版本下载到zip文件夹中。

   成功完成下载后，将会显示一个对话框，其中显示了将资产下载到用户系统的位置。

   ![](assets/aspera-download-2.png)

   如果您不想使用IBM® Aspera Connect，请单击&#x200B;**[!UICONTROL 拒绝]**。 如果&#x200B;**[!UICONTROL 快速下载]**&#x200B;被拒绝或失败，则系统填充错误消息。 单击&#x200B;**[!UICONTROL 正常下载]**&#x200B;按钮继续下载资产。

>[!NOTE]
>
>如果管理员关闭了&#x200B;**[!UICONTROL 快速下载]**&#x200B;设置，则所选格式副本将直接下载到zip文件夹中，而无需使用IBM® Aspera Connect。

<!-- 
On successful completion of the download, a dialog box shows the location where assets are downloaded onto the user's system. If there is a failure, it shows error.

   >[!NOTE]
   >
   >There is a known limitation in Aspera Connect client application that no prompt to select download location appears if **[!UICONTROL Always ask me where to save downloaded files]** is enabled under the tab **[!UICONTROL Transfers]** within **[!UICONTROL Preferences]**. Before any download begins, provide the location in the text box **[!UICONTROL Save downloaded files to]**.


1. Log in to Brand Portal using a supported browser.
1. Browse and select the folders or assets you want to download. From the toolbar at the top, click the **[!UICONTROL Download]** icon. the **[!UICONTROL Download]** dialog appears with the **[!UICONTROL Asset(s)]** and **[!UICONTROL Enable download acceleration]** check boxes selected by default. 

   ![](assets/download-assetsbp.png)

   >[!NOTE]
   >
   >The functionality to send email notification with the link to download assets is presently not supported while faster downloads are enabled.

   ![](assets/fast-download-emailchk.png)

1. Click **[!UICONTROL Download]**.

   To speed up the download experience on your Brand Portal tenant account, you need to have Aspera Connect client application installed in your browser's extension.

1. **Download Aspera Connect Client**

   If Aspera Connect client is not installed on your system or the existing Aspera Connect client is out of date, a prompt is displayed on the browser page from where you can download the system-specific Aspera Connect client by selecting **[!UICONTROL Download Latest Version]**.

   ![](assets/aspera-not-launched.png)

   To download the latest version of Aspera Connect from [https://downloads.asperasoft.com/connect2/](https://downloads.asperasoft.com/connect2/), select **[!UICONTROL Download Now]** and follow the instructions.

1. **Install Aspera Connect Client**

   To install IBM Aspera Connect client setup, run the setup from  .msi  file of IBM Aspera Connect client application and follow the installation wizard.

1. Once the client is successfully installed, refresh the browser page and initiate the download steps again.

   When using Aspera Connect for the first time, the browser prompts to open the link using **[!UICONTROL IBM Aspera Connect]**. To skip this dialog in future, enable **[!UICONTROL Remember my choice for FASP links]**.

   >[!NOTE]
   >
   >This message is different on the different browsers.

1. A dialog box confirms whether to proceed the transfer or not. Select **[!UICONTROL Allow]** to begin.
To skip this dialog in future, enable **[!UICONTROL Use my choice for all connections with this host]**.
Download begins. A dialog box shows the progress of the download. Use the dialog box to **[!UICONTROL pause]**, **[!UICONTROL resume]**, or **[!UICONTROL cancel]** the download.
Aspera Connect application provides an Activity Window on the system where user can view and manage all transfer sessions. For more information, refer [Aspera Connect Client documentation](https://downloads.asperasoft.com/en/documentation/8).

![](assets/aspera-activity-window.png)

On successful completion of the download, a dialog box shows the location where assets are downloaded onto the user's system. If there is a failure, it shows error.

   >[!NOTE]
   >
   >There is a known limitation in Aspera Connect client application that no prompt to select download location appears if **[!UICONTROL Always ask me where to save downloaded files]** is enabled under the tab **[!UICONTROL Transfers]** within **[!UICONTROL Preferences]**. Before any download begins, provide the location in the text box **[!UICONTROL Save downloaded files to]**.
-->

## 在Microsoft® Edge浏览器上使用文件加速器 {#using-file-accelerator-on-microsoft-edge-browser}

Microsoft® Edge在增强保护模式(EPM)下运行，以防止在同一个专用网络或受信任站点上与Aspera Connect服务器通信。 因此，每次建立与服务器的连接时都会出现一个弹出窗口。

![](assets/switchapps-msedge.png)

要在Microsoft® Edge上使用加速下载功能，请从“受信任的站点”列表中删除Brand Portal站点。

1. 打开控制面板(**[!UICONTROL 窗口键+ X]**，然后选择&#x200B;**[!UICONTROL 控制面板]**)。
1. 转到&#x200B;**[!UICONTROL 网络和互联网]** > **[!UICONTROL 互联网选项]**。 单击&#x200B;**[!UICONTROL 安全]**&#x200B;选项卡。
1. 单击&#x200B;**[!UICONTROL 受信任的站点区域]**，然后单击&#x200B;**[!UICONTROL 站点]**。
1. 从列表中删除Brand Portal站点。

## Aspera Connect客户端首选项 {#aspera-connect-client-preferences}

在IBM® Aspera Connect客户端首选项中，可通过右键单击图标并选择&#x200B;**[!UICONTROL 首选项]**&#x200B;来设置一些有用的首选项。

![](assets/download_assets_frombrandportalimg19.png)

您可以设置默认下载位置。

![](assets/aspera-preferences.png)

此外，可以标记Aspera Connect客户端，使其在系统启动时自动启动。 并且，Connect客户端将运行并可供下载，从而更快地开始下载。

![](assets/aspera-automaticallylaunch.png)

## 下载加速问题疑难解答 {#troubleshoot-issues-with-download-acceleration}

如果下载加速不适合您，请尝试以下建议：

1. 检查端口是否未被阻止。 使用Google Search查找选项，这些选项允许您根据使用的操作系统检查端口是否受阻。 <!-- THIS URL IS 404 AND DOES NOT REDIRECT [https://test-connect.asperasoft.com](https://test-connect.asperasoft.com/) from your computer. -->

   如果端口不能正常工作，请与网络团队联系，并确保端口33001（TCP和UDP）在防火墙中未被阻止。

1. 如果端口正常，则使用[https://www.speedtest.net/](https://www.speedtest.net/)测量可用带宽，检查网络是否运行不慢。

   如果带宽为几个(1-10 Mbps)或以Kbps为单位，则使用Aspera首选项并尝试将带宽限制为等于可用带宽。

   <!-- The URL in this step is giving a 404 error. 1. To confirm whether the downloads from Aspera demo server are working, use [https://demo.asperasoft.com/aspera/user](https://demo.asperasoft.com/aspera/user).  
   (login:  asperaweb , password:  demoaspera ) -->

1. 如果上述故障诊断步骤均无效，请取消选择启用下载加速选项并使用普通下载。
