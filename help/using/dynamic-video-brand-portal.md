---
title: Brand Portal 上的动态视频支持
seo-title: Brand Portal 上的动态视频支持
description: Brand Portal 上的动态视频支持
seo-description: Brand Portal 上的动态视频支持
uuid: a3502a4d-3971-4ea4-953c-44ba04446269
contentOwner: mgulati
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: download-install
discoiquuid: e18d992a-a3b5-45f2-9696-8161993213ee
translation-type: tm+mt
source-git-commit: eab0a56cfe03d13485386ddc60400ed458198950
workflow-type: tm+mt
source-wordcount: '1209'
ht-degree: 3%

---


# Brand Portal 上的动态视频支持 {#dynamic-video-support-on-brand-portal}

预览和在品牌门户上自适应播放视频，并提供Dynamic Media支持。 同时从门户和共享链接下载动态演绎版。
Brand Portal用户可以：

* 预览资产详细信息页面、卡片视图和链接共享预览页面中的视频。
* 在“资产详细信息”页面上播放视频编码。
* 视图资产详细信息页面的演绎版选项卡中的动态演绎版。
* 下载包含视频的视频编码和文件夹。

>[!NOTE]
>
>要处理视频并将其发布到Brand Portal，请确保在AEM Author混合模式或Dynamic Media模式下设置您的Dynamic Media实 **[!DNL Scene 7]** 例。

为了预览、播放和下载视频，Brand Portal向管理员公开以下两种配置：

* [Dynamic Media混合配](#configure-dm-hybrid-settings)置如果AEM Author实例在Dynamic Media混合模式上运行。
* [动态 [!DNL Scene 7] 媒体](#configure-dm-scene7-settings)配置如果AEM Author实例在动态媒体模式下&#x200B;**[!DNL Scene 7]** 运行。
根据您在AEM Author实例中设置的、与Brand Portal租户复制的配置，设置其中任一配置。

>[!NOTE]
>
>Brand Portal租户不支持使用在Scene7Connect运行模式上运行的AEM Author **[!UICONTROL 配置的动态]** 视频。

## 动态视频如何播放？ {#how-are-dynamic-videos-played}

![从云中获取视频编码](assets/VideoEncodes.png)

如果Dynamic Media配[置](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) (Hybrid [或[!DNL Scene 7]配置)在Brand Portal上设置，则会从服务器获取动态演](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings)**[!DNL Scene 7]** 绎版。 因此，视频编码在质量上没有延迟和扭曲地被预览和播放。

由于视频编码不存储在Brand Portal存储库中，并从服 **[!DNL Scene 7]** 务器获取，请确保AEM Author实例和Brand Portal上的Dynamic Media配置相同。

>[!NOTE]
>
>Brand Portal不支持视频查看器和查看器预设。 视频在品牌门户的默认查看器上预览和播放。

## 前提条件 {#prerequisites}

要在Brand Portal上处理动态视频，请确保：

* **开始在DM(AEM Author)模式上的Dynamic Media**&#x200B;在Dynamic Media混合模式或动态媒体代码 [上开始AEM Author实例](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) (已配置品 [牌门户) [!DNL Scene 7] ](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode)。
* **在AEM Author上配置Dynamic Media云服**&#x200B;务根据Dynamic Media模式 [AEM Author正在运行，在工具的上](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) 设置Dynamic Media云服 [[!DNL Scene 7] 务或](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) 在AEM Author上设 **置云服务** | **Cloud Service** | **Dynamic Media**。
* **在Brand Portal上配置Dynamic Media**&#x200B;根据AEM Author上的Dynamic Media云配置，从Brand Portal管 [理工具中配](#configure-dm-hybrid-settings) 置 [[!DNL Scene 7] Dynamic Media设](#configure-dm-scene7-settings) 置或设置。
如果您使 [用的是AEM Author混合](#separate-tenants) 、Dynamic MediaScene7模式，请确保为配置了Dynamic Media混合和Dynamic MediaS7模式的Dynamic Media实例使 **[!UICONTROL 用单独的Brand Portal租户]******。
* **使用应用于Brand Portal的视频编码发布文件夹**&#x200B;应 [用视频编码](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) ，并将包含富媒体资产的文件夹从AEM Author实例发布到Brand Portal。
* **启用安全预览时SPS中的允许列表** IP如果使用Dynamic Media **[!DNL Scene 7]** (对公司启用安全预览)，则建议公司管理员为使用SPS（场景7）发布系统(Publishing System)闪存 [SPS的各自区域](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) 列出公共出口IP **[!DNL Scene 7]**[](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)**** 。
出口IP如下所示：

| **区域** | **出口IP** |
|--- |--- |
| NA | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

要允许列出其中一个输出IP，请参 [阅为安全测试服务准备帐户](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)。

## 最佳实践

要确保您的动态视频资产能够从Brand Portal（和共享链接）中成功预览、播放和下载，请遵循以下惯例：

### Dynamic Media混合和Dynamic Media场景7模式的单独租户 {#separate-tenants}

如果您同时使用Dynamic Media **[!DNL Scene 7]** 和Dynamic Media混合功能，建议您对使用Dynamic Media混合模式和Dynamic Media模式配置的AEM Author实例使用不同的品牌门户 **[!DNL Scene 7]** 租户。<br />

![作者与BP一对一映射](assets/BPDynamicMedia.png)

### 在AEM Author实例和Brand Portal上提供相同的配置详细信息

确保配置(如 **[!UICONTROL Title]**、Video Service ID **[!UICONTROL 、Video Service]** URL **[!UICONTROL (在]************************[!DNL Scene 7]****** Dynamic Media中)、、、密码、混合公司、中的、、等)在同一Portal和Portal中都是同一品牌Dynamic Media和AEM云配置

### 允许列出Dynamic MediaScene 7模式的公共出口IP

如果使 **[!UICONTROL 用Dynamic Media]** Scene [7启用安全预览](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)来将视频资产提供给Brand Portal，则 **[!UICONTROL Scene 7]** 会为临时环境或内部应用程序建立专用图像服务器。 对此服务器的任何请求都检查来源IP地址。 如果传入请求不在IP地址的批准列表内，则返回失败响应。
因 **[!UICONTROL 此，Scene-7]** 公司管理员通过SPS **[!UICONTROL (Scene-7 Publishing System)flash UI为公司的安全测试]** 环境配置一个经 **[!UICONTROL 批准的]** IP地址列表。 确保将您各自区域的出口IP（来自以下区域）添加到该批准的列表。
要允许列出其中一个输出IP，请参 [阅为安全测试服务准备帐户](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)。
输出IP如下：

| **区域** | **出口IP** |
|--- |--- |
| NA | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

## 配置Dynamic Media（混合）设置 {#configure-dm-hybrid-settings}

如果AEM Author实例在动态媒体混合模式下运行，则使 **[!UICONTROL 用管理工具]** 面板中的视频拼贴来配置Dynamic Media网关设置。
>[!NOTE]
>
>视 [频编码用户档案](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) 不会发布到Brand Portal，而是从Scene 7服 **[!UICONTROL 务器获取]** 。 因此，为了在Brand Portal中成功播放视频编码，请确保配置详细信息与AEM Author实例 [[!UICONTROL 中的Scene7云配置]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) 相同。
要在Brand Portal租户上设置Dynamic Media配置，请执行以下操作：

1. 选择AEM徽标，从顶部的工具栏访问品牌门户中的管理工具。

2. 从管理工具面板中，选择视 **[!UICONTROL 频拼]** 贴。<br />

   ![Dynamic Media品牌门户上的混合配置](assets/DMHybrid-Video.png)
   **[!UICONTROL “编辑Dynamic Media配置]** ”页将打开。<br />
   ![Dynamic Media在Brand Portal上的混合配置](assets/edit-dynamic-media-config.png)

3. 指 **[!UICONTROL 定注册]** ID **[!UICONTROL 和视频服务URL]** （DM-网关URL）。 确保这些详细信息与AEM Author实例中 **[!UICONTROL 的“工具”]** >“Cloud Service”中的信息相同。

4. 选择 **保存** ，以保存配置。

## 配置Dynamic MediaScene7设置 {#configure-dm-scene7-settings}

如果AEM Author实例在Dynamic Media- Scene 7 **[!UICONTROL 模式下运]** 行，则使用管理工具面板中的 **[!UICONTROL Dynamic Media配置拼贴来配]** 置Scene 7服务器 **** 设置。

要在Brand Portal租户 **[!UICONTROL 上设置Dynamic Media]** Scene 7配置，请执行以下操作：

1. 选择AEM徽标，从顶部的工具栏访问品牌门户中的管理工具。

2. 从管理工具面板中，选择 **[!UICONTROL Dynamic Media配置]** 拼贴。<br />
   ![Brand Portal [!UICONTROL 上的] DM Scene 7配置](assets/DMS7-Tile.png)
   **[!UICONTROL “编辑Dynamic Media配置]** ”页将打开。<br />
   ![Brand Portal上的Scene 7配置](assets/S7Config.png)

3. 提供：
   * **[!UICONTROL 标题]**
   * 用于访&#x200B;**[!UICONTROL 问Scene 7]** 服 **[!UICONTROL 务器的凭]**&#x200B;据（电子邮件ID和密码）
   * **[!UICONTROL 区域]**&#x200B;确保这些值与AEM Author实例中的值相同。

4. Select **[!UICONTROL Connect to Dynamic Media]**.

5. 提供 **[!UICONTROL 公司]**，并 **[!UICONTROL 保存配]** 置。
