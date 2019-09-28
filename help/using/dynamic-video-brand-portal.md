---
title: Brand Portal上的动态视频支持
seo-title: Brand Portal上的动态视频支持
description: Brand Portal上的动态视频支持
seo-description: Brand Portal上的动态视频支持
uuid: a3502a4d-3971-4ea4-953c-44ba0446269
contentOwner: mgulati
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: 引用
topic-tags: 下载安装
discoiquuid: e18d992a-a3b5-45f2-9696-8161993213ee
translation-type: tm+mt
source-git-commit: 86d4d5c358ea795e35db2dce8c9529ed14e9ee2d

---


# Brand Portal上的动态视频支持 {#dynamic-video-support-on-brand-portal}

借助Dynamic media支持，在Brand Portal上自适应地预览和播放视频。 还可以从门户和共享链接下载动态演绎版。
Brand Portal用户可以：

* 在“资产详细信息”页面、“卡片视图”和“链接共享预览”页面中预览视频。
* 在“资产详细信息”页面上播放视频编码。
* 在“资产详细信息”页面的“演绎版”选项卡中查看动态演绎版。
* 下载视频编码和包含视频的文件夹。

>[!NOTE]
>
>要处理视频并将其发布到Brand Portal，请确保在Dynamic Media Hybrid模式或Dynamic media模式上设置AEM作者实 [!DNL Scene 7] 例。

要预览、播放和下载视频，Brand Portal向管理员公开以下两种配置：

* [Dynamic Media Hybrid配置](#configure-dm-hybrid-settings)如果AEM作者实例在Dynamic Media Hybrid模式上运行。
* [Dynamic Media [!DNL Scene 7]配置](#configure-dm-scene7-settings)If AEM Author实例正在Dynamic Media模式下运[!DNL Scene 7] 行。
根据您在AEM作者实例中设置的配置设置其中任一配置，该实例将复制Brand Portal租户。

>[!NOTE]
>
>与在 [!UICONTROL Scene7Connect运行模式上运行的AEM作者集成的Brand Portal租户不支持动态视频] 。

## 动态视频如何播放？ {#how-are-dynamic-videos-played}

![从云中获取视频编码](assets/VideoEncodes.png)

如果在Brand Portal上设置了Dynamic Media配置([Hybrid](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) or [[!DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) )，则会从服务器获取动态演绎 [!DNL Scene 7] 版。 因此，视频编码在质量上没有延迟和扭曲地被预览和播放。

由于视频编码不存储在Brand Portal存储库中，并从服务器获取，因此，请确保AEM作者实例和Brand Portal上的Dynamic media配置相同。 [!DNL Scene 7]

>[!NOTE]
>
>Brand Portal不支持视频查看器和查看器预设。 视频在Brand Portal的默认查看器上预览并播放。

## 先决条件 {#prerequisites}

要在Brand Portal上使用动态视频，请确保：

* **在DM(Dynamic Media)模式下启动AEM作者**-在 [Dynamic Media Hybrid模式或](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) Dynamic Media [!DNL Scene 7]模式下启动AEM作者实例（与其集成了Brand Portal） [](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode)。
* **在AEM作者上配置Dynamic Media云服务** author基于Dynamic Media模式，AEM作者正在运行，在AEM作者的AEM上设置 [Dynamic Media云服务](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) , [或通过工具设置[!DNL Scene 7]云服务](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices)**** |云 **服务** | **Dynamic Media**。
* **在Brand Portal上配置Dynamic Media**&#x200B;根据AEM作者上的Dynamic Media云配置，从Brand Portal管理工具中配置 [Dynamic Media设置或](#configure-dm-hybrid-settings)[](#configure-dm-scene7-settings) [!DNL Scene 7]设置。
如果您使 [用Dynamic Media Hybrid和Dynamic Media](#separate-tenants)Scene7模式配置的AEM Author实例，请确保单独的Brand Portal租户使用。
* **将视频编码应用于Brand Portal的文件夹**&#x200B;发 [布应用视频编码](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) ，并将包含富媒体资产的文件夹从AEM Author实例发布到Brand Portal。
* **白名单启用安全预览时SPS中的出口IP**([!DNL Scene 7] 公司预览安全)如果使用Dynamic Media [(](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) Dynamic Media安全)，则建议公司管理员使用SPS(Scene 7 Publishing Schene Flash System)为各自的区域为公开出口IP [!DNL Scene 7][](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) （Flash Flash系统）列出)。
出口IP如下所示：

| **区域** | **出口IP** |
|--- |--- |
| NA | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

要将这些出口IP列入白名单，请参 [阅为安全测试服务准备帐户](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)。

## 最佳实践

要确保您的动态视频资产能够从Brand Portal（和共享链接）中成功预览、播放和下载，请遵循以下实践：

### Dynamic Media Hybrid和Dynamic Media Scene 7模式的单独租户 {#separate-tenants}

如果您同时使用Dynamic Media和Dynamic [!DNL Scene 7] Media Hybrid功能，则建议您为使用Dynamic Media Hybrid和Dynamic Media模式配置的AEM作者实例使用不同的Brand Portal租户 [!DNL Scene 7] 。<br />

![作者与BP一对一映射](assets/BPDynamicMedia.png)

### 在AEM作者实例和Brand Portal中的相同配置详细信息

确保诸如 [!UICONTROL Title], [!UICONTROL Id],Service ID [!UICONTROL (] Service Video In The Madia)和Dynamic Media( [!DNL Scene 7]The In TheDynamic Media)中的The Region(The Digination,Chrid Region),HybridCompany(ThedTherianDynamic RegionErinThed)，动态媒体)，动态媒体)，动态标题（标题区域），动态媒体)，动态媒体)，动态标签和EdiaEde-E-Media-Erinal-Edia中的配置在电子邮件中与动态电子邮件中均在电子邮件中相同门户和AEM云配置。

### Dynamic Media Scene 7模式的白名单公共出口IP

如果使用启 [!UICONTROL 用了安全预览的Dynamic Media]Scene 7 [-来将视频资源提供给Brand Portal，则](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)Scene 7  会为升级环境或内部应用程序建立专用的图像服务器。 对此服务器的任何请求都检查源IP地址。 如果传入的请求不在IP地址的批准列表中，则返回失败响应。
因此， [!UICONTROL Scene-7] Company管理员通过 [!UICONTROL SPS] (Scene-7 Publishing System)flash UI为其公司的 [!UICONTROL Secure Testing] Environment配置IP地址的批准列表。 确保将您各自区域（来自以下）的出口IP添加到该批准列表。
要将这些出口IP列入白名单，请参 [阅为安全测试服务准备帐户](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)。
出口IP如下所示：

| **区域** | **出口IP** |
|--- |--- |
| NA | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

## 配置Dynamic Media(Hybrid)设置 {#configure-dm-hybrid-settings}

如果AEM作者实例在Dynamic Media混合模式上运行，则使用管理工具面板中的 [!UICONTROL Video] tile来配置Dynamic Media网关设置。
>[!NOTE]
>
>视 [频编码配置文件不会发布到Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) ，而是从 [!UICONTROL Scene 7服务器获取] 。 因此，要在Brand Portal中成功播放视频编码，请确保配置详细信息与AEM作者实例中的 [[!UICONTROL Scene7云配置]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) 相同。
要在Brand Portal租户上设置Dynamic media配置，请执行以下操作：

1. 选择AEM徽标，以从顶部的工具栏访问Brand Portal中的管理工具。

2. 从管理工具面板中，选择视 **[!UICONTROL 频拼]** 贴。<br />
   ![Brand Portal上的Dynamic Media Hybrid配置](assets/DMHybrid-Video.png)
   **[!UICONTROL 此时将打开“编辑Dynamic Media配置]** ”页。<br />
   ![Brand Portal上的Dynamic Media混合配置](assets/edit-dynamic-media-config.png)

3. 指定 **[!UICONTROL 注册ID]****[!UICONTROL 和视频服务URL]** (DM-Gateway URL)。 确保这些详细信息与AEM作者实例中 **[!UICONTROL 的“工具”]** &gt;“云服务”中的相同。

4. 选择 **保存** ，以保存配置。

## 配置Dynamic Media Scene7设置 {#configure-dm-scene7-settings}

如果AEM作者实例在Dynamic Media- [!UICONTROL Scene 7模式上运行] ，则使用管理工具面板中的 **[!UICONTROL Dynamic Media配置拼贴来配置]** Scene 7  服务器设置。

要在Brand Portal上设置Dynamic Media [!UICONTROL Scene 7] 配置，请执行以下操作：

1. 选择AEM徽标，以从顶部的工具栏访问Brand Portal中的管理工具。

2. 从管理工具面板中，选择Dynamic Media **[!UICONTROL 配置拼贴]** 。<br />
   ![Brand [!UICONTROL Portal上的DM Scene 7] 配置](assets/DMS7-Tile.png)
   [!UICONTROL 此时将打开“编辑Dynamic Media配置] ”页。<br />
   ![Brand Portal上的Scene 7配置](assets/S7Config.png)

3. 提供：
   * [!UICONTROL 标题]
   * 访问Scene 7[!UICONTROL 服务器的凭据] (电子邮 [!UICONTROL 件ID和密码])
   * [!UICONTROL 区域]确保这些值与AEM作者实例中的值相同。

4. Select **[!UICONTROL Connect to Dynamic Media]**.

5. 提供公 **[!UICONTROL 司名称]**，并 **[!UICONTROL 保存配置]** 。
