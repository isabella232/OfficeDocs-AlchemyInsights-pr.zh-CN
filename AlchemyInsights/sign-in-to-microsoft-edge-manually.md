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
- "8332"
- "9004625"
ms.openlocfilehash: f380d09dc14788205638cdee6aebe0b084ecab2f
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398647"
---
# <a name="sign-in-to-microsoft-edge-manually"></a><span data-ttu-id="4f447-102">手动登录到 Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="4f447-102">Sign in to Microsoft Edge manually</span></span>

<span data-ttu-id="4f447-103">如果用户在首次运行体验期间未自动登录，则用户可以通过浏览器的设置或标识飞出区手动登录。</span><span class="sxs-lookup"><span data-stu-id="4f447-103">If a user isn't automatically signed in during a first-run experience, the user can manually sign in through the browser's settings or the identity flyout.</span></span> <span data-ttu-id="4f447-104">若要管理登录，请使用以下策略：</span><span class="sxs-lookup"><span data-stu-id="4f447-104">To manage sign-in, use the following policies:</span></span>

1. <span data-ttu-id="4f447-105">[NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) - 确保用户在 Microsoft Edge 中始终具有工作配置文件。</span><span class="sxs-lookup"><span data-stu-id="4f447-105">[NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) - To ensure that a user always has a work profile in Microsoft Edge.</span></span>
2. <span data-ttu-id="4f447-106">[RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) - 限制登录一组受信任帐户。</span><span class="sxs-lookup"><span data-stu-id="4f447-106">[RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) - To restrict sign-in to a set of trusted accounts.</span></span>
3. <span data-ttu-id="4f447-107">[BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) - 禁用登录或强制用户登录。</span><span class="sxs-lookup"><span data-stu-id="4f447-107">[BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) - To disable sign-in or to force users to sign in.</span></span>

