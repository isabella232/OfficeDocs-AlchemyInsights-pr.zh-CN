---
title: 使用 iOS VPP 应用程序规则 Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 65b9a727171a7551068717f6327f15e1aa8e6bed
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420474"
---
# <a name="working-with-ios-vpp-applications"></a>使用 iOS VPP 应用程序

了解[如何通过使用 microsoft intune 通过批量购买计划购买的 iOS 应用](https://docs.microsoft.com/intune/vpp-apps-ios), 了解使用 Apple volume purchase program 的功能、约束和步骤, 以及在 Microsoft intune 中对其的支持。 
  
 **常见问题:**"我向用户分配了一个 iOS VPP 应用, 但安装失败。" 
  
- 如果跨多个移动设备管理提供程序使用单个 VPP 令牌, 则可能会发生这种情况。 来自 Apple 的 VPP 令牌仅可与一个提供程序一起使用。 如果将 VPP 令牌与多个提供程序一起使用, 则必须将令牌重新上载到 Intune。
    
- 如果安装总数超过许可证数量, 安装也可能会失败。 若要查看许可证的使用率报告, 请转到**Intune 移动应用** \> **应用程序许可证**页。 若要了解如何回收使用中的许可证, 请参阅[本文。](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
    

