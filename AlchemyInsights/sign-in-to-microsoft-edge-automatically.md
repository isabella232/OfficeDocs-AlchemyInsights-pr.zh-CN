---
title: 自动登录到 Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599443"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="3d3eb-102">自动登录到 Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="3d3eb-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="3d3eb-103">Microsoft Edge 根据用户设备的配置方式，使用 OS 的默认帐户自动登录用户。</span><span class="sxs-lookup"><span data-stu-id="3d3eb-103">Microsoft Edge uses the OS's default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="3d3eb-104">以下介绍每种类型的设备配置及其相关用户登录进程的方案：</span><span class="sxs-lookup"><span data-stu-id="3d3eb-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

1. <span data-ttu-id="3d3eb-105">**设备是混合型/AAD-J**：此选项在 windows 10、下层 windows 和相应的服务器版本上可用。</span><span class="sxs-lookup"><span data-stu-id="3d3eb-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="3d3eb-106">将使用 Azure Active Directory (AD) 帐户自动登录用户。</span><span class="sxs-lookup"><span data-stu-id="3d3eb-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
2. <span data-ttu-id="3d3eb-107">**设备已加入域**：此选项在 windows 10、下层 windows 和相应的服务器版本上可用。</span><span class="sxs-lookup"><span data-stu-id="3d3eb-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="3d3eb-108">默认情况下，不会自动登录具有域帐户的用户;若要为其启用自动登录，请使用 **ConfigureOnPremisesAccountAutoSignIn** 策略。</span><span class="sxs-lookup"><span data-stu-id="3d3eb-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="3d3eb-109">若要为使用 Azure AD 帐户的用户启用自动登录，请考虑混合加入其设备。</span><span class="sxs-lookup"><span data-stu-id="3d3eb-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
3. <span data-ttu-id="3d3eb-110">**OS 的默认帐户是 Microsoft 帐户**：在 WINDOWS 10 RS3 上提供此选项。 (版本1709，构建 10.0.16299) 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="3d3eb-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="3d3eb-111">企业设备上可能不会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="3d3eb-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="3d3eb-112">但是，如果 OS 的默认帐户是 Microsoft 帐户，则 Microsoft Edge 将使用 Microsoft 帐户自动登录用户。</span><span class="sxs-lookup"><span data-stu-id="3d3eb-112">However, if the OS's default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
