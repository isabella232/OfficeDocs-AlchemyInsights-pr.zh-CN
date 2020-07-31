---
title: 暂停计划的更新
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2020
ms.locfileid: "46530584"
---
# <a name="pausing-scheduled-updates"></a>暂停计划的更新

发出暂停命令后，设备在下一次签入 Intune 前不会处理该命令。 因此，你的设备可能存在以下情况：

- 签入前已安装计划的更新。
- 在你发出暂停命令时已关闭电源。 在这种情况下，当设备接通电源后，它们可能已在签入前下载并安装了计划的更新。