---
title: 与 Microsoft Surface Pro X 的应用程序兼容性
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7009"
- "9003951"
ms.openlocfilehash: 085815982a3948a7853326541101d2ed21c1869e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821354"
---
# <a name="app-compatibility-with-microsoft-surface-pro-x"></a>与 Microsoft Surface Pro X 的应用程序兼容性

应用程序在 Surface Pro X 等设备上运行的方式不同。但存在一些限制，大多数应用是可兼容的。 下面列出了你在运行应用程序时可能的问题： 

**驱动程序。** 如果驱动程序针对基于 Windows 10 ARM 的电脑进行设计，它们将会工作。 如果驱动程序不起作用，则应用（或它依赖的硬件）也不起作用。 有关你的设备的其他支持，请参阅 [基于 WINDOWS 10 ARM 的 PC 常见问题](https://support.microsoft.com/windows/windows-10-arm-based-pcs-faq-477f51df-2e3b-f68f-31b0-06f5e4f8ebb5) 或与硬件制造商核实。

**64 位 （x64） 应用。** 64 位 （x64） 应用将不起作用。 需要 64 位 （ARM64） 应用、32 位 （ARM32） 应用或 32 位 （x86） 应用。 通常可以找到 32 位 （x86） 版应用，但某些应用开发人员仅提供 64 位 （x64） 应用。

**自定义的应用。** 自定义 Windows 体验的应用（如辅助技术或云存储应用）可能会遇到问题。 若要了解更多信息，请与应用程序制造商联系。

**第三方防病毒软件。** 无法安装某些第三方防病毒软件。 Windows 安全可帮助你在 Windows 10 设备支持的生存期内保持安全。

**Windows 传真和扫描。** Windows 传真和扫描在基于 Windows 10 ARM 的电脑上不可用。

如果发现在安装、卸载或重新安装应用时遇到问题，请参阅 [应用疑难解答详细信息](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-app-install#app-troubleshooting-details)。

除在极少数情况下，所有关键字应为 OR，而不是 AND。