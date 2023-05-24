---
title: 管理资产的数字权限
seo-title: Manage digital rights of assets
description: 为资源和共享链接授予资产许可并设置过期时间，可确保控制这些资产的使用，并保护它们。
seo-description: Licensing assets and setting expiration for assets and shared links ensure controlled usage of these assets and safeguard them.
uuid: ce30e398-0109-41bf-a4d2-2fcca476f499
contentOwner: bdhar
topic-tags: download-install
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: f77003ba-31fe-4a9e-96c8-dbc4c2eba79e
role: Admin
exl-id: 86c31891-0627-41ca-b571-8dac3a074d55
source-git-commit: d1487434b10b01eaf55f34672267490fd8fd907e
workflow-type: tm+mt
source-wordcount: '907'
ht-degree: 2%

---

# 管理资产的数字权限 {#manage-digital-rights-of-assets}

确保创意资源和品牌资料的安全分发和使用对于保护您的品牌至关重要。 通过将到期日期（和时间）与从AEM发布到Brand Portal的已批准资源相关联，或通过许可这些资源以供有条件使用，可以在整个组织和外部实施此操作。 此外，Brand Portal还允许您为从Brand Portal共享的资源链接指定到期日期。

请阅读并了解如何在Brand Portal上保护资源以及相关的使用权限。

## 资产到期 {#asset-expiration}

资源到期是控制组织内对Brand Portal上已批准资源的使用情况的一种有效方式。 从AEM Assets发布到Brand Portal的所有资源都可以有一个过期日期，该日期会限制不同用户角色对这些资源的使用。

### 与过期资产相关的使用权限 {#usage-permissions-expired-assets}

在Brand Portal中，管理员可以查看、下载过期的资源并将其添加到收藏集。 而编辑者和查看者只能查看过期资产并将其添加到收藏集。

管理员可以将已过期的资源从AEM Assets发布到Brand Portal。 但是，无法通过Brand Portal中的墨迹共享过期的资源。 如果您从包含已过期和未过期资产的文件夹中选择任何已过期的资产，则 **[!UICONTROL 共享链接]** 操作不可用。 但是，如果选择包含已过期和未过期资产的文件夹，则 [!UICONTROL 共享] 和 **[!UICONTROL 共享链接]** 操作可用。

>[!NOTE]
>
>即使文件夹包含过期的资产，该文件夹仍可以链接形式共享。 在这种情况下，该链接不会列出已过期的资产，并且只会共享未过期的资产。

下表显示已过期资产的使用权限：

|  | **[!UICONTROL 链接共享]** | **[!UICONTROL 下载]** | **[!UICONTROL 属性]** | **[!UICONTROL 添加到收藏集]** | **[!UICONTROL 删除]** |
|---|---|---|---|---|---|
| **[!UICONTROL 管理员]** | 不可用 | 可用 | 可用 | 可用 | 可用 |
| **[!UICONTROL 编辑器]** | 不可用 | 不可用 | 可用 | 可用 | 不可用 |
| **[!UICONTROL 查看者]** | 不可用 | 不可用 | 可用 | 可用 | 不可用 |
| **[!UICONTROL 访客用户]** | 不可用 | 不可用 | 可用 | 可用 | 不可用 |

>[!NOTE]
>
>如果查看者和编辑者下载的文件夹中包含已过期和未过期的资产，则只会下载未过期的资产。 如果文件夹仅包含过期的资产，则会下载空文件夹。

### 资源的到期状态 {#expiration-status-of-assets}

您可以在其中查看资源的到期状态 **[!UICONTROL 卡片视图]**. 卡片上的红色标记表示资产已过期。

![](assets/expired_assets_cardview.png)

>[!NOTE]
>
>列表和列视图不显示资源的到期状态。

## 资产链接过期 {#asset-link-expiration}

通过链接共享资产时，管理员和编辑人员可以使用设置过期日期和时间 **[!UICONTROL 过期]** 中的字段 **[!UICONTROL 链接共享]** 对话框。 链接的默认过期时间是从链接共享日期起七天。

![](assets/asset-link-sharing.png)

它可确保作为链接共享的资源在Brand Portal管理员和编辑人员设置的日期和时间过期，并在过期日期后无法再查看和下载。 由于通过链接共享的资产也可以由不属于组织的外部用户查看，因此通过指定过期，您可以确保批准的资产受到保护，并在指定时间后不会向未知实体公开。

有关链接共享的详细信息，请参阅 [将资产作为链接共享](../using/brand-portal-link-share.md).

## 许可资产 {#licensed-assets}

在从Brand Portal下载许可资产之前，必须接受许可协议。 当您直接从Brand Portal下载资源或通过共享链接下载资源时，就会签署此许可资源协议。 无论是否已过期，所有用户都可以查看受许可证保护的资产。 但是，已过期许可资产的下载和使用有限。 要了解已过期许可资产的行为以及基于用户角色的可允许活动，请参阅 [已过期资产的使用权限](../using/manage-digital-rights-of-assets.md#usage-permissions-expired-assets).

受许可证保护的资产具有 [许可证协议已附加](https://experienceleague.adobe.com/docs/experience-manager-65/assets/administer/drm.html) ，方法是将资源的元数据属性设置为 [!DNL Experience Manager Assets].

如果资产包含以下（或两者）元数据属性之一，则该资产被视为受保护：

* `xmpRights:WebStatement`：此属性是指包含资产的许可协议的页面的路径。 `xmpRights:WebStatement` 应为存储库中的有效路径。
* `adobe_dam:restrictions`：此属性的值是指定许可协议的原始HTML。


如果您选择下载受许可证保护的资产，则会将您重定向到 **[!UICONTROL 版权管理]** 页面，具体取决于元数据属性。

| `adobe_dam:restrictions` | `xmpRights:WebStatement` | 版权管理 |
| --- | --- | --- |
| 是 | - | 该界面同时显示在Assets和Brand Portal中 |
| - | 是（无效路径） | 无界面 |
| 是 | 是（无效路径） | 无界面 |
| 是 | 是（有效路径） | 界面显示在Assets或Brand Portal中 </br> 取决于路径对Assets还是Brand Portal（或两者）有效。 |

![](assets/asset-copyright-mgmt.png)

在此，您需要选择要下载的资源并接受关联的许可协议。 如果您不接受许可协议， **[!UICONTROL 下载]** 按钮未启用。

![](assets/licensed-asset-download-2.png)

如果所选内容包含多个受保护的资产，则一次选择一个资产，接受许可协议，然后继续下载该资产。

## 生成有关已过期资产的报告 {#generate-report-about-expired-assets}

管理员可以生成并下载报表，其中列出在特定时间范围内过期的所有资源。 此报表包含有关过期资产的详细信息（例如大小、类型、指定资产在资产层次结构中的位置的路径、资产过期时间以及资产发布时间）。 可以自定义此报告的列，以根据用户要求显示更多数据。

![](assets/assets-expired.png)

有关报告功能的详细信息，请参阅 [使用报告](../using/brand-portal-reports.md#work-with-reports).
