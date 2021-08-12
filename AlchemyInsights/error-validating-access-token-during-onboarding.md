---
title: 在桌面分析启动期间验证访问令牌错误时出错
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
- "2536"
- "9000657"
ms.openlocfilehash: 1d6b840e731eaff537d8f74f9ce0af29af13bd390e701fb2835e8718b4521158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946605"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>桌面分析载入期间出现"验证访问令牌时出错"错误

通常在身份验证令牌过期时观察到此错误。 通常，刷新页面会刷新令牌。 但是，如果存在应用于用于板载桌面分析的帐户的任何条件访问策略，则此问题可能仍然存在。 你可以查看 Azure 门户中的 Azure AD 登录日志，以查看用于桌面分析载入的帐户是否有登录失败。

有关条件访问详细信息，请访问 [规划条件访问部署](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)。