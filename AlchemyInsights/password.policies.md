---
title: 密码策略
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718176"
---
# <a name="password-policies"></a><span data-ttu-id="f8289-102">密码策略</span><span class="sxs-lookup"><span data-stu-id="f8289-102">Password policies</span></span>

<span data-ttu-id="f8289-103">**我遇到用户密码策略问题**</span><span class="sxs-lookup"><span data-stu-id="f8289-103">**I'm having problems with the password policy for a user**</span></span>

- <span data-ttu-id="f8289-104">用户的密码策略取决于用户是仅云还是本地。</span><span class="sxs-lookup"><span data-stu-id="f8289-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span></span>
- <span data-ttu-id="f8289-105">仅云用户必须选择满足本文中要求的密码：仅适用于云用户帐户 [的密码策略](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="f8289-105">Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- <span data-ttu-id="f8289-106">本地用户必须选择满足本地要求的密码。</span><span class="sxs-lookup"><span data-stu-id="f8289-106">On-premises users must choose a password that meets the on-premises requirements.</span></span> <span data-ttu-id="f8289-107">如果本地用户无法设置其密码，请检查您的本地要求。</span><span class="sxs-lookup"><span data-stu-id="f8289-107">If an on-premises user is unable to set their password, check your on-premises requirements.</span></span>

<span data-ttu-id="f8289-108">**不知道如何设置或检查密码过期策略**</span><span class="sxs-lookup"><span data-stu-id="f8289-108">**I don't know how to set or check password expiration policies**</span></span>

- <span data-ttu-id="f8289-109">可以使用 PowerShell 为租户中的云用户设置和检查过期策略。</span><span class="sxs-lookup"><span data-stu-id="f8289-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span></span> <span data-ttu-id="f8289-110">按照本文中的说明操作：使用 [PowerShell 设置或检查密码策略](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="f8289-110">Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span></span>
- <span data-ttu-id="f8289-111">本地用户的密码过期策略在本地 AD 中设置。</span><span class="sxs-lookup"><span data-stu-id="f8289-111">The password expiration policy for on-premises users is set in your on-premises AD.</span></span>

<span data-ttu-id="f8289-112">**其他有用链接：**</span><span class="sxs-lookup"><span data-stu-id="f8289-112">**Other Helpful links:**</span></span>
- [<span data-ttu-id="f8289-113">密码重置入门</span><span class="sxs-lookup"><span data-stu-id="f8289-113">Getting Started with Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [<span data-ttu-id="f8289-114">管理员启动的密码重置疑难解答</span><span class="sxs-lookup"><span data-stu-id="f8289-114">Troubleshoot Administrator-initiated Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
