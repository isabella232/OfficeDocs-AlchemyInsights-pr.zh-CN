---
title: 电子数据展示保留错误疑难解答
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 70f0302fd13324b6778390aeb0fe41ff5668d0d1
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330770"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>电子数据展示保留错误疑难解答

遇到电子数据展示保留问题？ 下面提供了要考虑的一些最佳做法：

- 检查保留分发状态。  如果状态为 **开（挂起）** 或 **关（挂起）**，请等待保留分发完成。
- 将电子数据展示保留更新合并到单个批处理请求中，而不是为每个事务重复更新策略。
- 在安全与合规中心 PowerShell 中运行 Set-CaseHoledPolicy <policyname> -RetryDistribution。 有关详细信息，请参阅 [连接到安全与合规中心 PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell)。

有关检查这些设置以及缓解和解决电子数据展示保留问题的其他最佳做法的步骤，请参阅 [电子数据展示保留错误疑难解答](https://docs.microsoft.com/microsoft-365/compliance/hold-distribution-errors)。
有关其他常见电子数据展示问题的疑难解答信息，请参阅 [调查、排查和解决常见电子数据展示问题](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)。
