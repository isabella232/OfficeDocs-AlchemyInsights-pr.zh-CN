---
title: Microsoft Teams - 来宾访问
ms.author: heidip
author: microsoftheidi
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "311"
- "6500001"
ms.openlocfilehash: 2c78fec14d43c5cbf6aebbc889d606eb2f6c4c64af85997f523d06872c911a0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012298"
---
# <a name="microsoft-teams---guest-access"></a>Microsoft Teams - 来宾访问

如果您需要与 Teams 中组织外部的用户进行通信的帮助，您需要决定是使用来宾访问还是外部访问 ([联合身份验证) ，或者](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access)可以使用这两者。

请务必查看 [差异以了解](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access) 每个功能可用的功能。  例如，联盟 (外部) 允许一对一通信，如聊天和状态。  但是，联盟用户不能参与Teams协作。  如果希望外部用户加入并参与Teams对话或共享文件，则需要启用来宾访问。

**选项 1：打开来宾访问** 在"Teams管理中心"中，转到"组织范围 ["设置 >"来宾访问](https://admin.teams.microsoft.com/company-wide-settings/guest-configuration)"，然后打开"允许在 Teams 中访问"。  对于具有所有其他默认设置的租户，这应该是您需要执行的所有操作。  若要自定义来宾访问配置，请确保按照来宾访问清单 [中的所有步骤操作](https://docs.microsoft.com/microsoftteams/guest-access-checklist)。 完全完成后，你将需要等待 [24 小时](https://docs.microsoft.com/microsoftteams/manage-guests#guest-access-latencies) ，设置才能生效。

如果确信已完成检查表中所有步骤，且已超过 24 小时，请继续操作，尝试将来宾添加到 [团队](https://support.office.com/article/add-guests-to-a-team-in-teams-fccb4fa6-f864-4508-bdde-256e7384a14f#ID0EAABAAA=Desktop)。

有关详细信息（包括"如何"视频，请参阅"来宾访问[Microsoft Teams。](https://docs.microsoft.com/microsoftteams/guest-access)

**选项 2：打开外部访问 (联盟)** 如果还想启用外部访问 (联合身份验证) ，在 Teams 管理中心中，转到"组织范围的 [设置 >](https://admin.teams.microsoft.com/company-wide-settings/external-communications)外部访问"并打开"用户可以与 Skype for Business 和 Teams 用户通信"，然后按照允许 [Teams](https://docs.microsoft.com/microsoftteams/manage-external-access#let-your-teams-users-chat-and-communicate-with-users-in-another-organization)用户与其他组织中的用户聊天和进行通信中的所有步骤操作。
