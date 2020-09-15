---
title: 隔离中缺少电子邮件
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673704"
---
# <a name="missing-emails-in-quarantine"></a>隔离中缺少电子邮件 "

管理员可以 [查看、释放或删除这些邮件。](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

若要打开安全 & 合规中心，请转到 [https://protection.office.com](https://protection.office.com/) 。 若要直接打开隔离页面，请转到 [https://protection.office.com/quarantine](https://protection.office.com/quarantine) 。  

可以按下面的值搜索：  

- **邮件 ID**：邮件的全局唯一标识符。 如果选择列表中的邮件，则会在显示的 "**详细信息**" 弹出窗口中显示**邮件 ID**值。 管理员可以使用[邮件跟踪](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide)来查找邮件及其相应“邮件 ID”值。
- **发件人电子邮件地址**：单个发件人的电子邮件地址。
- **收件人电子邮件地址**：单个收件人的电子邮件地址。
- **主题**：使用邮件的整个主题。 搜索不区分大小写。

输入搜索条件后，单击 " ![ 刷新按钮 ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **刷新**" 以筛选结果。  

用于查看和管理隔离区中的邮件和文件的 cmdlet 为：
- [删除-Get-quarantinemessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-Get-quarantinemessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-quarantinemessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-get-quarantinemessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)：请注意，此 cmdlet 仅适用于邮件，而不适用于 SharePoint Online、OneDrive for Business 或团队的 ATP 中的恶意软件文件。
- [发布-Get-quarantinemessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)