---
title: 软件清单缺失或不准确
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52658046"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a>软件清单缺失或不准确

威胁和漏洞管理 （TVM） 中的软件清单是组织中具有官方公共平台枚举 （CPE） 的已知软件列表。

没有官方 CPE 的软件产品不发布漏洞。 库存还包括供应商名称、弱点数、威胁和公开设备数量等详细信息。

设备上的软件更改通常在两小时内反映到安全门户中。 但是，有时可能需要更长时间。 当前无法强制进行同步;这是持续持续评估。

如果 5 小时后进行了软件更改，并且更改未准确反映到 TVM 中，请按照下列步骤操作：

1. 检查软件证据部分，了解系统是如何检测到软件的。
1. 确保软件受支持。 软件可能仅在设备级别可见，即使威胁和漏洞管理当前也不支持该软件。 但是，只有有限的数据可用。
1. 有关从门户网站报告不准确度的步骤，请参阅[报告不准确度](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)。
   
    **注意**：从 MDE 门户报告不精确性是工程的一个单向通道。 如果问题紧急，请打开支持票证。

有关详细信息，请参阅[软件清单 - 威胁和漏洞管理](/microsoft-365/security/defender-endpoint/tvm-software-inventory)。