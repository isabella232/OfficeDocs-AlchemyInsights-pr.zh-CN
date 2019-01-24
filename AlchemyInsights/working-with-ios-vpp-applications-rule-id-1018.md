---
title: 使用 iOS VPP 应用程序规则 Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 5bcfb6dd7222bd102ff2620c19bfb943e7bd9591
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29459583"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="3ceb8-102">使用 iOS VPP 应用程序</span><span class="sxs-lookup"><span data-stu-id="3ceb8-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="3ceb8-103">阅读了解功能、 约束和步骤，以使[如何管理与 Microsoft Intune 卷购买程序通过购买的 iOS 应用程序](https://docs.microsoft.com/intune/vpp-apps-ios)使用的 Apple 卷购买程序以及为其 Microsoft Intune 中的支持。</span><span class="sxs-lookup"><span data-stu-id="3ceb8-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="3ceb8-104">**常见问题：**"已在 iOS VPP 应用分配给我的用户，但安装失败。"</span><span class="sxs-lookup"><span data-stu-id="3ceb8-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="3ceb8-p101">如果跨多个移动设备管理提供程序使用单个 VPP 标记，则可能发生错误。Apple VPP 令牌仅可与一个提供程序。如果在 VPP 令牌使用多个提供程序，您必须重新上载到 Intune 的令牌。</span><span class="sxs-lookup"><span data-stu-id="3ceb8-p101">This can happen if a single VPP token is used across multiple mobile device management providers. VPP tokens from Apple may only be used with one provider. If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="3ceb8-p102">如果安装的总数超过许可证数量，也可以失败安装。若要查看您的许可证使用情况报告，请转到**Intune 移动应用程序** \> **应用程序许可证**页。若要了解如何回收中使用的许可证，请参阅[本文。](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="3ceb8-p102">The installation can also fail if the total number of installations exceed the number of licenses. To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page. To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

