---
title: 使用 iOS VPP 应用程序规则 Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: a0bbc1f49f251ef4f16300c8cca98e219008d17e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36557973"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="38ccc-102">使用 iOS VPP 应用程序</span><span class="sxs-lookup"><span data-stu-id="38ccc-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="38ccc-103">了解[如何通过使用 Microsoft intune 通过批量购买计划购买的 iOS 应用](https://docs.microsoft.com/intune/vpp-apps-ios), 了解使用 Apple Volume purchase program 的功能、约束和步骤, 以及在 Microsoft intune 中对其的支持。</span><span class="sxs-lookup"><span data-stu-id="38ccc-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="38ccc-104">**常见问题:**"我向用户分配了一个 iOS VPP 应用, 但安装失败。"</span><span class="sxs-lookup"><span data-stu-id="38ccc-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="38ccc-105">如果跨多个移动设备管理提供程序使用单个 VPP 令牌, 则可能会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="38ccc-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="38ccc-106">来自 Apple 的 VPP 令牌仅可与一个提供程序一起使用。</span><span class="sxs-lookup"><span data-stu-id="38ccc-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="38ccc-107">如果将 VPP 令牌与多个提供程序一起使用, 则必须将令牌重新上载到 Intune。</span><span class="sxs-lookup"><span data-stu-id="38ccc-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="38ccc-108">如果安装总数超过许可证数量, 安装也可能会失败。</span><span class="sxs-lookup"><span data-stu-id="38ccc-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="38ccc-109">若要查看许可证的使用率报告, 请转到**Intune 移动应用** \> **应用程序许可证**页。</span><span class="sxs-lookup"><span data-stu-id="38ccc-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="38ccc-110">若要了解如何回收使用中的许可证, 请参阅[本文。](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="38ccc-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
