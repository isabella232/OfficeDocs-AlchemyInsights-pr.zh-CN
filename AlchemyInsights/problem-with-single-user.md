---
title: 单个用户的问题
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50428569"
---
# <a name="problem-with-single-user"></a>单个用户的问题

- 用户可能尚未设置，因为服务尚未有机会评估用户。 查看预配需要的时间以及设置配置页面上的进度栏的指南。 如果其他详细信息部分中指定的稳定状态是在用户创建/更新/删除日期之前，这意味着我们尚未评估用户。 在此方案中，最好等待预配服务完成。

  - 请注意，我们的服务仅知道源系统中用户对云 HR (的更改) 。 对于 Azure AD，源系统中必须存在有效的更改，以检测更改并流入 Active Directory。
- 预配服务评估了用户，并确定了不应进行预配：
  - 如果已设置基于属性的作用域筛选器，请确保用户满足您指定的条件。
  - 如果用户已存在于目标系统中，并且源和目标匹配中用户的状态，我们不会执行任何其他操作。
- 预配服务尝试设置用户，但失败。 对于这些方案，请查看预配日志的"疑难解答和建议"选项卡：
  - 本地 Active Directory 或 Azure AD 中可能缺少用户所需的属性。 例如，userPrincipalName 或 sAMAccountName 生成规则未生成正确的值。
  - 匹配属性 (通常是 employeeId) 无法解析为本地 Active Directory 或 Azure AD 中的唯一用户。 例如，AD 中具有相同 employeeId 的两个用户，服务返回错误代码，指示同一源条目的重复目标条目。

若要查看单个用户和组的日志，请参阅查看特定用户的问题的预配 [日志](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)。
