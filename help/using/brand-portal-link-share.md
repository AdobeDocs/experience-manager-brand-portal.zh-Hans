---
title: 将资产共享为链接
seo-title: 将资产共享为链接
description: AEM Assets Brand Portal管理员可以与授权的内部用户和外部实体(包括合作伙伴和供应商)共享多个资产的链接。编辑人员只能查看和共享与其共享的资产。
seo-description: AEM Assets Brand Portal管理员可以与授权的内部用户和外部实体(包括合作伙伴和供应商)共享多个资产的链接。编辑人员只能查看和共享与其共享的资产。
uuid: 8889ac24-c56 d-4a47-b792-80c34 ffb5 c3 f
contentOwner: bdar
content-type: 引用
topic-tags: sharing
products: SG_ EXPERIENCE MANAGER/Brand_ Portal
discoiquuid: f3573219-3c58-47ba-90db-62b003d8b9aa
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# 将资产共享为链接 {#share-assets-as-a-link}

[!DNL AEM Assets Brand Portal] 管理员可以与授权的内部用户和外部实体(包括合作伙伴和供应商)共享多个资产的链接。编辑人员只能查看和共享与其共享的资产。

通过链接共享资产是一种方便的方式，使外部用户可使用这些资源，因为接收方无需登录 [!DNL Brand Portal] 即可访问资产。

链接共享权限仅限编辑和管理员。有关详细信息，请参阅 [管理用户、用户组和用户角色](../using/brand-portal-adding-users.md#manage-user-roles)。

>[!NOTE]
>
>使用链接共享功能允许最多5GB zip下载 [!DNL brand portal]。

要将资产共享为链接，请执行以下步骤：

1. 单击左侧的叠加图标，然后选择 **“导航**”。

   ![](assets/siderail.png)

2. 从左侧的提问器中，单击 **“文件** ”以共享文件夹或图像。要共享收藏集，请单击 **[!UICONTROL 收藏集]**。

   ![](assets/navigationrail.png)

3. 选择要作为链接共享的文件夹或集合。

   ![](assets/asset-link-share.png)

4. 在顶部的工具栏中，单击 **共享链接** 图标。

   将显示 **“链接共享”** 对话框。

   ![](assets/link-sharing.png)

   >[!NOTE]
   >
   >**“共享链接** ”字段会显示一个自动创建的资产链接。此链接的默认到期时间为天。您可以复制链接并将其单独共享给用户，或从 **“链接共享”** 对话框共享它。

5. 在电子邮件地址框中，键入您要与之共享链接的用户的电子邮件ID。您可以与多个用户共享链接。

   如果用户是单位的成员，请从下拉列表中显示的建议中选择其电子邮件ID。如果用户为外部用户，请键入完整的电子邮件ID并按 **Enter**；电子邮件ID将添加到用户列表中。

   ![](assets/link-sharing-text.png)

6. In the **Subject** box, type a subject for the asset you want to share.
7. In the **Message** box, type a message if necessary.
8. 在 **“过期** ”字段中，使用日期选取器指定链接的过期日期和时间。默认情况下，过期日期设置为从您共享链接之日起天。

   通过链接共享的资产在跨越 **“过期”** 字段中指定的日期和时间后过期。有关过期资产的行为以及基于中 [!DNL Brand Portal]用户角色的允许活动更改的信息，请参阅 [管理资产的数字权限](../using/manage-digital-rights-of-assets.md#asset-expiration)。

9. 单击&#x200B;**共享**。系统会显示一条消息，确认与用户共享了该链接。用户将收到包含链接的电子邮件。

   ![](assets/link-sharing-email.png)

   >[!NOTE]
   >
   >管理员可以自定义电子邮件消息传递，包括自定义带有 [品牌](../using/brand-portal-branding.md) 功能的徽标、说明和页脚。

## 从共享链接下载资源 {#download-assets-from-shared-links}

单击电子邮件中的链接以查看共享资产。[!DNL AEM] 此时将打开链接共享页面。

要下载共享资产，请执行以下操作：

1. 单击资产，然后单击 **工具栏中的下载** 图标。

   ![](assets/assets-shared-link.png)

   >[!NOTE]
   >
   >当前，您只能为某些资产生成预览和缩略图，具体取决于文件格式。有关支持的文件格式的更多信息，请参阅 [预览和缩览图支持资产格式](#preview-thumbnail-support)。

   >[!NOTE]
   >
   >如果您下载的资产还包含许可的资产，则您将被重定向到 **“版权管理** ”页面。在此页面中，选择许可的资产，单击 **“同意”**，然后单击 **“下载**”。如果您选择不同意，则仅下载未授权的资产。\
   >受许可保护的资产已 [附加](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) 许可协议，通过设置资产 [的元数据属性](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) 来完成此操作 [!DNL AEM Assets]。

   ![](assets/licensed-asset-download.png)

   将显示 **“下载** ”对话框。
   ![](assets/download-linkshare.png)

   * 要加快共享作为链接的资源文件的下载速度，请选择 **“启用下载加速** 选项”并 [按照向导](../using/accelerated-download.md#download-workflow-using-file-accelerator)进行操作。要了解有关快速下载资产的更多信息 [!DNL Brand Portal] ，请参阅参考 [指南快速下载[！DNL Brand Portal]](../using/accelerated-download.md)。

2. 要在共享链接之外下载资产的演绎版，请选择 **演绎版** 选项。这样做时，默认情况下会显示 **“排除系统演绎版** ”选项。这可防止下载现成再现以及已批准的资产或其自定义演绎版。

   但是，要允许自动生成的演绎版与自定义演绎版一起下载，请取消选择 **“排除系统演绎版** ”选项。

   >[!NOTE]
   >
   >如果管理员无权访问原始演绎版 [，则使用共享链接的用户不会使用共享链接下载原始再现](../using/brand-portal-adding-users.md#manage-group-roles-and-privileges)。

   ![](assets/download-linkshare-autoren.png)

3. 点按/单击 **下载**。资产(如果选择)作为ZIP文件下载到本地文件夹。但是，如果下载单个资源而不使用任何再现，则不会创建zip文件，从而确保了快速下载。

>[!NOTE]
>
>[!DNL Brand Portal] 限制下载大于GB的每个文件大小的资源。

## 对资产格式的预览和缩略图支持 {#preview-thumbnail-support}

下面的矩阵列出 [!DNL Brand Portal] 了支持缩略图和预览的资产格式：

| 资产格式 | 缩略图支持 | 预览支持 |
|--------------|-------------------|-----------------|
| PNG | ✓ | ✓ |
| GIF | ✓ | ✓ |
| TIFF | ✓ | ✕ |
| JPEG | ✓ | ✓ |
| BMP | ✓ | ✕ |
| PNM* | NA | NA |
| PGM* | NA | NA |
| PBM* | NA | NA |
| PPM* | NA | NA |
| PSD | ✓ | ✕ |
| EPS | NA | ✕ |
| DNG | ✓ | ✕ |
| PICT | ✓ | ✕ |
| PSB* | ✓ | ✕ |
| JPG | ✓ | ✓ |
| AI | ✓ | ✕ |
| DOC | ✕ | ✕ |
| DOCX | ✕ | ✕ |
| ODT* | ✕ | ✕ |
| PDF | ✓ | ✕ |
| HTML | ✕ | ✕ |
| RTF | ✕ | ✕ |
| TXT | ✓ | ✕ |
| XLS | ✕ | ✕ |
| XLSX | ✕ | ✕ |
| ODS | ✕ | ✕ |
| PPT | ✓ | ✕ |
| PPTX | ✕ | ✕ |
| ODP | ✕ | ✕ |
| INDD | ✓ | ✕ |
| PS | ✕ | ✕ |
| QXP | ✕ | ✕ |
| EPUB | ✓ | ✕ |
| AAC | ✕ | ✕ |
| MIDI | ✕ | ✕ |
| 3GP | ✕ | ✕ |
| MP3 | ✕ | ✕ |
| MP4 | ✕ | ✕ |
| OGA | ✕ | ✕ |
| OGG | ✕ | ✕ |
| RA | ✕ | ✕ |
| WAV | ✕ | ✕ |
| WMA | ✕ | ✕ |
| DVI | ✕ | ✕ |
| FLV | ✕ | ✕ |
| M4V | ✕ | ✕ |
| MPG | ✕ | ✕ |
| OGV | ✕ | ✕ |
| MOV | ✕ | ✕ |
| WMV | ✕ | ✕ |
| SWF | ✕ | ✕ |
| TGZ | NA | ✕ |
| JAR | ✓ | ✕ |
| RAR | NA | ✕ |
| TAR | NA | ✕ |
| ZIP | ✓ | ✕ |

以下图例解释了矩阵中使用的符号：

| Symbol | 意义 |
|---|---|
| ✓ | 此文件格式支持此功能 |
| ✕ | 此文件格式不支持此功能 |
| NA | 此功能不适用于此文件格式 |
| * | 此功能需要在创作实例上 [!DNL AEM] 对此文件格式执行附加支持， [!DNL Brand Portal] 但在资产发布到 [!DNL Brand Portal] |

## 取消共享共享作为链接的资产 {#unshare-assets-shared-as-a-link}

要将之前共享的资产取消共享为链接，请执行以下操作：

1. 要查看共享为链接的资产，请单击左侧的叠加图标，然后选择 **“导航”**。

   ![](assets/siderail.png)

2. 从侧栏中，单击 **共享链接**。

   ![](assets/navigationrail.png)

3. 查看您从显示的列表中共享的链接。
4. 要从列表中取消共享链接，请选择该链接，然后单击链接条目旁边的bin图标或顶部工具栏中 **的取消共享** 图标。

   ![](assets/unshare-links.jpg)

   >[!NOTE]
   >
   >共享链接的显示是特定于用户的。此功能不显示租户的所有用户共享的所有链接。

5. 在警告消息框中，单击 **继续** 以确认取消共享。链接条目将从共享链接列表中删除。