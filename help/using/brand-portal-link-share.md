---
title: 以链接方式共享资产
seo-title: 以链接方式共享资产
description: AEM Assets Brand Portal管理员可以与授权的内部用户和外部实体（包括合作伙伴和供应商）共享多个资产的链接。 编辑人员只能视图和共享与他们共享的资源。
seo-description: AEM Assets Brand Portal管理员可以与授权的内部用户和外部实体（包括合作伙伴和供应商）共享多个资产的链接。 编辑人员只能视图和共享与他们共享的资源。
uuid: 8889ac24-c56d-4a47-b792-80c34ffb5c3f
contentOwner: bdhar
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f3573219-3c58-47ba-90db-62b003d8b9aa
translation-type: tm+mt
source-git-commit: fab0855e8d30e7b6ddf9b4ae5b2ce1fb627c81ce
workflow-type: tm+mt
source-wordcount: '1002'
ht-degree: 7%

---


# 以链接方式共享资产 {#share-assets-as-a-link}

Adobe Experience Manager Assets Brand Portal管理员可以与授权的内部用户和外部实体（包括合作伙伴和供应商）共享多个资产的链接。 编辑人员只能视图和共享与他们共享的资源。

通过链接共享资产是一种方便的方式，可让外部方可使用它们，因为接收方不必登录Brand Portal即可访问资产。

<!-- Link sharing access is restricted to editors and administrators. 
-->

有关详细信息，请参阅[管理用户、组和用户角色](../using/brand-portal-adding-users.md#manage-user-roles)。

>[!NOTE]
>
>使用Brand Portal上的链接共享功能最多可下载5GB的zip文件。


以下是将资产共享为链接的步骤：

1. 登录到您的Brand Portal租户。 默认情况下，将打开&#x200B;**[!UICONTROL 文件]**&#x200B;视图，其中包含所有已发布的资产和文件夹。

1. 选择要共享的资产或文件夹，或导航到&#x200B;**[!UICONTROL 收藏集]**&#x200B;视图以共享已创建的收藏集。

   ![select-multiple-assets](assets/select-assets-new.png)

1. 在顶部的工具栏中，单击&#x200B;**[!UICONTROL 共享链接]**&#x200B;图标。

   将显示&#x200B;**[!UICONTROL 链接共享]**&#x200B;对话框。

   ![](assets/link-sharing.png)

   * 在电子邮件地址框中，键入要与其共享链接的用户的电子邮件ID。 您可以与多个用户共享链接。 如果用户是您组织的成员，请从下拉列表中显示的建议中选择其电子邮件ID。 如果用户是外部用户，请键入完整的电子邮件ID并按&#x200B;**[!UICONTROL Enter]**;电子邮件ID将添加到用户列表。

      ![](assets/link-sharing-text.png)

   * 在&#x200B;**[!UICONTROL 主题]**&#x200B;框中，为要共享的资产键入主题。
   * 在&#x200B;**[!UICONTROL 消息]**&#x200B;框中，根据需要键入消息。
   * 在&#x200B;**[!UICONTROL 过期]**&#x200B;字段中，使用日期选取器指定链接的过期日期和时间。 默认情况下，过期日期设置为共享链接之日起的7天。
   * 启用&#x200B;**[!UICONTROL 允许下载原始文件]**&#x200B;复选框，以允许收件人下载原始再现。

   通过链接共享的资产在超过&#x200B;**[!UICONTROL Expiration]**&#x200B;字段中指定的日期和时间后过期。 有关过期资产的行为以及基于用户角色在Brand Portal中对允许活动的更改的信息，请参阅[管理资产的数字权限](../using/manage-digital-rights-of-assets.md#asset-expiration)。

   >[!NOTE]
   >
   >链接的默认到期时间为7天。 必须使用&#x200B;**[!UICONTROL 链接共享]**&#x200B;对话框将链接通过电子邮件发送给用户，请勿单独复制和共享链接。

1. 单击&#x200B;**[!UICONTROL 共享]**。系统会显示一条消息，确认已与用户共享该链接。 用户会收到一封包含共享链接的电子邮件。

   ![](assets/link-share-email.png)

   >[!NOTE]
   >
   >管理员可以自定义电子邮件消息，包括使用[品牌](../using/brand-portal-branding.md)功能自定义徽标、说明和页脚。

## 从共享链接{#download-assets-from-shared-links}下载资源

单击电子邮件中的链接以访问共享的资产。 将打开AEM链接共享页面。

要下载共享资产，请执行以下操作：

1. 单击资产或文件夹，然后单击工具栏中的&#x200B;**[!UICONTROL 下载]**&#x200B;图标。

   ![](assets/download-share-link.png)

   >[!NOTE]
   >
   >目前，您只能为某些资产生成预览和缩略图，具体取决于文件格式。 有关支持的文件格式的详细信息，请参阅[资产格式的预览和缩略图支持](#preview-thumbnail-support)。

1. 出现&#x200B;**[!UICONTROL 下载]**&#x200B;对话框。

   ![下载对话框](assets/download-dialog-box-new.png)

1. 默认情况下，在&#x200B;**[!UICONTROL 下载设置]**&#x200B;中启用&#x200B;**[!UICONTROL 快速下载]**&#x200B;设置。 因此，使用IBM Aspera Connect时，会显示一个确认框以继续下载。

   要继续使用&#x200B;**[!UICONTROL 快速下载]**，请单击&#x200B;**[!UICONTROL 允许]**。

   所有选定的演绎版都会下载到一个zip文件夹中，其中每个资产都有一个单独的文件夹。

   >[!NOTE]
   >
   >如果选择了要下载的文件夹、集合或20多个资产，将跳过&#x200B;**[!UICONTROL 下载]**&#x200B;对话框，用户可以访问的所有资产演绎版（不包括动态演绎版）都将下载到zip文件夹中。 系统会为zip文件夹中的每个资产创建一个单独的文件夹。

   >[!NOTE]
   >
   >如果共享资产作为链接的用户未获得管理员的[授权，无法访问原始演绎版](../using/brand-portal-adding-users.md#manage-group-roles-and-privileges)，则不会使用共享链接下载原始演绎版。


>[!NOTE]
>
>Brand Portal限制下载每个文件大小大于5GB的资源。

<!--
1. The **[!UICONTROL Download]** dialog box appears.

   ![](assets/download-linkshare.png)

    * To speed up the download of asset files shared as the link, select **[!UICONTROL Enable download acceleration]** option and [follow the wizard](../using/accelerated-download.md#download-workflow-using-file-accelerator). To know more about the fast download of assets on Brand Portal refer [Guide to accelerate downloads from Brand Portal](../using/accelerated-download.md).
    
1. To download the renditions of assets in addition to the assets from the shared link, select **[!UICONTROL Rendition(s)]** option. When you do so, **[!UICONTROL Exclude System Renditions]** option appears that is selected by default. This prevents the download of out-of-the-box renditions along with approved assets or their custom renditions.

   However, to allow auto-generated renditions to download along with custom renditions, deselect the **[!UICONTROL Exclude System Renditions]** option.

   >[!NOTE]
   >
   >Original renditions are not downloaded using the shared link if the user who shared the assets as a link is not [authorized by the administrator to have access to the original renditions](../using/brand-portal-adding-users.md#manage-group-roles-and-privileges).

   ![](assets/download-linkshare-autoren.png)

1. Click **[!UICONTROL Download]**. The assets (and renditions if selected) are downloaded as a ZIP file to your local folder. However, no zip file is created if a single asset is downloaded without any of the renditions, thereby ensuring speedy download.

>[!NOTE]
>
>Brand Portal restricts downloading assets larger than 5GB per file size.
-->

## 预览和缩略图支持资产格式{#preview-thumbnail-support}

以下矩阵列表了Brand Portal支持其缩略图和预览的资产格式：

| 资产格式 | 缩览图支持 | 预览支持 |
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

下面的图例说明了矩阵中使用的符号：

| 符号 | 意义 |
|---|---|
| ✓ | 此文件格式支持此功能 |
| ✕ | 此文件格式不支持此功能 |
| NA | 此功能不适用于此文件格式 |
| * | 此功能要求在AEM作者实例上支持此文件格式，但在资产发布到Brand Portal后，不要在Brand Portal上支持此文件格式 |

## 取消共享作为链接{#unshare-assets-shared-as-a-link}共享的资源

要取消共享以前共享的资产作为链接，请执行以下操作：

1. 登录Brand Portal时，默认情况下会打开&#x200B;**[!UICONTROL File]**&#x200B;视图。 要视图您作为链接共享的资产，请导航到&#x200B;**[!UICONTROL 共享链接]**&#x200B;视图。

1. 查看您从显示的列表共享的链接。

   ![](assets/shared-links.png)

1. 要从列表中取消共享链接，请选择该链接，然后单击顶部工具栏中的&#x200B;**[!UICONTROL 取消共享]**&#x200B;图标。

   ![](assets/unshare-asset.png)

   >[!NOTE]
   >
   >共享链接的显示特定于用户。 此功能不显示租户的所有用户共享的所有链接。

1. 在警告消息框中，单击&#x200B;**[!UICONTROL 继续]**&#x200B;以确认取消共享。 链接的条目将从共享链接的列表中删除。
