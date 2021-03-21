---
title: Microsoft Defender for Endpoints 的计算机载入问题
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901557"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a>Microsoft Defender for Endpoints 的计算机载入问题

将计算机载入到 MDE 服务时可能会遇到问题。 如果可以访问最终用户计算机，请按照下列步骤进行操作：

1. 下载 [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) 诊断工具的最新预览版本。
2. 右键单击 **MDEClientAnalyzer.cmd** 并选择“以管理员角色运行”。
3. 按照 **MDEClientAnalyzer.htm** 中的任何指导建议操作。
4. 有关详细日志，请查看创建的名为 **MDEClientAnalyzerResult** 的子文件夹。
5. 如果需要其他指导，请与 [Microsoft Defender for Endpoint 支持](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support)联系，并提供生成的 MDEClientAnalyzerResult.zip 文件以供分析。
