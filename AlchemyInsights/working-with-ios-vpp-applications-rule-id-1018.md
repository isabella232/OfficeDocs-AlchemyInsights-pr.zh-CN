---
title: 使用 iOS VPP 应用程序规则 ID 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083004"
---
# <a name="working-with-ios-vpp-applications"></a>使用 iOS VPP 应用程序

阅读如何管理通过 Microsoft Intune 批量购买计划购买的[iOS](https://docs.microsoft.com/intune/vpp-apps-ios)应用，以了解利用 Apple 批量购买计划的功能、约束和步骤，以及 Microsoft Intune 中对它的支持。
  
 **常见问题：** "我向用户分配了 iOS VPP 应用，但安装失败。"
  
- 如果跨多个移动设备管理提供程序使用单个 VPP 令牌，可能会发生这种情况。 来自 Apple 的 VPP 令牌只能用于一个提供程序。 如果你将 VPP 令牌与多个提供程序一同使用，则必须将令牌重新上传到 Intune。

- 如果安装总数超过许可证数，安装也可能失败。 若要查看许可证的使用情况报告，请转到 **Intune 移动应用** \> **应用许可证** 页面。 若要了解如何回收使用中的许可证，请参阅 [本文。](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
