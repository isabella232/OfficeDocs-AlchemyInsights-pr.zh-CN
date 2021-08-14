---
title: 解决 PST 导入问题
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
- "1800027"
- "1225"
ms.openlocfilehash: 549af832f9c58db1cdd8fbe80b8b5bd2aba9bd937f33116806a9391cbc9a5d4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972409"
---
# <a name="troubleshooting-pst-import-issues"></a>解决 PST 导入问题

- 如果要在 Outlook 客户端内导入，请参阅 [解决导入 Outlook .pst 文件的问题](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)。

- 如果使用的是“导入服务”，并且已卡住，请注意，你上传到 Azure 存储位置的每个 PST 文件的大小不得超过 20 GB。 大于 20 GB 的 PST 文件可能会影响 PST 导入过程的性能。 有关卡住作业疑难解答的详细信息，请参阅[影响 PST 导入作业的问题](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)。

- 如果想要验证特定导入任务的状态，请使用 [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest)。

- 有关导入服务的完整信息，请参阅[有关导入组织的 PST 文件概述](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)。
