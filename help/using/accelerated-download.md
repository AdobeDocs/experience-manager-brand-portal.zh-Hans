---
title: 加快品牌门户下载
seo-title: 加快品牌门户下载
description: 增强从Brand Portal和共享链接的下载性能。
seo-description: 增强从Brand Portal和共享链接的下载性能。
uuid: 2871137e-6471-49a7-872a-841bd92543d1
contentOwner: mgulati
topic-tags: download-install
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 301f7a0b-5527-4aac-b731-bfc145fed0c0
translation-type: tm+mt
source-git-commit: ecd53a7d92dd020e6a3527793ff11efadcb531ee
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 2%

---


# 加快品牌门户下载 {#guide-to-accelerate-downloads-from-brand-portal}

Brand Portal通过与IBM Aspera Connect集成，可增强大资产文件的下载性能，后者是一个按需安装的应用程序。 该应用程序使用专有技术来消除TCP开销并帮助提高资产文件的传输速度。 此集成可确保增强的下载体验。

>[!NOTE]
>
>下载速度因网络带宽、服务器延迟和客户端地理位置等因素而异。

默 **[!UICONTROL 认情况下]** ，快速下载配置处于启用状态，这可显着缩短从Brand Portal下载所需资产文件所花费的时间。

![](assets/download-configuration.png)

## 加快文件下载的先决条件 {#prerequisites-to-accelerate-file-download}

要更快地下载文件，请确保：

* 导航到 **[!UICONTROL 工具]** >下 **[!UICONTROL 载]** ，并验证在下载设置中 **[!UICONTROL 是否启用了快]** 速下载 ****&#x200B;配置。
* 端口33001（TCP和UDP）在防火墙上处于打开状态。 有关先决条件的详细信息，请参 [阅Aspera Connect客户端文档](https://downloads.asperasoft.com/en/documentation/8)。
* 使用管理员权限安装Aspera Connect。
* 有关Aspera传输客户端的平台支持，请参 [阅Aspera Connect平台支持列表](https://www.asperasoft.com/company/support/transfer-clients/)。

## 下载域 {#download-domains}

以下是不同地理位置的下载域：

| 区域代码 | 域 |
|---|---|
| NA OR1 | downloads-na1.brand-portal.adobe.com |
| NA VA5 | downloads-na2.brand-portal.adobe.com |
| EMEA LON5 | downloads-emea1.brand-portal.adobe.com |
| 亚太SIN2 | downloads-apac1.brand-portal.adobe.com |

## 使用文件加速器的示例下载性能 {#expected-download-performance-using-file-accelerator}

下表显示了使用Aspera Connect文件下载加速器下载2 GB文件的性能：

*由于Brand Portal服务器位于俄勒冈州（美国），因此观察结果会因网络带宽、服务器延迟和客户端位置等因素而有所不同。*

| 客户端位置 | 客户端与服务器之间的延迟（毫秒） | 使用Aspera Connect文件传输加速器(MBps)加快速度 | 下载带Aspera文件传输加速器的2 GB文件所花费的时间（秒） |
|---------------------------|-----------------------------------|---------------------------------------------|-------------------------------------------------------------------------|
| 美国西部（加利福尼亚北部） | 18 | 36 | 57 |
| 美国西部（俄勒冈） | 42 | 36 | 57 |
| 美国东部（弗吉尼亚北部） | 85 | 35 | 58 |
| APAC（东京） | 124 | 36 | 57 |
| 诺伊达语（印度） | 275 | 13.36 | 153 |
| 悉尼 | 175 | 29 | 70 |
| 伦敦 | 179 | 35 | 58 |
| 新加坡 | 196 | 34 | 60 |

## 使用文件加速器下载工作流程 {#download-workflow-using-file-accelerator}

要更快地从Brand Portal下载资源，请执行以下操作：

1. 使用支持的浏览器登录到Brand Portal。
1. 浏览并选择要下载的文件夹或资产。 在顶部的工具栏中，单击“下 **[!UICONTROL 载]** ”图标。 随后 **[!UICONTROL 将显示]** “下载 **[!UICONTROL ”对话框，并]** 默认选中“资产 **[!UICONTROL ”和“]** 启用下载加速”复选框。

   ![](assets/download-assetsbp.png)

   >[!NOTE]
   >
   >当前不支持使用指向下载资产的链接发送电子邮件通知功能，同时启用更快的下载。

   ![](assets/fast-download-emailchk.png)

1. 单击“ **[!UICONTROL 下载]**”。

   要加快Brand Portal租户帐户的下载体验，您需要在浏览器扩展中安装Aspera Connect客户端应用程序。

1. **下载Aspera Connect客户端**

   如果系统中未安装Aspera Connect客户端或现有Aspera Connect客户端已过时，则浏览器页面上会显示提示，您可以通过选择“下载最新版本”从该页面下载系统特定 **[!UICONTROL 的Aspera Connect客户端]**。

   ![](assets/aspera-not-launched.png)

   要从https://downloads.asperasoft.com/connect2/下载最新版Aspera Connect，请选 [择](https://downloads.asperasoft.com/connect2/)“立 **[!UICONTROL 即下载]** ”并按照说明操作。

1. **安装Aspera Connect客户端**

   要安装IBM Aspera Connect客户端安装程序，请从IBM Aspera Connect客户端应用程序的。msi文件运行安装程序，然后按照安装向导进行操作。

1. 成功安装客户端后，请刷新浏览器页面并再次启动下载步骤。

   首次使用Aspera Connect时，浏览器会提示使用IBM Aspera Connect打 **[!UICONTROL 开链接]**。 要以后跳过此对话框，请启 **[!UICONTROL 用“记住我对FASP链接的选择]**”。

   >[!NOTE]
   >
   >此消息在不同的浏览器上不同。

1. 对话框会确认是否继续传输。 选择 **[!UICONTROL 允许]** ，开始。
要在将来跳过此对话框，请启 **[!UICONTROL 用“对与此主机的所有连接使用我的选择]**”。
下载开始。 将显示一个对话框，显示下载进度。 使用对话框 **[!UICONTROL 暂停]**、 **[!UICONTROL 恢复]****** 或取消下载。
Aspera Connect应用程序在系统上提供一个活动窗口，用户可以在该窗口中视图和管理所有传输会话。 有关详细信息，请参 [阅Aspera Connect客户端文档](https://downloads.asperasoft.com/en/documentation/8)。

![](assets/aspera-activity-window.png)

成功完成下载后，将显示一个对话框，显示资产下载到用户系统的位置。 如果出现故障，则显示错误。

>[!NOTE]
>
>Aspera Connect客户端应用程序存在已知限制，如果在“首选项”中的选项卡“传输”下启 **[!UICONTROL 用“始终询问我保存下载文件的位置]** ”，则不会显示选 **[!UICONTROL 择下载]** 位置的提示 ****。 在开始下载之前，请在文本框中提供将下载的文 **[!UICONTROL 件保存到的位置]**。

## 在Microsoft Edge浏览器上使用文件加速器 {#using-file-accelerator-on-microsoft-edge-browser}

Microsoft Edge在同一专用网络或受信任站点上以增强保护模式(EPM)运行，可防止与Aspera Connect服务器进行通信。 因此，每次与服务器建立连接时都会出现一个弹出窗口。

![](assets/switchapps-msedge.png)

要在Microsoft Edge上使用加速下载功能，请从受信任的站点列表中删除Brand Portal站点。

1. 打开控制面板(**[!UICONTROL Window键+ X]**，然后选择 **[!UICONTROL 控制面板]**)。
1. 转到“网 **[!UICONTROL 络和因特网]** ”> **[!UICONTROL “因特网选项]**”。 Click the **[!UICONTROL Security]** tab.
1. 单击“受 **[!UICONTROL 信任的站点]**”区域，然 **[!UICONTROL 后单击]**“站点”。
1. 从列表中删除Brand Portal站点。

## Aspera Connect客户端首选项 {#aspera-connect-client-preferences}

在IBM Aspera Connect客户端首选项中，可以右键单击该图标并选择首选项来设置一些有用的 **[!UICONTROL 首选项]**。

![](assets/download_assets_frombrandportalimg19.png)

可以设置默认下载位置。

![](assets/aspera-preferences.png)

此外，Aspera Connect客户端可被标记为在系统启动时自动开始，以便连接客户端正在运行并可供下载以更快地开始。

![](assets/aspera-automaticallylaunch.png)

## 下载加速问题疑难解答 {#troubleshoot-issues-with-download-acceleration}

如果下载加速不适合您，请按照以下步骤进行疑难解答：

1. 通过从计算机访问https://test-connect.asperasoft.com，检查端 [口](https://test-connect.asperasoft.com/) 是否未被阻止。

   如果端口不正常，请联系网络团队，并确保防火墙中不阻止端口33001（TCP和UDP）。

1. 如果端口正常，则使用https://www.speedtest.net/测量可用带宽，检查网络是否不 [慢](https://www.speedtest.net/)。

   如果带宽只有几(1-10 Mbps)或Kbps，则使用Aspera首选项并尝试限制等于可用带宽的带宽。

1. 要确认来自Aspera演示服务器的下载是否正常，请使用 [https://demo.asperasoft.com/aspera/user](https://demo.asperasoft.com/aspera/user)。\
   (登录： asperaweb，密码： 德马斯帕

1. 如果上述疑难解答步骤均无效，请取消选择“启用下载加速”选项，然后使用正常下载。
