---
title: Exchange PowerShell 和基本身份验证弃用
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015679"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell 和基本身份验证弃用

有关如何在不使用基本身份验证的情况下连接到 Exchange Online PowerShell 的最新信息，[请转到此处](https://aka.ms/psbasicauth)。

请注意，仍需在客户端计算机上启用基本身份验证。
新版 PowerShell V2 模块使用新式身份验证建立连接，以启用所有基于 REST 的 V2 Cmdlet。 除了 V2 cmdlet 之外，还可访问需要建立远程 PowerShell 会话的旧版远程 PowerShell （RPS） Cmdlet。 在 Windows 计算机上建立 RPS 会话需要在客户端计算机上启用 WinRM 基本身份验证，即使该模块使用新式身份验证机制向该服务进行身份验证。 WinRM 基本身份验证管道用于传输新式身份验证令牌。 如果客户端计算机上禁用了 WinRM 基本身份验证，新版 V2 cmdlet 将继续工作（但旧版 RPS cmdlet 不会）。
