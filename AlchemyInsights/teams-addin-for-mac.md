---
title: Mac 版 Teams 外接程序
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: c9c4eb811c93f6d11ebf606ba4bd20cddc2901d6616700ebfe6ef597dd8dc006
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940665"
---
# <a name="teams-add-in-for-mac"></a>Mac 版 Teams 外接程序

若要对 Mac 操作系统用户缺失 Teams 外接程序进行故障排除，请按照下列步骤操作：

**步骤 1：** 如果你有混合 Exchange 本地（需要 2016 CU3 或更高版本），请使用 Test-HMA.ps1 工具确认已正确配置混合新式验证。 有关详细信息，请参阅[验证用于 Outlook for iOS 和 Outlook for Android 的混合新式验证设置](https://aka.ms/TestHMAEAS)。  

**注意** 使用 UPN 地址格式（例如 [username@contoso.com](mailto:username@contoso.com)），而不是域\用户名。 即使对于具有 Exchange Online 邮箱的用户，也要这样做。

**步骤 2：** 让用户在 Outlook for Mac 中转到“**工具**” > “**帐户...**”，然后查找并选择帐户。 确认列出的用户名采用 UPN 格式（例如 [username@contoso.com](mailto:username@contoso.com)）。

**步骤 3：** 确认用户是许可的 Microsoft Teams 用户。 用户必须使用 Office 365 for Mac 订阅、产品版本 16.24 或更高版本。