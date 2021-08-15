---
title: 属性和范围筛选器问题
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 51ed0fabe220d0069d721ec64d049787bacd5b094e19f0c1996a28e07bb56f03
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960177"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>属性和范围筛选器问题

**存在 UPN 值冲突的问题**

“Workday 到 AD 用户设置 Workday 到 AD 用户设置” 显示错误信息 **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**。 操作失败，因为用于添加/修改的 UPN 值不是全林中唯一的。 错误详细信息: **CONSTRAINT_ATT_TYPE - userPrincipalName**。

Workday连接器在创建AD用户账户时试图设置的 **userPrincipalName** 值已经存在于目标 AD 域中。 这意味着：(1) 用户已经存在，且该用户的匹配 ID 检查失败，或者 (2) UPN生成规则生成了一个冲突值。

以下是建议的解决步骤：

如果用户已经存在，并且匹配 ID 检查未能将 Workday 账户链接到 Active Directory 账户，则检查 Workday 和 AD 中的匹配 ID 属性（通常是 **employeeID**）是否完全匹配。 如果他们没有匹配，则是数据问题，需要解决。 例如，如果 Workday 中的 EmployeeID 是 001052，而 AD 中的 EmployeeID 是 1052，那么供应引擎将无法链接这两个账户，并将尝试创建一个已经存在的用户。 本案例的解决方法是改变 AD 中的 **EmployeeID** 值，使其包含前导零成为 001052。
如果生成 UPN 的表达式没有生成唯一值，可以考虑使用 “去重复函数” **SelectUniqueValue** 来每次生成唯一值。

**Workday 到 AD 用户设置没有为 AD 用户账户设管理器属性值**

“Workday 到 AD 用户设置”作业没有为 AD 用户账户设置 **manager** 属性值。 出现此行为时，有两种可能的情形：

1. Workday 中的管理器无法解析到对应的 AD 用户账户，因为该管理器不在范围内。
2. 在有 **多个 AD 域** 的情形下，Workday 中的管理器与用户不在同一个域中。

尝试使用以下步骤来解决问题：

1. 如果已经定义作用域筛选器，请首先检查管理器是否在作用域中，且它是否满足作用域子句。 如果管理器不满足范围筛选器，请更改筛选器，使管理器也位于供应操作的范围内。
2. 如果你有多个 AD 域，则连接器具有一个已知的无用限制来解决跨域管理器的引用。

有关配置 workday 以实现自动设置的更多细节，请参阅 [教程：为自动用户设置配置 Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)。













