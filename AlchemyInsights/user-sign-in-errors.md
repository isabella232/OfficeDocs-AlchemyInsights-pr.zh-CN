---
title: 用户登录错误
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7790"
- "9004355"
ms.openlocfilehash: 05bd31cb4afecf1342e040eecd9e58cd38bd8d49
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886777"
---
# <a name="user-sign-in-errors"></a><span data-ttu-id="b02cd-102">用户登录错误</span><span class="sxs-lookup"><span data-stu-id="b02cd-102">User sign-in errors</span></span>

<span data-ttu-id="b02cd-103">**通过登陆诊断解析问题**</span><span class="sxs-lookup"><span data-stu-id="b02cd-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="b02cd-104">要检测和用户登录问题有关的原因或诊断，请执行下列步骤：</span><span class="sxs-lookup"><span data-stu-id="b02cd-104">To detect the cause or diagnose problems related to user sign-in, perform the following steps:</span></span>

1. <span data-ttu-id="b02cd-105">启动[登陆诊断](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)。</span><span class="sxs-lookup"><span data-stu-id="b02cd-105">Launch the [Sign-in Diagnostic](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
2. <span data-ttu-id="b02cd-106">通过输入你具有的关于用户、应用、登陆时间、请求 ID 或相关 ID 的详细信息，来找到要分析的事件。</span><span class="sxs-lookup"><span data-stu-id="b02cd-106">Find the event to analyze by entering the details you have about the user, application, time of sign in, request Id, or correlation Id.</span></span>
3. <span data-ttu-id="b02cd-107">查看诊断结果，它会显示发生的问题以及可以采取的措施，如果需要措施的话。</span><span class="sxs-lookup"><span data-stu-id="b02cd-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="b02cd-108">**查找关于从 Azure Active Directory (Azure AD) 安全令牌服务 (STS) 返回的 AADSTS 错误代码的信息？**</span><span class="sxs-lookup"><span data-stu-id="b02cd-108">**Looking for information about the AADSTS error codes that are returned from the Azure Active Directory (Azure AD) security token service (STS)?**</span></span> <span data-ttu-id="b02cd-109">阅读[这篇文章](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes)来找到 AADSTS 错误描述、修复以及一些建议的解决方案</span><span class="sxs-lookup"><span data-stu-id="b02cd-109">Read [this article](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds</span></span>