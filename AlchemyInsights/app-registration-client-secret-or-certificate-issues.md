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
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123065"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>应用注册客户端密码或证书问题

应用程序客户端密码是否即将过期？

无论是通过应用注册门户中的标准注册过程，还是使用应用程序许可在租户中创建服务主体，都需要在当前客户端密码过期之前创建一个新的客户端密码，并更新相关应用程序代码。 最长有效期为 2 年。 提醒一下，必须记录密码值，因为它在门户中离开应用注册页面后将不再可见。 有关详细信息，请参阅 [快速入门：在 Microsoft](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) 标识平台中注册应用和 [Microsoft 标识平台最佳做法](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)。

若要了解更多信息，请参阅在门户 - Microsoft 标识平台 & Azure [AD](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)应用和服务主体。
