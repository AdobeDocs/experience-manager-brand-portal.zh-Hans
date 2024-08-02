---
title: 管理资产的数字权限
description: 为资源和共享链接授予资产许可并设置过期时间，可确保控制这些资产的使用，并保护它们。
contentOwner: bdhar
topic-tags: download-install
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
role: Admin
exl-id: 86c31891-0627-41ca-b571-8dac3a074d55
source-git-commit: 10f89ded6febb1a024cbe181fa48a290d90223f0
workflow-type: tm+mt
source-wordcount: '887'
ht-degree: 3%

---

# 管理资产的数字权限 {#manage-digital-rights-of-assets}

确保创意资产和品牌资料的安全分发和使用对于保护您的品牌至关重要。 通过将到期日期（和时间）与从AEM发布到Brand Portal的已批准资源关联，或通过许可这些资源进行有条件使用，可以强制执行此流程。 此外，通过Brand Portal，还可以指定从Brand Portal共享的资源链接的到期日期。

请阅读并了解如何在Brand Portal上保护资源以及相关的使用权限。

## 资产到期 {#asset-expiration}

资源到期是控制Brand Portal上批准资源在组织内的使用情况的一种有效方式。 从AEM Assets发布到Brand Portal的所有资源都可以有一个过期日期，该日期限制不同用户角色使用这些资源。

### 与过期资产相关的使用权限 {#usage-permissions-expired-assets}

在Brand Portal中，管理员可以查看、下载过期的资源并将其添加到收藏集。 但是，编辑者和查看者只能查看已过期的资产并将其添加到收藏集。

管理员可以将已过期的资源从AEM Assets发布到Brand Portal。 但是，无法使用Brand Portal中的链接共享已过期的资源。 如果从包含已过期和未过期资产的文件夹中选择任何已过期的资产，则&#x200B;**[!UICONTROL 共享链接]**&#x200B;操作将不可用。 但是，如果您选择的文件夹包含已过期和未过期的资源，则可使用[!UICONTROL 共享]和&#x200B;**[!UICONTROL 共享链接]**&#x200B;操作。

>[!NOTE]
>
>即使文件夹包含过期的资产，该文件夹仍可以链接形式共享。 在这种情况下，该链接不会列出已过期的资产，而是仅共享未过期的资产。

下表显示已过期资产的使用权限：

|   | **[!UICONTROL 链接共享]** | **[!UICONTROL 下载]** | **[!UICONTROL 属性]** | **[!UICONTROL 添加到收藏集]** | **[!UICONTROL 删除]** |
|---|---|---|---|---|---|
| **[!UICONTROL 管理员]** | 不可用 | 可用 | 可用 | 可用 | 可用 |
| **[!UICONTROL 编辑器]** | 不可用 | 不可用 | 可用 | 可用 | 不可用 |
| **[!UICONTROL 查看器]** | 不可用 | 不可用 | 可用 | 可用 | 不可用 |
| **[!UICONTROL 来宾用户]** | 不可用 | 不可用 | 可用 | 可用 | 不可用 |

>[!NOTE]
>
>如果查看者和编辑者下载的文件夹包含已过期和未过期的资产，则只会下载未过期的资产。 如果文件夹仅包含过期的资源，则会下载空文件夹。

### 资源的到期状态 {#expiration-status-of-assets}

您可以在资产的&#x200B;**[!UICONTROL 卡片视图]**&#x200B;中查看资产的到期状态。 卡片上的红色标记表示资产已过期。

![](assets/expired_assets_cardview.png)

>[!NOTE]
>
>列表和列视图不显示资源的到期状态。

## 资产链接过期 {#asset-link-expiration}

通过链接共享资产时，管理员和编辑者可以使用&#x200B;**[!UICONTROL 链接共享]**&#x200B;对话框中的&#x200B;**[!UICONTROL 过期]**&#x200B;字段设置过期日期和时间。 链接的默认有效期为自链接共享日期起七天。

![](assets/asset-link-sharing.png)

它可确保作为链接共享的资源在Brand Portal管理员和编辑人员设置的日期和时间过期。 并且，在过期日期之后，将无法再查看和下载资源。 为了防止外部用户访问您的已批准资产，请在共享链接上设置到期日期，以确保在指定时间后不会向未知实体公开这些资源。

有关链接共享的详细信息，请参阅[将资源作为链接共享](../using/brand-portal-link-share.md)。

## 许可的Assets {#licensed-assets}

在从Brand Portal下载许可资产之前，必须接受许可协议。 当您直接从Brand Portal或通过共享链接下载资源时，即会签署此许可资源协议。 无论是否已过期，所有用户都可以查看受许可证保护的资产。 但是，已过期的许可资产的下载和使用有限。 要了解过期许可资产的行为以及基于用户角色的可允许活动，请参阅过期资产的[使用权限](../using/manage-digital-rights-of-assets.md#usage-permissions-expired-assets)。

受许可证保护的资产附有[许可协议](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/administer/drm)，可通过在[!DNL Experience Manager Assets]中设置资产的元数据属性来完成此操作。

如果资产包含以下（或两者）元数据属性之一，则将该资产视为受保护：

* `xmpRights:WebStatement`：此属性引用包含资产的许可协议的页面的路径。 `xmpRights:WebStatement`应为存储库中的有效路径。
* `adobe_dam:restrictions`：此属性的值是指定许可协议的原始HTML。


如果您选择下载受许可证保护的资产，则会根据元数据属性将您重定向到&#x200B;**[!UICONTROL 版权管理]**&#x200B;页面。

| `adobe_dam:restrictions` | `xmpRights:WebStatement` | 版权管理 |
| --- | --- | --- |
| 是 | - | 该界面同时显示在Assets和Brand Portal中 |
| - | 是（无效路径） | 无接口 |
| 是 | 是（无效路径） | 无接口 |
| 是 | 是（有效路径） | 该界面显示在Assets或Brand Portal</br>中，具体取决于路径对Assets还是Brand Portal有效（或两者都有效）。 |

![](assets/asset-copyright-mgmt.png)

在此，您需要选择要下载的资源并接受关联的许可协议。 如果不接受许可协议，则不会启用&#x200B;**[!UICONTROL 下载]**&#x200B;按钮。

![](assets/licensed-asset-download-2.png)

如果所选内容包含多个受保护资产，则一次选择一个资产，接受许可协议，然后继续下载资产。

## 生成有关已过期资产的报告 {#generate-report-about-expired-assets}

管理员可以生成并下载报表，其中列出在特定时间范围内过期的所有资源。 此报表包含有关过期资产的详细信息（例如大小、类型、指定资产在资产层次结构中的位置的路径、资产过期时间以及资产发布时间）。 此报告的列可以自定义，以根据用户要求显示更多数据。

![](assets/assets-expired.png)

有关报告功能的详细信息，请转到[使用报告](../using/brand-portal-reports.md#work-with-reports)。
