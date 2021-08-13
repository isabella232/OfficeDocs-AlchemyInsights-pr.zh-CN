---
title: 用户预配
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
- "9004348"
- "8428"
ms.openlocfilehash: 12490df735ca8c524058404df92db79c6c5682fe2ecafe2b42baed70fa3ab142
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971329"
---
# <a name="user-provisioning"></a>用户预配

- 使用 [按需预配功能](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) 预配用户，并获取有关所执行步骤的详细诊断。
- 若要解决预配用户和组时遇到的疑难问题，请参阅疑难解答指南 [未对用户进行预配](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)。
- 如果看到未预配用户，请参阅 Active Directory (AD) 中的 [预配日志（预览）](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)。 搜索针对特定用户的日志条目。
- 定期重新启动预配，以捕获在上一个预配周期中丢失的任何用户。
- 用户/组可能尚未设置，因为我们的服务尚未有机会评估用户。 查看预配需要的时间指南以及预配配置页上的进度栏。 如果其他详细信息部分中指定的稳定状态是在创建/更新/删除用户的日期之前，则意味着我们尚未评估用户。 在此方案中，最好等待设置服务完成。 如果已实现稳定状态，我们建议在 Azure 门户中从 UI 重新启动。
  - 请注意，我们的服务仅知道源系统中用户/组 (Azure Active Directory) 。 如果直接在应用程序中删除用户/组 (例如 ServiceNow) ，我们将不会注意到这些更改，并且不会根据源系统中用户的状态回滚。 在这种情况下，最好直接在目标应用程序中回滚更改。
- 我们的服务已评估用户/组，确定不应进行预配：
  - 如果已将作用域设置为分配的用户和组，请检查用户/组是否分配给应用程序。
  - 如果将用户/组分配给应用程序，请确保未将其分配给默认访问角色。 此角色不能用于设置。
  - 如果已设置基于属性的作用域筛选器，请确保用户满足您指定的条件。
  - 如果用户已存在于目标系统中以及源和目标匹配中的用户状态，我们不会执行任何进一步的操作。
- 我们的服务尝试预配用户，但失败。 对于这些方案，请查看预配日志的疑难解答和建议选项卡：
  - 用户上的必需属性可能Azure Active Directory或不匹配第三方应用程序所需的格式。 例如，当用户的 Country 属性应为 US 时，该属性可能会设置为美国。
  - 属性是目标应用程序中尚不存在的参照属性。 引用属性是指向另一个对象（例如，作为组的成员的用户）的属性。 用户 ID 将位于组的 member 属性中，但只有在它指向的用户对象已存在时才能进行处理。
