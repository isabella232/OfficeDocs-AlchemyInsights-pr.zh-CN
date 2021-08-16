---
title: 阻止用户录制会议
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
- "9002530"
- "9325"
ms.openlocfilehash: 7eb3fd34ec6f1a2d431ed276b00dd46b5ec6aa73d69b37ef88b1ba0ca6f5d077
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019174"
---
# <a name="block-user-from-recording-meetings"></a>阻止用户录制会议

如果需要阻止 **或阻止特定** 用户录制Teams会议，可以通过会议策略设置Teams会议策略设置。 在Microsoft Teams中心中，关闭分配给该用户的会议策略中的"允许云录制"设置。 若要了解更多信息，请参阅管理[会议Teams。](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording)

若要验证是否允许特定用户录制Teams会议，请使用支持诊断。 运行新的支持查询，并键入 **Diag： Meeting Recording** - 诊断将检查指定用户的策略设置并确定其策略设置。 请记住，新策略设置可能需要几个小时才能生效，因此，如果你刚刚进行了更改，请等待几小时，然后再再次运行诊断。

有关详细信息，请参阅启用 [或关闭云录制](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)。
