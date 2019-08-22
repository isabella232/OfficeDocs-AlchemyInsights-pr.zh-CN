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
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36545145"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="8d0a6-102">与 MFA 相关的问题</span><span class="sxs-lookup"><span data-stu-id="8d0a6-102">Issues with MFA</span></span>
<span data-ttu-id="8d0a6-103">有几个问题需要检查用户是否无法使用多重身份验证 (MFA) 进行登录</span><span class="sxs-lookup"><span data-stu-id="8d0a6-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="8d0a6-104">受影响的用户可能会在 Azure Active Directory 门户中被阻止。</span><span class="sxs-lookup"><span data-stu-id="8d0a6-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="8d0a6-105">如果是这种情况, 该特定用户的身份验证尝试将被自动拒绝。</span><span class="sxs-lookup"><span data-stu-id="8d0a6-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="8d0a6-106">请按照本文中的步骤取消阻止。</span><span class="sxs-lookup"><span data-stu-id="8d0a6-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="8d0a6-107">如果取消阻止用户没有帮助或用户未被阻止, 则可以尝试重置用户的 MFA, 并将再次执行注册过程。</span><span class="sxs-lookup"><span data-stu-id="8d0a6-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="8d0a6-108">请按照本文中的步骤操作。</span><span class="sxs-lookup"><span data-stu-id="8d0a6-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="8d0a6-109">如果这是你第一次启用 MFA, 并且你的用户无法登录到非浏览器客户端 (如 Outlook、Skype 等), 可能在你的 O365 订阅上未启用此类客户端 (Active Directory 身份验证库)。</span><span class="sxs-lookup"><span data-stu-id="8d0a6-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="8d0a6-110">在这种情况下, 您需要连接到 Exchange Online Powershell 并运行以下 cmdlet:  *set-organizationconfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="8d0a6-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>