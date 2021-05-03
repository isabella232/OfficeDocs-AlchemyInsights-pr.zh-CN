---
title: 导入服务作业停滞疑难解答
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059840"
---
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="57ea1-102">导入服务作业停滞疑难解答</span><span class="sxs-lookup"><span data-stu-id="57ea1-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="57ea1-103">如果遇到导入服务作业停滞或失败的问题，请检查并尝试以下操作：</span><span class="sxs-lookup"><span data-stu-id="57ea1-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="57ea1-104">检查 PST 文件大小。</span><span class="sxs-lookup"><span data-stu-id="57ea1-104">Review the size of of the PST file.</span></span> <span data-ttu-id="57ea1-105">建议导入的 PST 文件的最大大小为 20 GB。</span><span class="sxs-lookup"><span data-stu-id="57ea1-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="57ea1-106">如果怀疑由于损坏跳过的项目，请运行 Scanpst.exe 诊断并修复 PST 文件中的错误。</span><span class="sxs-lookup"><span data-stu-id="57ea1-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="57ea1-107">如果在导入过程中看到“MapiExceptionShutoffQuotaExceeded”错误，请确保目标邮箱有足够容量导入所需的 PST 文件。</span><span class="sxs-lookup"><span data-stu-id="57ea1-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="57ea1-108">有关 PST 导入作业问题疑难解答的详细信息，请参阅[PST 导入作业问题疑难解答](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)。</span><span class="sxs-lookup"><span data-stu-id="57ea1-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="57ea1-109">有关如何修复将 PST 导入 Outlook 时出现问题的信息，请参阅[修复导入 Outlook .pst 文件时出现的问题 (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)。</span><span class="sxs-lookup"><span data-stu-id="57ea1-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>