---
title: 使用 Intune 管理控制台时出现的问题
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 9310e8685a922207be8d5672d7929e19313cbb57e0fa6d25de149106692e811f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53944121"
---
# <a name="problems-using-the-intune-admin-console"></a>使用 Intune 管理控制台时出现的问题

**导航 Intune 管理门户时出现“访问被拒绝”情况。**

- 如果你是 Intune 自定义角色的成员，请确保将 Intune 或企业移动性套件 (EMS) 许可证分配给你的帐户。
- 如果你使用 Configuration Manager 来管理设备，请确认你不属于 Configuration Manager MDM 的 Intune 用户集合。
- 验证是否已在 Intune 角色边栏选项卡中向你分配了适当的基于角色的管理控制 (RBAC) 权限。
- 确认所使用的组不是通讯组列表。 Microsoft Azure 门户中的 Intune 仅支持属于 Azure Active Directory 安全组的用户帐户。 在 Microsoft Azure 门户 >“**Intune**” > “**组**”中或者在 Microsoft Azure 门户 >“**Azure Active Directory**”中查看你的组。

**用户对分配的 Intune 角色拥有太多权限**

建议用户转到“**Intune**” > “**Intune 角色**” > “**我的权限**” > “**导出**”以查看已授予的权限。

**我向某个角色添加了范围组，但是该角色中的用户仍可查看其他用户或设备。**

范围组不会筛选掉用户或设备。范围组：

- 限制用户可以向谁分配策略或应用程序。
- 仅允许特定用户在设备上运行远程任务。

有关范围组的详细信息，请参阅 [Microsoft Intune 的基于角色的访问控制 (RBAC)](https://docs.microsoft.com/intune/role-based-access-control)。

**我向某个 Intune 角色添加到了用户，但他们仍对 Intune 管理控制台具有完全访问权限。**

在 Microsoft Azure 门户中导航到“Intune”>“**用户**”，并验证用户是否未分配给 Microsoft Azure 门户中的以下任何角色：

- 全局管理员
- Intune 服务管理员
- SharePoint 管理员

有关详细信息，请参阅 [Microsoft Intune 的基于角色的访问控制 (RBAC)](https://docs.microsoft.com/intune/role-based-access-control)。

**访问问题**

有关详细信息，请参阅[无法登录到 Office 365、Azure 或 Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune)。