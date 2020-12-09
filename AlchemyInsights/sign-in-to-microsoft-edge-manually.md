---
title: 手动登录到 Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
ms.openlocfilehash: c5d71c26ba3584f8ce496a28587fe75cae2d344f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599455"
---
# <a name="sign-in-to-microsoft-edge-manually"></a><span data-ttu-id="00ddb-102">手动登录到 Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="00ddb-102">Sign in to Microsoft Edge manually</span></span>

<span data-ttu-id="00ddb-103">如果用户在首次运行体验期间未自动登录，则用户可以通过浏览器的设置或 "标识" 浮出控件进行手动登录。</span><span class="sxs-lookup"><span data-stu-id="00ddb-103">If a user isn't automatically signed in during a first-run experience, the user can manually sign in through the browser's settings or the identity flyout.</span></span> <span data-ttu-id="00ddb-104">若要管理登录，请使用以下策略：</span><span class="sxs-lookup"><span data-stu-id="00ddb-104">To manage sign-in, use the following policies:</span></span>

1. <span data-ttu-id="00ddb-105">[NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) -确保用户在 Microsoft Edge 中始终有工作配置文件。</span><span class="sxs-lookup"><span data-stu-id="00ddb-105">[NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) - To ensure that a user always has a work profile in Microsoft Edge.</span></span>
2. <span data-ttu-id="00ddb-106">[RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) -将登录限制为一组受信任的帐户。</span><span class="sxs-lookup"><span data-stu-id="00ddb-106">[RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) - To restrict sign-in to a set of trusted accounts.</span></span>
3. <span data-ttu-id="00ddb-107">[BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) -要禁用登录或强制用户登录。</span><span class="sxs-lookup"><span data-stu-id="00ddb-107">[BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) - To disable sign-in or to force users to sign in.</span></span>

