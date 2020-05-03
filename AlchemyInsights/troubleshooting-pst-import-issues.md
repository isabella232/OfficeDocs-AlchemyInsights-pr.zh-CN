---
title: 解决 PST 导入问题
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 58fdd509fae5e87bf5ae72db5d8926c4367cdd64
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991107"
---
# <a name="troubleshooting-pst-import-issues"></a>解决 PST 导入问题

- 如果你要在 Outlook 客户端内导入，请参阅 [解决导入 Outlook .pst 文件的问题](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)。

- 如果你使用的是“导入服务”，并且已卡住，请注意，你上传到 Azure 存储位置的每个 PST 文件的大小不得超过 20 GB。 大于 20 GB 的 PST 文件可能会影响 PST 导入过程的性能。

- 如果你想要验证特定导入任务的状态，可使用 [MailboxImportRequest-batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest)。

- 有关导入服务的完整信息，请参阅[有关导入到组织的 PST 文件的概述](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)。
