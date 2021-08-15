---
title: 隔离中缺少电子邮件
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 900d5f250846e9a7046f72156c150f4970d91d5ad94cb7fc054952228f4bf257
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026212"
---
# <a name="missing-emails-in-quarantine"></a>隔离中缺少电子邮件"

管理员可以查看 [、释放或删除这些邮件。](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

若要打开安全&合规中心，请转到 [https://protection.office.com](https://protection.office.com/) 。 若要直接打开"隔离"页面，请转到 [https://protection.office.com/quarantine](https://protection.office.com/quarantine) 。  

可以按下面的值搜索：  

- **邮件 ID**：邮件的全局唯一标识符。 如果在列表中选择邮件，则"邮件 **ID"** 值将显示在出现的"详细信息"飞出窗格中。 管理员可以使用[邮件跟踪](/microsoft-365/security/office-365-security/message-trace-scc)来查找邮件及其相应“邮件 ID”值。
- **发件人电子邮件地址**：单个发件人的电子邮件地址。
- **收件人电子邮件地址**：单个收件人的电子邮件地址。
- **主题**：使用邮件的整个主题。 搜索不区分大小写。

输入搜索条件后，单击“刷新” ![“刷新”按钮](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) 来筛选结果。

用于查看和管理隔离邮件和文件的 cmdlet 包括：
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage：](/powershell/module/exchange/preview-quarantinemessage)请注意，此 cmdlet 仅适用于来自 Office 365 for SharePoint Online、OneDrive for Business 或 Teams 的 Microsoft Defender 恶意软件文件。
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)