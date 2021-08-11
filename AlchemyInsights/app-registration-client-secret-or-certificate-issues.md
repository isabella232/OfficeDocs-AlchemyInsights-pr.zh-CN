---
title: 应用注册客户端密码或证书问题
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9685"
ms.openlocfilehash: 588273f43f7c2d57b377b234885cf4283d466919b562536f78a64356422f9f9f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951483"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>应用注册客户端密码或证书问题

应用程序客户端密码是否即将过期？

无论是通过应用注册门户中的标准注册过程，还是使用应用程序许可在租户中创建服务主体，都需要在当前客户端密码过期之前创建一个新的客户端密码，并更新相关应用程序代码。 最长有效期为 2 年。 提醒一下，必须记录密码值，因为它在门户中离开应用注册页面后将不再可见。 有关详细信息，请参阅快速[入门：](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app)在 Microsoft 标识平台 中注册应用和适用于[Microsoft 标识平台。](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)

若要了解更多信息，请参阅门户中的创建[Azure AD &服务主体 - Microsoft 标识平台。](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)
