---
title: 暂停计划的更新
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 7ea6c56de00a52080c4a8b47eb5eeee37838420a9e979878c10aeb12885a8b99
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010462"
---
# <a name="pausing-scheduled-updates"></a>暂停计划的更新

发出暂停命令时，设备在下次签入 Intune 之前不会处理该命令。因此，你的设备可能已经：

- 在签入前安装了计划的更新。
- 在发出暂停命令时已关闭了电源。在这种情况下，当设备开启时，可能已在签入之前下载并安装了计划的更新。