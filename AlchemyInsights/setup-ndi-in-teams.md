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
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023512"
---
# <a name="turn-on-ndi-technology"></a>打开 NDI 技术

NDI 技术需要为用户打开两个步骤：

1. 租户管理员必须在 CsTeamsMeetingPolicy 中启用"AllowNDIStreaming"属性。

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. 填充此更改后，最终用户必须从"权限"中®其特定客户端启用 NDI设置 >**技术**。

有关详细信息，请参阅在 Microsoft Teams[中使用 NDI 技术](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)。
