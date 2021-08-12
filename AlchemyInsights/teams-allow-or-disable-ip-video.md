---
title: Teams 允许或禁用 IP 视频
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: ad60225e5deee4a37831a3145d37916c9ce849f9f4cf475dce4c9a6210f83af9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940629"
---
# <a name="teams-allow-or-disable-ip-video"></a>Teams 允许或禁用 IP 视频

**更改或创建会议策略**

若要更改或创建会议策略，请转到 **Microsoft Teams 管理中心 > 会议 > 会议策略**。 从列表中选择一个策略，或者单击“**添加**”。 如果正在创建新策略，则添加名称和说明。 名称不能包含特殊字符或超过 64 个字符。 选择设置，然后单击“保存”。

例如，假设你有很多用户并且你想要限制这些用户的会议所需的带宽量。 你要创建新的自定义策略并命名为“带宽限制”，然后禁用以下设置：

在“音频和视频”中：

- 禁用“允许云录制”。
- 禁用“允许 IP 视频”。

然后将此策略分配给用户。

**将会议策略分配给用户**

1. 在 Microsoft Teams 管理员中心的左侧导航中，转到“用户”，然后单击相应的用户。
2. 单击用户名的左侧以选择用户，然后单击“编辑设置”。
3. 在 **“会议策略”** 中，选择想要分配的策略，然后单击 **“应用”**。

若要了解详细信息，请参阅[管理 Teams 中的会议策略](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)。
