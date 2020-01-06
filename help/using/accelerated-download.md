---
title: 加快Brand Portal下载
seo-title: 加快Brand Portal下载
description: 增强从Brand Portal和共享链接的下载性能。
seo-description: 增强从Brand Portal和共享链接的下载性能。
uuid: 2871137e-6471-49a7-872a-841bd92543d1
contentOwner: mgulati
topic-tags: download-install
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 301f7a0b-5527-4aac-b731-bfc145fed0c0
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873

---


# 加快Brand Portal下载 {#guide-to-accelerate-downloads-from-brand-portal}

Brand Portal通过与IBM Aspera connect集成来增强大型资产文件的下载性能，后者是一个按需安装的应用程序。 该应用程序使用专有技术来消除TCP开销并帮助提高资产文件的传输速度。 此集成可确保增强的下载体验。

>[!NOTE]
>
>下载速度因网络带宽、服务器延迟和客户端地理位置等因素而异。

如果启用，Brand Portal用户可以通过安装Aspera connect客户端，显着缩短从Brand Portal或通过共享链接下载所需资源文件所花费的时间。

![](assets/enable-fast-file-download.png)

## 加快文件下载的先决条件 {#prerequisites-to-accelerate-file-download}

要更快地下载文件，请确保：

* **[!UICONTROL 从管理工具面板的]**“常规设置”中启用“下载加[!UICONTROL 速”]（默认情况下为禁用）。
* 端口33001（TCP和UDP）在防火墙上处于打开状态。 有关入门项目的详细信息，请参 [阅Aspera connect客户端文档](https://downloads.asperasoft.com/en/documentation/8)。
* 使用管理员权限安装Aspera Connect。
* 有关Aspera传输客户端的平台支持，请参 [阅Aspera connect平台支持列表](https://www.asperasoft.com/company/support/transfer-clients/)。

## 下载域 {#download-domains}

以下是不同地理位置的下载域：

| 区域代码 | 域 |
|---|---|
| NA OR1 | downloads-na1.brand.portal.adobe.com |
| NA VA5 | downloads-na2.brand.portal.adobe.com |
| EMEA LON5 | downloads-emea1.brand-portal.adobe.com |
| APAC SIN2 | downloads-apac1.brand-portal.adobe.com |

## 使用文件加速器的示例下载性能 {#expected-download-performance-using-file-accelerator}

下表显示了使用Aspera connect文件下载加速器下载2 GB文件的性能：

*由于Brand Portal服务器位于俄勒冈州（美国），因此观察到的结果会因网络带宽、服务器延迟和客户端位置等因素而异。*

| 客户端位置 | 客户端与服务器之间的延迟（毫秒） | 使用Aspera connect文件传输加速器(MBps)加快速度 | 下载带Aspera文件传输加速器的2 GB文件所花费的时间（秒） |
|---------------------------|-----------------------------------|---------------------------------------------|-------------------------------------------------------------------------|
| 美国西部（北美）加利福尼亚) | 18 | 36 | 57 |
| 美国西部（俄勒冈） | 42 | 36 | 57 |
| 美国东部（北美）维吉尼亚) | 85 | 35 | 58 |
| APAC（东京） | 124 | 36 | 57 |
| Noida（印度） | 275 | 13.36 | 153 |
| 悉尼 | 175 | 29 | 70 |
| 伦敦 | 179 | 35 | 58 |
| 新加坡 | 196 | 34 | 60 |

## 使用文件加速器下载工作流程 {#download-workflow-using-file-accelerator}

要从Brand Portal更快地下载资源，请执行以下操作：

1. 使用支持的浏览器登录到Brand Portal。
1. 浏览并选择要下载的所需资产文件、文件夹或集合。 点按／单击下载选项。
将显示“下载”对话框， [并选中“启用下载加速] ”选项。
   ![](assets/download-assetsbp.png)

   >[!NOTE]
   >
   >当前不支持使用指向下载资产的链接发送电子邮件通知的功能，同时启用更快的下载。

   ![](assets/fast-download-emailchk.png)

1. 点按／单击“下 **[!UICONTROL 载]**”选项。
要加快Brand Portal租户帐户的下载体验，您需要在系统上安装Aspera connect客户端应用程序。

1. **下载Aspera connect客户端**&#x200B;如果系统中未安装Aspera connect客户端，或现有安装的Aspera connect客户端已过时，则浏览器页面上会显示提示，您可以通过选择“下载最新版本”从中下载系统特定的Aspera connect客户端 ****。

   ![](assets/aspera-not-launched.png)

   要从https://downloads.asperasoft.com/connect2/下载最新版Aspera Connect [，请选择“](https://downloads.asperasoft.com/connect2/)立即下载 ****”并按照说明操作。

1. **安装Aspera connect客户端**&#x200B;要安装IBM Aspera connect客户端设置，请从IBM Aspera connect客户端应用程序的。msi文件运行安装程序，然后按照安装向导进行操作。

1. 成功安装客户端后，刷新浏览器页面并再次启动下载步骤，或选择“在资产下载中重 **[!UICONTROL 新启动]**”(**[!UICONTROL  Restart in asset Download]** )对话框（步骤#2）。
首次使用Aspera connect时，浏览器会提示使用 **[!UICONTROL IBM Aspera connect打开链接]**。 要在将来跳过此对话框，请启**[!UICONTROL &#x200B;用记住我对FASP链接的选择]**。

   >[!NOTE]
   >
   >此消息在不同的浏览器上不同。

1. 对话框会确认是否继续传输。 选择 **[!UICONTROL 允许]**，开始。
要在将来跳过此对话框，请启**[!UICONTROL &#x200B;用“对与此主机的所有连接使用我的选择”]**。
下载开始。 将显示一个对话框，显示下载进度。 使用对话框可 **[!UICONTROL 暂停]**、继**[!UICONTROL &#x200B;续]**或取 **[!UICONTROL 消下载]**。
Aspera connect应用程序在系统上提供一个活动窗口，用户可在该窗口中查看和管理所有传输会话。 有关详细信息，请参[阅Aspera connect客户端文档](https://downloads.asperasoft.com/en/documentation/8)。

![](assets/aspera-activity-window.png)

成功完成下载后，将显示一个对话框，其中显示资产下载到用户系统的位置。 如果出现故障，则显示错误。

>[!NOTE]
>
>Aspera connect客户端应用程序中存在一个已知限制，即如果在“首选项”中的选项卡“传输”下启用了“始终询问我保存下载文件的位置 ****”，则不会显示选择下载位置的提示。 在任何下载开始之前，请在“将下载的文件保存到”文本框**[!UICONTROL &#x200B;中提供该位置]**。

## 在Microsoft edge浏览器上使用文件加速器 {#using-file-accelerator-on-microsoft-edge-browser}

Microsoft edge在同一专用网络或受信任站点上以增强保护模式(EPM)运行，以防止与Aspera connect服务器通信。 因此，每次与服务器建立连接时都会出现一个弹出窗口。

![](assets/switchapps-msedge.png)

要在Microsoft edge上使用加速下载功能，请从受信任的站点列表中删除Brand Portal站点。

1. 打开控制面板(按 **[!UICONTROL Window键+ X]**，然后选择**[!UICONTROL &#x200B;控制面板]**)。
1. 转到“网 **[!UICONTROL 络和Internet”>“Internet选项”]**。 Click the**[!UICONTROL  Security]** tab.
1. 单击“受 **[!UICONTROL 信任的站点”区域]**，然后单击“**[!UICONTROL &#x200B;站点”]**。
1. 从列表中删除Brand Portal站点。

## Aspera connect客户端首选项 {#aspera-connect-client-preferences}

在IBM Aspera connect客户端首选项中，右键单击图标并选择首选项，可以设置一些有用的首 **[!UICONTROL 选项]**。

![](assets/download_assets_frombrandportalimg19.png)

您可以设置默认下载位置。

![](assets/aspera-preferences.png)

此外，Aspera connect客户端可以标记为在系统启动时自动启动，以便连接客户端正在运行并可供下载以更快开始。

![](assets/aspera-automaticallylaunch.png)

## 下载加速问题疑难解答 {#troubleshoot-issues-with-download-acceleration}

如果下载加速不适合您，请按照以下步骤进行疑难解答：

1. 通过从您的计算机访问https://test-connect.asperasoft.com，检查是否 [阻止](https://test-connect.asperasoft.com/) 端口。

   如果端口不正常，请联系网络团队，确保防火墙中不阻止端口33001（TCP和UDP）。

1. 如果端口正常，则使用https://www.speedtest.net/测量可用带宽，检查网络是否不 [慢](https://www.speedtest.net/)。

   如果带宽只有几(1-10 Mbps)或Kbps，则使用Aspera首选项并尝试限制与可用带宽相等的带宽。

1. 要确认来自Aspera演示服务器的下载是否正常，请使用 [https://demo.asperasoft.com/aspera/user](https://demo.asperasoft.com/aspera/user)。\
   (登录： asperaweb，密码： demoaspera

1. 如果上述疑难解答步骤都不起作用，请取消选择“启用下载加速”选项，然后使用正常下载。
