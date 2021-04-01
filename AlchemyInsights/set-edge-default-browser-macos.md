---
title: 将 Microsoft Edge 设置为 macOS 设备上的默认浏览器
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426771"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="7bd00-102">将 Microsoft Edge 设置为 macOS 设备上的默认浏览器</span><span class="sxs-lookup"><span data-stu-id="7bd00-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="7bd00-103">使用以下两种方法之一将 Microsoft Edge 设置为默认浏览器：</span><span class="sxs-lookup"><span data-stu-id="7bd00-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="7bd00-104">方法 1：使用已将 Microsoft Edge 设置为默认浏览器的 macOS 映像刷新设备。</span><span class="sxs-lookup"><span data-stu-id="7bd00-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="7bd00-105">方法 2：将 DefaultBrowserSettingEnabled 策略设置为提示用户将 Microsoft Edge 设置为默认浏览器。</span><span class="sxs-lookup"><span data-stu-id="7bd00-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="7bd00-106">这两种方法都允许用户更改默认浏览器。</span><span class="sxs-lookup"><span data-stu-id="7bd00-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="7bd00-107">因此，我们建议你即使使用了方法 1，也部署 DefaultBrowserSettingEnabled 策略。</span><span class="sxs-lookup"><span data-stu-id="7bd00-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="7bd00-108">如果用户在部署策略后更改了默认浏览器，则该策略会提示用户将默认浏览器设置回 Microsoft Edge。</span><span class="sxs-lookup"><span data-stu-id="7bd00-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
