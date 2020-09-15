---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685588"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="95ebb-102">阻止旧版身份验证</span><span class="sxs-lookup"><span data-stu-id="95ebb-102">Blocking legacy authentication</span></span>

<span data-ttu-id="95ebb-103">旧式身份验证是指由以下客户端发出的身份验证请求的术语：</span><span class="sxs-lookup"><span data-stu-id="95ebb-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="95ebb-104">不使用新式验证的较旧的 Office 客户端 (例如，Office 2010 客户端) 。</span><span class="sxs-lookup"><span data-stu-id="95ebb-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="95ebb-105">任何使用旧版邮件协议（比如 IMAP/SMTP/POP3）的客户端。</span><span class="sxs-lookup"><span data-stu-id="95ebb-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="95ebb-106">有关阻止旧版身份验证和启用新式身份验证的详细信息，请参阅 [阻止旧版身份验证](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)。</span><span class="sxs-lookup"><span data-stu-id="95ebb-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="95ebb-107"> (Azure AD 中的 Azure Active Directory 中的安全性默认值，) 使其更易于安全并帮助保护组织。</span><span class="sxs-lookup"><span data-stu-id="95ebb-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="95ebb-108">安全性默认值包含针对常见攻击的预先配置的安全设置。</span><span class="sxs-lookup"><span data-stu-id="95ebb-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="95ebb-109">有关安全性默认设置的详细信息，请参阅 [什么是安全默认设置？](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)。</span><span class="sxs-lookup"><span data-stu-id="95ebb-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="95ebb-110">**注意**：如果您的租户是在22Nd 年10月或之后创建的2019，则可能是你遇到了新的安全默认行为，并且已在租户中启用了安全默认行为。</span><span class="sxs-lookup"><span data-stu-id="95ebb-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="95ebb-111">为了保护我们所有用户的努力，安全默认值将向创建的所有新租户推出。</span><span class="sxs-lookup"><span data-stu-id="95ebb-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
