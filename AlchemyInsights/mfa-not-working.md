---
title: 与 MFA 相关的问题
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755121"
---
# <a name="issues-with-azure-mfa"></a>Azure MFA 的问题
若要检查用户是否无法使用多重身份验证 (MFA 进行登录，请执行以下操作之一) 

1. 受影响的用户可能会在 Azure Active Directory 门户中被阻止。 如果是这种情况，该特定用户的身份验证尝试将被自动拒绝。 [请按照本文中的步骤取消阻止。](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. 如果取消阻止用户没有帮助或用户未被阻止，则可以尝试重置用户的 MFA，并将再次执行注册过程。 [请按照本文中的步骤操作。](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

如果这是你第一次启用 MFA，且你的用户无法登录到非浏览器客户端（如 Outlook、Skype 等），可能是你的 O365 订阅上未启用 (Active Directory 身份验证库) 。 在这种情况下，您需要连接到 Exchange Online Powershell 并运行以下 cmdlet：  *set-organizationconfig-OAuth2ClientProfileEnabled： $true*