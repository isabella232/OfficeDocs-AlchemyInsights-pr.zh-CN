---
title: 与 MFA 相关的问题
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768827"
---
# <a name="issues-with-azure-mfa"></a>Azure MFA 的问题
有几个问题需要检查用户是否无法使用多重身份验证（MFA）登录

1. 受影响的用户可能会在 Azure Active Directory 门户中被阻止。 如果是这种情况，该特定用户的身份验证尝试将被自动拒绝。 [请按照本文中的步骤取消阻止。](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. 如果取消阻止用户没有帮助或用户未被阻止，则可以尝试重置用户的 MFA，并将再次执行注册过程。 [请按照本文中的步骤操作。](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

如果这是你第一次启用 MFA，并且你的用户无法登录到非浏览器客户端（如 Outlook、Skype 等），可能在你的 O365 订阅上未启用此类客户端（Active Directory 身份验证库）。 在这种情况下，您需要连接到 Exchange Online Powershell 并运行以下 cmdlet：  *set-organizationconfig-OAuth2ClientProfileEnabled： $true*