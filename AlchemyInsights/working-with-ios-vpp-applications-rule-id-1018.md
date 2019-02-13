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
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29917486"
---
# <a name="working-with-ios-vpp-applications"></a>使用 iOS VPP 应用程序

阅读了解功能、 约束和步骤，以使[如何管理与 Microsoft Intune 卷购买程序通过购买的 iOS 应用程序](https://docs.microsoft.com/intune/vpp-apps-ios)使用的 Apple 卷购买程序以及为其 Microsoft Intune 中的支持。 
  
 **常见问题：**"已在 iOS VPP 应用分配给我的用户，但安装失败。" 
  
- 如果跨多个移动设备管理提供程序使用单个 VPP 标记，则可能发生错误。Apple VPP 令牌仅可与一个提供程序。如果在 VPP 令牌使用多个提供程序，您必须重新上载到 Intune 的令牌。
    
- 如果安装的总数超过许可证数量，也可以失败安装。若要查看您的许可证使用情况报告，请转到**Intune 移动应用程序** \> **应用程序许可证**页。若要了解如何回收中使用的许可证，请参阅[本文。](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
    

