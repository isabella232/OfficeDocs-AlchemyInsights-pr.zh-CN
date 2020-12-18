---
title: Apple 自动设备注册同步错误
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49707858"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Apple 自动设备注册同步错误

"我们检测到你拥有一个或多个 ADE/DEP 令牌，这些令牌的状态为错误。 在解决每个受影响的令牌的错误状态之前，ADE 功能将不能用于同一个"。

此错误可能以多种方式显示，包括：

1. 设备可能无法从 ABM/ASM 同步到 Intune
2. 注册配置文件分配可能失败
3. 设备可能无法成功完成 ADE 注册

在设备 > **注册设备 > Apple** 注册 > 注册计划令牌下检查 Intune 控制台中报告的同步错误，并查看以下文档以查看任何可能的修正：

[iOS/iPadOS 和 macOS 自动设备注册令牌的 ABM/ASM 同步错误](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
