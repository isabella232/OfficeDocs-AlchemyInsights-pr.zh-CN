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
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="9569d-102">解决 PST 导入问题</span><span class="sxs-lookup"><span data-stu-id="9569d-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="9569d-103">如果你要在 Outlook 客户端内导入，请参阅 [解决导入 Outlook .pst 文件的问题](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)。</span><span class="sxs-lookup"><span data-stu-id="9569d-103">If you are importing within the Outlook client itself, please see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="9569d-104">如果你使用的是“导入服务”，并且已卡住，请注意，你上传到 Azure 存储位置的每个 PST 文件的大小不得超过 20 GB。</span><span class="sxs-lookup"><span data-stu-id="9569d-104">If you are using Import Service and it is stuck, please note that each PST file that you upload to the Azure Storage location should be no larger than 20 GB.</span></span> <span data-ttu-id="9569d-105">大于 20 GB 的 PST 文件可能会影响 PST 导入过程的性能。</span><span class="sxs-lookup"><span data-stu-id="9569d-105">PST files larger than 20 GB may impact the performance of the PST import process.</span></span>

- <span data-ttu-id="9569d-106">如果你想要验证特定导入任务的状态，可使用 [MailboxImportRequest-batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest)。</span><span class="sxs-lookup"><span data-stu-id="9569d-106">If you want to verify the status of a specific Import job, you can use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="9569d-107">有关导入服务的完整信息，请参阅[有关导入到组织的 PST 文件的概述](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)。</span><span class="sxs-lookup"><span data-stu-id="9569d-107">For full details on the import service, please see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
