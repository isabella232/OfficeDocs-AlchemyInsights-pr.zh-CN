---
title: 身份验证应用
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403784"
---
# <a name="authentication-app"></a><span data-ttu-id="2a669-102">身份验证应用</span><span class="sxs-lookup"><span data-stu-id="2a669-102">Authentication app</span></span>

<span data-ttu-id="2a669-103">如果你是全局管理员，可以使用登录诊断快速了解发生了什么或诊断与用户 [登录相关的问题](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)。</span><span class="sxs-lookup"><span data-stu-id="2a669-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="2a669-104">通过单击"启动[诊断"按钮启动](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)诊断。</span><span class="sxs-lookup"><span data-stu-id="2a669-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="2a669-105">通过输入有关用户、应用程序、登录时间、请求 ID 或相关 ID 的详细信息，查找要分析的事件。</span><span class="sxs-lookup"><span data-stu-id="2a669-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="2a669-106">查看诊断结果，它会详细显示发生的问题以及可以采取的措施，如果需要措施的话。</span><span class="sxs-lookup"><span data-stu-id="2a669-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="2a669-107">**检查适用的方案：**</span><span class="sxs-lookup"><span data-stu-id="2a669-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="2a669-108">如果用户未在 Microsoft Authenticator 应用中收到推送通知，请验证他们未显示在 MFA 阻止的用户下，如阻止和 [取消阻止用户中所述](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)。</span><span class="sxs-lookup"><span data-stu-id="2a669-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="2a669-109">如果未阻止用户进行 MFA，但没有收到推送通知，他们可以打开 Microsoft Authenticator 应用，这将拉取挂起的审批请求。</span><span class="sxs-lookup"><span data-stu-id="2a669-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="2a669-110">作为备用登录方法，用户还可以单击"以其他方式登录"，然后从我的移动应用中选择使用验证码。</span><span class="sxs-lookup"><span data-stu-id="2a669-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="2a669-111">Microsoft Authenticator 应用是许多用户唯一可用的方法。</span><span class="sxs-lookup"><span data-stu-id="2a669-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="2a669-112">[详细了解安全默认值，请查看](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) [Authenticator 应用常见问题](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) 解答，了解常见问题以及如何解决这些问题。</span><span class="sxs-lookup"><span data-stu-id="2a669-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="2a669-113">**建议的视频**</span><span class="sxs-lookup"><span data-stu-id="2a669-113">**Recommended Videos**</span></span>

<span data-ttu-id="2a669-114">[如何在 2 分钟或 2 分钟的新手机上 (Authenticator) 。 ](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="2a669-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
