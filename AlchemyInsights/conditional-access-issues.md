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
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069954"
---
# <a name="conditional-access-issues"></a>条件访问问题

**通过登陆诊断解析问题**

通过使用登录诊断，可以快速了解发生了什么或诊断与用户 [登录相关的问题](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)：

1. 启动登陆诊断。
1. 通过输入有关用户、应用程序、登录时间、请求 ID 或相关 ID 的详细信息，查找要分析的事件。
1. 查看诊断结果，其中显示所发生的情况的详细信息，以及当需要进行更改时 (可采取的) 。

**登录疑难解答的步骤** 

1. 导航到 Azure AD 登录页面。
1. 按用户、时间范围、应用程序、状态、客户端应用等筛选登录。
1. 选择登录事件并查看"条件访问"选项卡以查看评估了哪些策略。
1. 单击策略的行以查看策略详细信息并了解它应用的原因。

**条件访问策略疑难解答的工具**

- 仅报告模式允许你评估策略，而不会影响用户。
- 模拟工具允许你模拟登录事件并查看哪些策略适用。
- Insights和报告工作簿将显示每个策略实时影响。

**基线保护策略**

基准保护策略已弃用。 它们不再强制执行，并且很快将从 Azure 门户中删除。 我们建议启用 [安全默认值](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)。

有关条件访问详细信息，请参阅：

[用于条件访问的最佳实践Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
[条件访问中的条件](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
[条件访问中的控件](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
[条件访问中的位置](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
