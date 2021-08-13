---
title: 解决用户同意问题
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007888"
---
# <a name="troubleshoot-user-consent"></a>解决用户同意问题

1. 你可以配置最终用户如何通过 Azure 门户或 PowerShell 同意应用程序。 有关详细信息 [，请参阅用户](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) 同意设置。
1. 管理员还可使用 Microsoft [Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings)代表单个用户授予委派权限的许可。 有关详细信息，请参阅代表 [用户获取访问权限](https://docs.microsoft.com/graph/auth-v2-user)。
1. [用户同意](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)错误 ：本文讨论在同意应用程序的过程中可能会发生的错误。 如果要解决不包含任何错误消息的意外同意提示，请参阅 [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)的身份验证方案。