---
title: 在桌面分析备前验证访问令牌错误时出现错误
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741124"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>"在桌面 Analytics 载入过程中验证访问令牌时出现错误" 错误

当身份验证令牌过期时，通常会看到此错误。 通常情况下，刷新页面会刷新令牌。 但是，如果对用于机载桌面 Analytics 的帐户应用了任何条件访问策略，则可能会保留此问题。 您可以在 Azure 门户中查看 Azure AD 登录日志，以查看用于桌面 Analytics 载入的帐户是否存在登录故障。

有关条件访问的详细信息，请参阅[Plan a 条件 access 部署](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)。