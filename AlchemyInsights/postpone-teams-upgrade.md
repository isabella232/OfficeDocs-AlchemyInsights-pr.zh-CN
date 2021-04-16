---
title: 推迟 Teams 升级
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2737"
- "4000006"
ms.openlocfilehash: abbf696b1554743bda188704272bfd85fe6f94e2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51801221"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a>如何推迟 Microsoft 推动的 Teams 升级

**重要** 提示：我们可以帮助你使用支持诊断修复此问题，但看起来你未使用新管理中心。 若要使用"新建管理中心"，请从右上方滑动切换，右上方显示" **新建管理** 中心"。 使用"新建管理中心"，单击" **需要帮助** ？"小组件，键入"推迟 Teams 升级"，然后按照提示运行诊断。

如果你收到有关从 Skype for Business 到 Microsoft Teams 的 Microsoft 驱动自动升级的通信，并且你希望将自动升级推迟至以后日期，则全局管理员可以登录到[Teams](https://admin.teams.microsoft.com/dashboard)管理门户，在选择Microsoft Teams 升级下的"刷新状态"按钮后，选择"推迟"按钮。 若要查看租户自动升级到 Microsoft Teams 的新日期，请刷新 Teams 管理门户页面。

**注意：** 只有 **收到** 有关自动升级的消息中心通知时，"推迟"按钮才可用。 

全局管理员还可以运行 [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) 来了解有关其当前升级状态的信息。
