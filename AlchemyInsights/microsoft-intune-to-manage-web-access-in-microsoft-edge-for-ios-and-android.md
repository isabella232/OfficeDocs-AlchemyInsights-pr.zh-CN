---
title: 使用 Microsoft Intune 在适用于 iOS 和 Android Microsoft Edge管理 Web 访问
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003846"
- "6895"
- "9006502"
- "11144"
ms.openlocfilehash: a6c6f9563933b7cf6b71c4758c29ffd94617c4be
ms.sourcegitcommit: 7a406a3d4680662e81f0056454f7e25fb2f52504
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52989647"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="d100b-102">使用 Microsoft Intune 在适用于 iOS 和 Android Microsoft Edge管理 Web 访问</span><span class="sxs-lookup"><span data-stu-id="d100b-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="d100b-103">Microsoft Edge适用于 iOS 和 Android 的配置文件允许用户从多个完全独立的配置文件浏览 Web。</span><span class="sxs-lookup"><span data-stu-id="d100b-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="d100b-104">订阅 企业移动性 + 安全性 套件时，Microsoft 365数据的最广泛保护功能（包括 Microsoft Intune 和 Azure Active Directory Premium 功能，如条件访问）。</span><span class="sxs-lookup"><span data-stu-id="d100b-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="d100b-105">至少需要部署一个条件访问策略，即 (1) 允许用户从移动设备连接到 Microsoft Edge for iOS 和 Android，并且 (2) 实现提供受保护浏览体验的 Microsoft Intune 应用保护策略。</span><span class="sxs-lookup"><span data-stu-id="d100b-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="d100b-106">若要了解如何使用条件访问和策略，请参阅：</span><span class="sxs-lookup"><span data-stu-id="d100b-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="d100b-107">应用Azure Active Directory访问策略</span><span class="sxs-lookup"><span data-stu-id="d100b-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="d100b-108">创建Microsoft Intune应用保护策略</span><span class="sxs-lookup"><span data-stu-id="d100b-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="d100b-109">在策略保护的Azure Active Directory中对连接的 Web 应用使用单一登录</span><span class="sxs-lookup"><span data-stu-id="d100b-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="d100b-110">使用应用配置管理浏览体验</span><span class="sxs-lookup"><span data-stu-id="d100b-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="d100b-111">仅允许使用工作和学校帐户</span><span class="sxs-lookup"><span data-stu-id="d100b-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="d100b-112">部署常规应用配置策略</span><span class="sxs-lookup"><span data-stu-id="d100b-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="d100b-113">部署数据保护的应用配置策略</span><span class="sxs-lookup"><span data-stu-id="d100b-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="d100b-114">使用Microsoft Endpoint Manager部署应用配置策略</span><span class="sxs-lookup"><span data-stu-id="d100b-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="d100b-115">若要了解如何访问托管的应用日志，请参阅使用[Microsoft Edge for iOS 和 Android 访问托管的应用日志](https://go.microsoft.com/fwlink/?linkid=2132578)。</span><span class="sxs-lookup"><span data-stu-id="d100b-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
