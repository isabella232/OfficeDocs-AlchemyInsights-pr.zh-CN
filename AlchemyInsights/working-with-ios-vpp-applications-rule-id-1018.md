---
title: 使用 iOS VPP 应用程序规则 Id 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719947"
---
# <a name="working-with-ios-vpp-applications"></a>使用 iOS VPP 应用程序

了解[如何通过使用 Microsoft intune 通过批量购买计划购买的 iOS 应用](https://docs.microsoft.com/intune/vpp-apps-ios)，了解使用 Apple Volume purchase program 的功能、约束和步骤，以及在 Microsoft intune 中对其的支持。
  
 **常见问题：**"我向用户分配了一个 iOS VPP 应用，但安装失败。"
  
- 如果跨多个移动设备管理提供程序使用单个 VPP 令牌，则可能会发生这种情况。 来自 Apple 的 VPP 令牌仅可与一个提供程序一起使用。 如果将 VPP 令牌与多个提供程序一起使用，则必须将令牌重新上载到 Intune。

- 如果安装总数超过许可证数量，安装也可能会失败。 若要查看许可证的使用率报告，请转到**Intune 移动应用** \> **应用程序许可证**页。 若要了解如何回收使用中的许可证，请参阅[本文。](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
