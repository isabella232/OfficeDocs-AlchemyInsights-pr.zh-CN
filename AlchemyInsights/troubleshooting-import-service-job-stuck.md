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
ms.openlocfilehash: bf07102d01d85eaed8ea95b571a0eabea7c4b7448839294f37e5e30134e04282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105090"
---
# <a name="troubleshooting-import-service-job-stuck"></a>导入服务作业停滞疑难解答

如果遇到导入服务作业停滞或失败的问题，请检查并尝试以下操作：

- 检查 PST 文件大小。 建议导入的 PST 文件的最大大小为 20 GB。

- 如果怀疑由于损坏跳过的项目，请运行 Scanpst.exe 诊断并修复 PST 文件中的错误。

- 如果在导入过程中看到“MapiExceptionShutoffQuotaExceeded”错误，请确保目标邮箱有足够容量导入所需的 PST 文件。

有关 PST 导入作业问题疑难解答的详细信息，请参阅[PST 导入作业问题疑难解答](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)。

有关如何修复将 PST 导入 Outlook 时出现问题的信息，请参阅[修复导入 Outlook .pst 文件时出现的问题 (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)。