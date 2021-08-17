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
ms.openlocfilehash: 1ac3158914455502d2de493dd1320034b1d09573ebb3ffef24c23eb1e816cad0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082932"
---
# <a name="authentication-app"></a>身份验证应用

如果你是全局管理员，可以使用登录诊断快速了解发生了什么或诊断与用户 [登录相关的问题](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)。

1. 通过单击"启动[诊断"按钮启动](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)诊断。 
1. 通过输入有关用户、应用程序、登录时间、请求 ID 或相关 ID 的详细信息，查找要分析的事件。
1. 查看诊断结果，它会详细显示发生的问题以及可以采取的措施，如果需要措施的话。

**检查适用的方案：**

1. 如果用户未在 Microsoft Authenticator 应用中收到推送通知，请验证它们未显示在"阻止和取消阻止用户"中所述的 MFA 阻止[用户下](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)。
1. 如果未阻止用户进行 MFA，但没有收到推送通知，他们可以打开 Microsoft Authenticator 应用，这将拉取挂起的审批请求。
1. 作为备用登录方法，用户还可以单击"以其他方式登录"，然后从我的移动应用中选择使用验证码。
1. the Microsoft Authenticator App is the only available method for many users. [详细了解安全默认值，请查看](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)[Authenticator常见问题](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq)的应用常见问题以及如何解决这些问题。
 
**建议的视频**

[如何在 2 分钟Authenticator新手机上设置 (应用) 。 ](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
