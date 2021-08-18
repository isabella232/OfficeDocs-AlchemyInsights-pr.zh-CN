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
ms.openlocfilehash: c77da6716c0755d6ed4911f490e000bd74d08f92
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329652"
---
# <a name="missing-emails-in-quarantine"></a>隔离中缺少电子邮件

管理员可以查看 [、释放或删除这些邮件](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

In the Microsoft 365 Defender portal at <https://security.microsoft.com> ， go to Review  \> **Quarantine**. 或者，若要直接转到"隔离 **"页面** ，请使用 <https://security.microsoft.com/quarantine> 。  

有关可以使用的搜索/筛选器值详细信息，请参阅在 EOP 中以管理员角色管理隔离的邮件 [和文件](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)。

用于查看和管理隔离邮件和文件的 cmdlet 包括：

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage：](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)请注意，此 cmdlet 仅适用于邮件，而不是 保险箱 Attachments for SharePoint、OneDrive 或 Microsoft Teams。
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
