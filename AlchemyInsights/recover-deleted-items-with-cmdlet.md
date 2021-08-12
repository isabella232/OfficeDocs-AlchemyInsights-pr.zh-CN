---
title: 使用 cmdlet 恢复已删除的项目
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
- "1800008"
- "5718"
ms.openlocfilehash: b3f4f034d5d7486dafa1b5c1801a285b09a34644b811146f09f454fad9647833
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910644"
---
# <a name="recover-deleted-items-with-cmdlet"></a>使用 cmdlet 恢复已删除的项目

- 使用 [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet 查看邮箱中的已删除项目。 找到已删除的项目后，可使用 [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet 还原它们。

- 请参阅 [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) 的完整详细信息。

- 你必须先分配到“邮箱导入导出”角色，才能运行此 cmdlet。有关详细信息，请参阅 [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)。
