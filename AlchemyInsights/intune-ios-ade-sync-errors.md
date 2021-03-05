---
title: Apple 自动设备注册同步错误
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448912"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Apple 自动设备注册同步错误

"我们检测到你拥有一个或多个 ADE/DEP 令牌，这些令牌在错误状态中。 在解决每个受影响的令牌的错误状态之前，ADE 功能不会像预期一样工作。"。

此错误可能以多种方式显示，包括：

1. 设备可能无法从 ABM/ASM 同步到 Intune
2. 注册配置文件分配可能失败
3. 设备可能无法成功完成 ADE 注册

检查 Intune 控制台中"设备注册设备>注册设备> Apple 注册> **注册计划令牌** 下报告的同步错误。

同步错误的最常见原因之一是当前令牌过期。 在许多情况下，受影响令牌的续订将解决问题。

如果一个或多个令牌已过期，请参阅以下文档，以帮助你根据情况续订它们：

[续订自动设备注册令牌](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

此外，还可以参阅以下文档，了解可能导致令牌同步失败的其他错误的潜在修正：

[iOS/iPadOS 和 macOS 自动设备注册令牌的 ABM/ASM 同步错误](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[iOS/iPadOS 和 macOS 自动设备注册令牌的 ABM/ASM 同步错误](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
