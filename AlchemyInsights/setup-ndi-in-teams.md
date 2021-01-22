---
title: 打开 NDI 技术
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/21/2021
ms.locfileid: "49917308"
---
# <a name="turn-on-ndi-technology"></a>打开 NDI 技术

NDI 技术需要为用户打开两个步骤：

1. 租户管理员必须在 CsTeamsMeetingPolicy 中启用"AllowNDIStreaming"属性。

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. 填充此更改后，最终用户必须从"设置®权限"中为特定客户端> **NDI>技术**。

有关详细信息，请参阅在 [Microsoft Teams 中使用 NDI 技术](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)。
