---
title: 日历图标在 Microsoft 团队客户端中未显示
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576378"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>日历图标在 Microsoft 团队客户端中未显示

团队中的 " **日历** " 选项卡需要通过 Exchange Web 服务访问 exchange 邮箱。 Exchange 邮箱可以是联机的，也可以是本地的。 对于看不到 " **日历** " 选项卡的联机用户，请确保他们已 [获得 Exchange Online 邮箱许可，并且已启用邮箱](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes)。 如果您的用户驻留在本地，则需要确认您的混合配置运行状况良好。 请使用[混合配置向导](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent)排除故障。 请注意，[Teams 需要 Exchange 2016 CU3 或更高版本](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)。

有关详细信息和疑难解答步骤，请参阅 [Microsoft 团队和 Exchange Server 交互问题的疑难解答](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue)。
