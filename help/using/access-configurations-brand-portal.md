---
title: 管理 Brand Portal 上的用户访问权限
seo-title: Administer user access on Brand Portal
description: 在Brand Portal上設定訪客存取權及新使用者存取權。
seo-description: Configure guest access and new users access on brand portal.
uuid: 522b499d-33a0-455f-ac7e-719face48009
contentOwner: mgulati
topic-tags: administration
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 393025b4-722d-4e81-8a47-f83415d0b9b6
role: Admin
exl-id: 27a9cd26-9bb3-473b-b1ac-37f77975c912
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 9%

---

# 管理 Brand Portal 上的用户访问权限 {#administer-user-access-on-brand-portal}

Adobe Experience Manager Assets Brand Portal 6.4.2之後授權管理員設定guest存取權，並讓使用者能夠在其組織的Brand Portal上請求存取權。 這些設定提供為 **[!UICONTROL 存取設定]** 「管理」面板上的設定。 這兩個設定預設為停用。

![](assets/access-configs.png)

**A**   允許訪客存取Brand Portal的設定，使用 **[!UICONTROL 訪客存取？]** Brand Portal歡迎畫面上的連結。 （預設為停用）

**B**   允許使用者透過以下專案請求Brand Portal存取權的設定： **[!UICONTROL 需要存取權？]** Brand Portal歡迎畫面上的連結。 （預設為停用）

## 允许来宾访问 {#allow-guest-access}

透過允許訪客存取，使用者無需登入Brand Portal即可存取公開資產。
若要允許Guest存取，管理員必須執行下列步驟：

1. 從頂端的工具列選取AEM標誌以存取管理工具。
1. 從管理工具面板中選取 **[!UICONTROL 存取]** 以開啟 **[!UICONTROL 存取設定]** 頁面。
1. 啟用 **[!UICONTROL 允許訪客存取]** 設定。
1. **[!UICONTROL 保存更改。]**
1. 登出讓變更生效。

![](assets/bp-welcome-screen.png)

## 允许用户请求访问权限 {#allow-users-to-request-access}

管理員可允許組織使用者從歡迎畫面請求對Brand Portal的存取權。 不過，管理員必須啟用 **[!UICONTROL 允許使用者要求存取權]** 設定，讓請求存取連結出現在歡迎畫面上。

若要允許組織使用者請求對Brand Portal的存取權，管理員需要：

1. 從頂端的工具列選取AEM標誌以存取管理工具。
1. 從管理工具面板中選取 **[!UICONTROL 存取]** 以開啟 **[!UICONTROL 存取設定]** 頁面。
1. 啟用 **[!UICONTROL 允許使用者要求存取權]** 設定。
1. **[!UICONTROL 保存更改。]**
1. 登出讓變更生效。
