---
title: 应用程序保护策略
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: ab6ad9c4bf95ee013c66384ec8449ceb1b56e8f3ea9e95c695dbbab0e9fa3fc3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53969961"
---
# <a name="application-protection-policy"></a>应用程序保护策略

如果你不熟悉应用程序保护策略 (APP)，请查看[应用程序保护策略概述](https://docs.microsoft.com/intune/apps/app-protection-policy)。

要开始使用 APP，请参阅[如何创建和分配应用保护策略](https://docs.microsoft.com/intune/app-protection-policies)。

应用程序保护策略要求：

- 用户拥有 Intune 或 EMS 许可证。
- 用户属于应用程序保护策略的目标组。
- 只有一个企业用户登录到设备上受保护的应用程序。
- 应用程序已实施 [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started)。 有关支持 SDK 的应用的列表，请参阅 [Microsoft Intune 的受保护应用](https://docs.microsoft.com/intune/apps-supported-intune-apps)。

满足上述要求的用户登录启用 Intune SDK 的应用后，将应用策略。 确定是否应用策略的最简单方法是要求用户在策略中设置 PIN。 

有关详细信息，请参阅：

[APP/MAM 常见问题疑难解答](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[如何验证应用保护策略设置](https://docs.microsoft.com/intune/app-protection-policies-validate)

[了解应用保护策略发布时间](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[如何监视 Intune 应用保护策略](https://docs.microsoft.com/intune/app-protection-policies-monitor)