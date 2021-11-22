---
title: Brand Portal 上的动态视频支持
seo-title: Dynamic video support on Brand Portal
description: Brand Portal 上的动态视频支持
seo-description: Dynamic video support on Brand Portal
uuid: a3502a4d-3971-4ea4-953c-44ba04446269
contentOwner: mgulati
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: download-install
discoiquuid: e18d992a-a3b5-45f2-9696-8161993213ee
exl-id: 08d6a0fb-061e-4bef-b8e2-bb8522e7482e
source-git-commit: 7128c71576ae938a49f9bff0b95b98b7fc480f69
workflow-type: tm+mt
source-wordcount: '1256'
ht-degree: 3%

---

# Brand Portal 上的动态视频支持 {#dynamic-video-support-on-brand-portal}

在支持Dynamic Media的Brand Portal上自适应预览和播放视频。 此外，还可以从门户和共享链接下载动态演绎版。
Brand Portal用户可以：

* 在“资产详细信息”页面、卡片视图和链接共享预览页面中预览视频。
* 在“资产详细信息”页面上播放视频编码。
* 在资产详细信息页面的演绎版选项卡中查看动态演绎版。
* 下载视频编码和包含视频的文件夹。

>[!NOTE]
>
>要处理视频并将它们发布到Brand Portal，请确保在Dynamic Media混合模式或Dynamic Media上设置您的Experience Manager创作实例 **[!DNL Scene7]** 模式。

为了预览、播放和下载视频，Brand Portal向管理员提供了以下两种配置：

* [Dynamic Media混合配置](#configure-dm-hybrid-settings)
如果Experience Manager创作实例在Dynamic Media混合模式下运行。
* [Dynamic Media [!DNL Scene7] 配置](#configure-dm-scene7-settings)
如果Experience Manager创作实例在Dynamic Media上运行 — **[!DNL Scene7]** 模式。
根据您在用于复制Brand Portal租户的Experience Manager创作实例中设置的配置，设置这些配置中的任一配置。

>[!NOTE]
>
>配置了在上运行“Experience Manager作者”的Brand Portal租户上，不支持动态视频 **[!UICONTROL Scene7Connect]** 运行模式。

## 动态视频的播放方式是如何？ {#how-are-dynamic-videos-played}

![从云中获取视频编码](assets/VideoEncodes.png)

如果Dynamic Media配置([混合](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) 或 [[!DNL Scene7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) 配置)，则会从Brand Portal中获取动态演绎版 **[!DNL Scene7]** 服务器。 因此，视频编码可以在质量上没有延迟和失真地预览和播放。

由于视频编码未存储在Brand Portal存储库中，因此是从 **[!DNL Scene7]** 服务器中，请确保Adobe Experience Manager创作实例和Brand Portal上的Dynamic Media配置相同。

>[!NOTE]
>
>Brand Portal不支持视频查看器和查看器预设。 在Brand Portal的默认查看器上预览和播放视频。

## 前提条件 {#prerequisites}

要处理有关Brand Portal的动态视频，请确保：

* **在Dynamic Media模式下启动Experience Manager作者**
在中启动Experience Manager创作实例(配置了Brand Portal) [Dynamic Media - [!DNL Scene7] 模式](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-scene7-mode/config-dms7.html?lang=en#enabling-dynamic-media-in-scene-mode) 或 [Dynamic Media — 混合模式](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html) 或
* **在Experience Manager作者上配置Dynamic MediaCloud Services**
根据Dynamic Media模式(Scene7模式或混合模式)Experience Manager作者正在运行的模式，请设置以下任一 [Dynamic MediaCloud Services([!DNL Scene7] mode)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-scene7-mode/config-dms7.html?lang=en#configuring-dynamic-media-cloud-services) 或 [Dynamic MediaCloud Services（混合模式）](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html?lang=en#configuring-dynamic-media-cloud-services) 在Experience Manager作者从 **工具** | **Cloud Services** | **Dynamic Media**.
* **在Brand Portal上配置Dynamic Media**
根据Dynamic Media云在Experience Manager作者上的配置，配置 [Dynamic Media设置](#configure-dm-hybrid-settings) 或 [[!DNL Scene7] 设置](#configure-dm-scene7-settings)  从Brand Portal管理工具。
确保 [单独的Brand Portal租户](#separate-tenants) 用于在Dynamic Media中配置的Experience Manager创作实例 —  **[!UICONTROL Scene7]** 模式和Dynamic Media — 混合模式。 特别是当您使用Dynamic Media的功能 **[!UICONTROL S7]** 和Dynamic Media混合。
* **发布文件夹，并将视频编码应用于Brand Portal**
应用 [视频编码](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) 并将包含富媒体资产的文件夹从Experience Manager创作实例发布到Brand Portal。
* **在启允许列表用安全预览时，在SPS中删除IP**
如果使用Dynamic Media -**[!DNL Scene7]** ( [已启用安全预览](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) )，则建议 **[!DNL Scene7]** 公司管理员 [允许列表管理公共出口IP](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) 对于使用SPS的各个区域(**[!UICONTROL Scene7]** 发布系统)flash UI。
出口IP如下：

| **区域** | **出口IP** |
|--- |--- |
| NA | 130.248.160.68, 20.94.203.130 |
| 欧洲、中东和非洲 | 185.34.189.3, 51.132.146.75 |
| APAC | 63.140.44.54 |

要将这些出口IP添加到白名单，请参阅 [准备安全测试服务的帐户](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## 最佳实践

要确保您的动态视频资产能够从Brand Portal（和共享链接）成功预览、播放和下载，请遵循以下实践：

### Dynamic Media - Scene7和Dynamic Media — 混合模式的单独租户 {#separate-tenants}

如果您同时使用Dynamic Media - **[!DNL Scene7]** 模式和Dynamic Media — 混合模式功能，对使用Dynamic Media配置的Experience Manager创作实例使用不同的Brand Portal租户 —  **[!DNL Scene7]** 和Dynamic Media — 混合模式。


![作者与BP一对一映射](assets/BPDynamicMedia.png)

### 与Experience Manager创作实例和Brand Portal中的配置详细信息相同

确保在Brand Portal和 **[!UICONTROL Experience Manager云配置]**. 相同的配置详细信息包括：

* **[!UICONTROL 标题]**
* **[!UICONTROL 注册 ID]**
* **[!UICONTROL 视频服务URL]** in **[!UICONTROL Dynamic Media — 混合模式]**
* **[!UICONTROL 标题]**
* 凭据(**[!UICONTROL 电子邮件]** 和密码)
* **[!UICONTROL 区域]**
* **[!UICONTROL 公司]** 在Dynamic Media中 —  **[!DNL Scene7]** 模式

### 允许列表为Dynamic Media Scene7模式管理公共出口IP

如果Dynamic Media **[!UICONTROL Scene7]**-having [已启用安全预览](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) — 用于将视频资产提供给Brand Portal，然后 **[!UICONTROL Scene7]** 为暂存环境或内部应用程序建立专用的映像服务器。 对此服务器的任何请求都会检查源IP地址。 如果传入的请求不在批准的IP地址列表中，则返回失败响应。
的 **[!UICONTROL Scene7]** 因此，公司管理员会为其公司的 **[!UICONTROL 安全测试]** 环境，通过 **[!UICONTROL SPS]** (Scene7 Publishing System)Flash UI。 确保将相应区域的出口IP（从以下来源）添加到该批准列表。
要将这些出口IP添加到白名单，请参阅 [准备安全测试服务的帐户](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
出口IP如下：

| **区域** | **出口IP** |
|--- |--- |
| NA | 130.248.160.66, 52.151.32.108 |
| 欧洲、中东和非洲 | 185.34.189.1 |
| APAC | 63.140.44.54 |

## 配置Dynamic Media（混合）设置 {#configure-dm-hybrid-settings}

如果Experience Manager创作实例在Dynamic Media混合模式下运行，则使用 **[!UICONTROL 视频]** “管理工具”面板中用于配置Dynamic Media网关设置的磁贴。

>[!NOTE]
>
>的 [视频编码配置文件](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) 不会发布到Brand Portal，而是从 **[!UICONTROL Scene7]** 服务器。 因此，为了在Brand Portal中成功播放视频编码，请确保配置详细信息与 [Dynamic MediaCloud Services([!DNL Scene7] mode)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-scene7-mode/config-dms7.html?lang=en#configuring-dynamic-media-cloud-services) 在Experience Manager创作实例中。

要在Brand Portal租户上设置Dynamic Media配置，请执行以下操作：

1. 选择Experience Manager徽标，以便可以从顶部Brand Portal的工具栏访问管理工具。
1. 从管理工具面板中，选择 **[!UICONTROL 视频]** 拼贴。

   ![Dynamic Media Hybrid Config on Brand Portal](assets/DMHybrid-Video.png)

   **[!UICONTROL 编辑Dynamic Media配置]** 页面。

   ![Dynamic Media Brand Portal上的混合配置](assets/edit-dynamic-media-config.png)

1. 指定 **[!UICONTROL 注册ID]** 和 **[!UICONTROL 视频服务URL]** （DM网关URL）。 确保这些详细信息与 **[!UICONTROL 工具>Cloud Services]** 在Experience Manager创作实例中。
1. 选择 **保存** 以保存配置。

## 配置Dynamic Media Scene7设置 {#configure-dm-scene7-settings}

如果Experience Manager创作实例正在Dynamic Media上运行 —  **[!UICONTROL Scene7]** 模式，然后使用 **[!UICONTROL Dynamic Media配置]** 从“管理工具”面板中配置磁贴 **[!UICONTROL Scene7]** 服务器设置。

设置Dynamic Media **[!UICONTROL Scene7]** Brand Portal租户的配置：

1. 选择Experience Manager徽标，以便可以从顶部Brand Portal的工具栏访问管理工具。

2. 从管理工具面板中，选择 **[!UICONTROL Dynamic Media配置]** 拼贴。

   ![DM [!UICONTROL 场景7] 在Brand Portal中配置](assets/DMS7-Tile.png)

   **[!UICONTROL 编辑Dynamic Media配置]** 页面。

   ![Brand Portal上的Scene 7配置](assets/S7Config.png)

3. 提供：

   * **[!UICONTROL 标题]**
   * 凭据(**[!UICONTROL 电子邮件ID]** 和 **[!UICONTROL 密码]**)访问Scene7服务器
   * **[!UICONTROL 区域]**

   确保这些值与在Experience Manager创作实例中找到的那些值相同。

4. 选择 **[!UICONTROL 连接到Dynamic Media]**.

5. 提供 **[!UICONTROL 公司名称]**&#x200B;和 **[!UICONTROL 保存]** 配置。
