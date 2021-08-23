---
title: 警报选项卡中缺少警报
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12732"
ms.openlocfilehash: 9fbd9a32e40d858f0ba49931c723a824478aaa12
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/16/2021
ms.locfileid: "58362358"
---
# <a name="alerts-missing-from-alerts-tab"></a>警报选项卡中缺少警报

" **警报"** 选项卡基于租户中应用治理门户中的设置和激活策略运行。 还必须激活应用治理中的开箱即用策略，以允许信号流入 **警报** 选项卡。 

确认已生成警报：

1. 转到"应用管理 [策略](https://compliance.microsoft.com/m365appprotection?viewid=policies) "，并确认你已创建至少一个"活动"或"审核"策略。

1. 选择该策略， **然后在飞出** 窗格中删除"编辑"。 

1. 检查策略配置，确认应基于 24 小时之前启动的策略事件生成警报。

有关应用治理中的警报详细信息，请参阅应用 [威胁检测和修正入门](https://docs.microsoft.com/microsoft-365/compliance/app-governance-detect-remediate-get-started)。