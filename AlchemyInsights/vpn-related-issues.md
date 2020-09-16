---
title: VPN 相关问题
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 3c031725c92f5d7af7c0dd0c37ea34fecf4792c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47726081"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="996d1-102">VPN 相关问题</span><span class="sxs-lookup"><span data-stu-id="996d1-102">VPN related issues</span></span>

<span data-ttu-id="996d1-103">成功实现 MDM 客户端的 VPN 连接取决于已部署的配置文件，此配置文件可正确反映 VPN 基础结构的要求。</span><span class="sxs-lookup"><span data-stu-id="996d1-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="996d1-104">有关正在调查的客户端平台的相应设置，请参阅：</span><span class="sxs-lookup"><span data-stu-id="996d1-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="996d1-105">使用 Intune 添加 VPN 连接的 Windows 10 和 Windows 全息设备设置</span><span class="sxs-lookup"><span data-stu-id="996d1-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="996d1-106">在 Microsoft Intune 中添加 iOS 和 iPadOS 设备 VPN 设置</span><span class="sxs-lookup"><span data-stu-id="996d1-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="996d1-107">Intune 中配置 VPN 的 Android 设备设置</span><span class="sxs-lookup"><span data-stu-id="996d1-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="996d1-108">在 Microsoft Intune 中添加 macOS 设备 VPN 设置</span><span class="sxs-lookup"><span data-stu-id="996d1-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="996d1-109">如果你的 VPN 配置文件使用基于证书的身份验证，请确保已成功部署链接到 VPN 配置文件的根证书和客户端身份验证证书配置文件。</span><span class="sxs-lookup"><span data-stu-id="996d1-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="996d1-110">**常见问题**</span><span class="sxs-lookup"><span data-stu-id="996d1-110">**Common Issues**</span></span>

<span data-ttu-id="996d1-111">**我将 VPN 配置文件部署到设备。 Intune 显示已成功，但设备未连接到VPN。**</span><span class="sxs-lookup"><span data-stu-id="996d1-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="996d1-112">成功状态表示 Intune 已按照配置成功部署了配置文件。</span><span class="sxs-lookup"><span data-stu-id="996d1-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="996d1-113">但是，这些配置可能不符合您的网络和/或身份验证要求。</span><span class="sxs-lookup"><span data-stu-id="996d1-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="996d1-114">查看基础设施和身份验证服务中的日志（在 VPN 服务器和 NPS / Radius 服务器上），以获取有关尝试的连接的更多详细信息。</span><span class="sxs-lookup"><span data-stu-id="996d1-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="996d1-115">可能需要与网络基础设施团队或第三方 VPN 供应商合作，以收集和查看日志。</span><span class="sxs-lookup"><span data-stu-id="996d1-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="996d1-116">**配置适用于 iOS 的自定义 VPN 时，每应用 VPN 功能不可用。**</span><span class="sxs-lookup"><span data-stu-id="996d1-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="996d1-117">当前，Intune 中适用于 iOS 设备的每应用程序 VPN 适用于特定的提供商和合作伙伴列表，配置每应用 VPN 之前，还必须满足证书的先决条件。</span><span class="sxs-lookup"><span data-stu-id="996d1-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="996d1-118">有关更多信息，请参阅[在 Intune 中为 iOS / iPadOS 设备设置每个应用程序的虚拟专用网络 (VPN)](https://docs.microsoft.com/intune/vpn-setting-configure-per-app)。</span><span class="sxs-lookup"><span data-stu-id="996d1-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="996d1-119">有关 Intune 中所有 VPN 连接类型的详细信息，请参阅[创建 VPN 配置文件以连接到 Intune 中的 VPN 服务器](https://docs.microsoft.com/intune/vpn-settings-configure)。</span><span class="sxs-lookup"><span data-stu-id="996d1-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="996d1-120">**访问配置的域时，iOS 按需 VPN 未触发**</span><span class="sxs-lookup"><span data-stu-id="996d1-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="996d1-121">要测试自动 VPN 设置，请设定以下值：</span><span class="sxs-lookup"><span data-stu-id="996d1-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="996d1-122">我要执行以下操作：**评估每一连接尝试**</span><span class="sxs-lookup"><span data-stu-id="996d1-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="996d1-123">选择是否连接：**根据需要连接**</span><span class="sxs-lookup"><span data-stu-id="996d1-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="996d1-124">用户访问以下域时：**目标** *域名*</span><span class="sxs-lookup"><span data-stu-id="996d1-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="996d1-125">如果以上配置不成功，请添加以下元素：</span><span class="sxs-lookup"><span data-stu-id="996d1-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="996d1-126">无法访问该 URL 时，强制连接 VPN： **BADURL**</span><span class="sxs-lookup"><span data-stu-id="996d1-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>