---
title: 密码策略
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718176"
---
# <a name="password-policies"></a>密码策略

**我遇到用户密码策略问题**

- 用户的密码策略取决于用户是仅云还是本地。
- 仅云用户必须选择满足本文中要求的密码：仅适用于云用户帐户 [的密码策略](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)
- 本地用户必须选择满足本地要求的密码。 如果本地用户无法设置其密码，请检查您的本地要求。

**不知道如何设置或检查密码过期策略**

- 可以使用 PowerShell 为租户中的云用户设置和检查过期策略。 按照本文中的说明操作：使用 [PowerShell 设置或检查密码策略](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- 本地用户的密码过期策略在本地 AD 中设置。

**其他有用链接：**
- [密码重置入门](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [管理员启动的密码重置疑难解答](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
