---
title: 条件访问问题
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013920"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="df12e-102">条件访问问题</span><span class="sxs-lookup"><span data-stu-id="df12e-102">Conditional access issues</span></span>

<span data-ttu-id="df12e-103">**通过登陆诊断解析问题**</span><span class="sxs-lookup"><span data-stu-id="df12e-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="df12e-104">可以通过使用登录诊断快速了解发生了什么或诊断与用户登录 [相关的问题](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)：</span><span class="sxs-lookup"><span data-stu-id="df12e-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="df12e-105">启动登陆诊断。</span><span class="sxs-lookup"><span data-stu-id="df12e-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="df12e-106">通过输入有关用户、应用程序、登录时间、请求 ID 或相关 ID 的详细信息来查找要分析的事件。</span><span class="sxs-lookup"><span data-stu-id="df12e-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="df12e-107">查看诊断结果，其中显示所发生的情况的详细信息，以及如果需要任何更改 (可采取哪些操作) 。</span><span class="sxs-lookup"><span data-stu-id="df12e-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="df12e-108">**登录疑难解答的步骤**</span><span class="sxs-lookup"><span data-stu-id="df12e-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="df12e-109">导航到 Azure AD 登录页面。</span><span class="sxs-lookup"><span data-stu-id="df12e-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="df12e-110">按用户、时间范围、应用程序、状态、客户端应用等筛选登录。</span><span class="sxs-lookup"><span data-stu-id="df12e-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="df12e-111">选择登录事件并查看"条件访问"选项卡以查看评估了哪些策略。</span><span class="sxs-lookup"><span data-stu-id="df12e-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="df12e-112">单击策略的行以查看策略详细信息并了解应用策略的原因。</span><span class="sxs-lookup"><span data-stu-id="df12e-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="df12e-113">**条件访问策略疑难解答的工具**</span><span class="sxs-lookup"><span data-stu-id="df12e-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="df12e-114">仅报告模式允许你评估策略，而不会影响用户。</span><span class="sxs-lookup"><span data-stu-id="df12e-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="df12e-115">模拟工具允许你模拟登录事件并查看哪些策略适用。</span><span class="sxs-lookup"><span data-stu-id="df12e-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="df12e-116">见解和报告工作簿显示每个策略实时影响。</span><span class="sxs-lookup"><span data-stu-id="df12e-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="df12e-117">**基线保护策略**</span><span class="sxs-lookup"><span data-stu-id="df12e-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="df12e-118">基线保护策略已弃用。</span><span class="sxs-lookup"><span data-stu-id="df12e-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="df12e-119">它们不再强制执行，并且很快将从 Azure 门户中删除。</span><span class="sxs-lookup"><span data-stu-id="df12e-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="df12e-120">我们建议启用 [安全默认值](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)。</span><span class="sxs-lookup"><span data-stu-id="df12e-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="df12e-121">有关条件访问详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="df12e-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="df12e-122">[Azure Active Directory 中条件访问的最佳实践](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
[条件访问中的条件](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
[条件访问中的控件](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
[条件访问中的位置](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="df12e-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
