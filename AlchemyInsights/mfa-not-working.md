---
title: MFA 问题
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810474"
---
# <a name="issues-with-azure-mfa"></a>Azure MFA 问题
需要检查用户是否无法使用 MFA 身份验证或 MFA (登录) 

1. 受影响的用户可能在 Azure Active Directory 门户中受阻。 如果是这种情况，将自动拒绝对特定用户的身份验证尝试。 [请按照本文中的步骤取消阻止它们。](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. 如果取消阻止用户没有帮助或未阻止用户，可以尝试重置用户的 MFA，他们将再次完成注册过程。 [请按照本文中的步骤操作。](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

如果这是第一次启用 MFA，并且用户无法登录非浏览器客户端（如 Outlook、Skype 等），可能是因为 O365 订阅上未启用 ADAL (Active Directory 身份验证库) 。 在这种情况下，您需要连接到 Exchange Online Powershell 并运行此  *cmdlet：Set-OrganizationConfig -OAuth2ClientProfileEnabled：$true*