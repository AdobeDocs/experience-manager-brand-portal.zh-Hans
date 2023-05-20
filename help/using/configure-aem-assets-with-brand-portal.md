---
title: 使用 Brand Portal 配置 Experience Manager Assets
seo-title: Configure Experience Manager Assets with Brand Portal
description: 深入瞭解如何使用Brand Portal設定Experience Manager Assets。
seo-description: Get an insight into configuring Experience Manager Assets with Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
role: Admin
exl-id: 261c0e84-6b3d-459c-b6b9-a9af106d6943
source-git-commit: 454b05c05359a2068cc29124f826d5bd25a1bad1
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 6%

---

# 使用 Brand Portal 配置 Experience Manager Assets {#configure-integration}

透過Brand Portal設定Adobe Experience Manager Assets可為Brand Portal使用者啟用資產發佈、資產發佈和資產貢獻功能。 它可讓Experience Manager Assets使用者與Brand Portal使用者一起發佈和發佈資產。 Brand Portal使用者可以存取共用資產，並將新資產上傳至資產貢獻資料夾，再發佈回Experience Manager Assets來貢獻資產。

支援使用Brand Portal設定Experience Manager Assets：

* Experience Manager Assetsas a Cloud Service
* Experience Manager Assets （內部部署和託管服務） 6.5及更高版本

從Cloud Manager啟動Experience Manager Assets，即可使用Brand Portal自動設定Brand Portalas a Cloud Service。 啟動工作流程會在後端建立所需的設定，並在與Experience Manager Assetsas a Cloud Service執行個體相同的IMS組織上啟動Brand Portal。

然而，Experience Manager Assets （內部部署和Managed Service）是使用Brand Portal手動設定Adobe Developer主控台，這會取得AdobeIdentity Management Services (IMS) Token以授權Brand Portal租使用者。

>[!NOTE]
>
>***適用於Experience Manager Assets 6.5及更高版本***
>
>之前，Brand Portal是透過舊版OAuth閘道在傳統介面中設定，它會使用JSON Web權杖(JWT)交換取得IMS權杖以取得授權。
>
>自2020年4月6日起，系統不再支援透過舊版OAuth進行設定，而會變更為透過Adobe Developer主控台進行設定。


>[!TIP]
>
>***僅供現有客戶使用（內部部署和託管服務）***
>
>舊版OAuth閘道設定將繼續適用於現有客戶。
>
>如果您遇到舊版OAuth閘道設定問題，請刪除現有設定，並透過Adobe Developer主控台建立新設定。

使用Brand Portal設定AEM Assets的步驟因您的AEM版本，以及您是第一次設定還是升級現有設定而異：

| **AEM 版本** | **新設定** | **升級設定** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [啟動Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 （6.5.4.0及更高版本）** | [创建配置](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [升級設定](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
