---
title: Microsoft Defender for Endpoint on Microsoft 上的性能问题
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: ab6ad888b34524ac6e3b3d5448d0e6be409ffc0e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331847"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Microsoft Defender for Endpoint on Microsoft 上的性能问题

本文将引导你完成识别适用于 Microsoft Defender for Endpoint（Microsoft Defender for Endpoint）性能问题的步骤。

首先验证您遇到的问题是否已通过[最新版本](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/linux-whatsnew)解决，这一点很重要。 

若要开始调查，请参阅 [Linux上的 Microsoft Defender for Endpoint 性能问题的疑难](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/linux-support-perf)。

## <a name="exclusions"></a>排除项

排除可帮助缓解性能问题。 开始之前应检查排除项，以便已知且记录任何其他风险。

有关详细信息，请参阅 [并验证 Microsoft Defender for Endpoint 在Linux上的排除](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/linux-exclusions)。

如果有多个要排除的文件和文件夹且它们均位于同一个挂载上，排除挂载项可能更简单。 从 2 月 101.22.80 版开始，可以排除整个挂载。

例如，如果 /mnt/backup 是一个挂载项，则可通过运行以下命令将 /mnt/backup 添加到排除列表：

`$ mdatp exclusion folder add –path /mnt/backup`

**注意**：添加排除会增加未检测到恶意软件的风险，应谨慎处理和实施。

## <a name="need-help"></a>需要帮助？

要以最高效的方式提供帮助，请打开支持案例前收集诊断数据。
