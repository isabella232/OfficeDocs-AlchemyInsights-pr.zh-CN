---
title: "\"我的应用\"未显示在\"应用治理\"中"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/16/2021
ms.locfileid: "58362360"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>"我的应用"未显示在"应用治理"中

如果应用程序未显示在"应用治理"中，请检查以下内容：

1. 转到 [Azure AD，](https://aad.portal.azure.com/) 通过搜索"概述"页面上顶部栏中的应用名称来查找应用程序的应用 ID。

1. 访问Graph资源管理器"，并使用此查询并替换为相关应用 ID，在服务主体中搜索应用 <appId> < https://graph.microsoft.com/v1.0/servicePrincipals? ID：$search= "appId： <appId> ">

1. 如果未返回任何结果，则使用此查询并替换为相关应用 ID，在应用程序中搜索应用 <appId> < https://graph.microsoft.com/v1.0/applications? ID：$search= "appId： <appId> ">

如果遇到查询问题，请参阅获取 [支持](https://docs.microsoft.com/microsoft-365/business-video/get-help-support)。 

若要详细了解或深入了解应用治理中的应用，请参阅 [了解可见性和见解](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)。

有关查看应用详细信息，请参阅 [查看应用](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps)。
