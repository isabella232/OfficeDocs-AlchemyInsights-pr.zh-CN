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
ms.openlocfilehash: 3f633ee1fb3329b6fc634acabbc824af1eccfb33
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897524"
---
# <a name="block-user-from-recording-meetings"></a>阻止用户录制会议

如果你需要阻止 **或阻止** 特定用户录制 Teams 会议，可以通过 Teams 会议策略设置来这样做。 在 Microsoft Teams 管理中心中，关闭分配给该用户的会议策略中的"允许云录制"设置。 若要了解更多信息，请参阅 [在 Teams 中管理会议策略](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording)。

若要验证是否允许特定用户录制 Teams 会议，请使用支持诊断。 运行新的支持查询，并键入 **Diag： Meeting Recording** - 诊断将检查指定用户的策略设置并确定其策略设置。 请记住，新策略设置可能需要几个小时才能生效，因此，如果你刚刚进行了更改，请等待几小时，然后再再次运行诊断。

有关详细信息，请参阅启用 [或关闭云录制](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)。
