---
title: 由于使用符合条件的设备被条件访问阻止
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897525"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a><span data-ttu-id="a3952-102">由于使用符合条件的设备被条件访问阻止</span><span class="sxs-lookup"><span data-stu-id="a3952-102">I’m getting blocked by Conditional Access with compliant device</span></span>

<span data-ttu-id="a3952-103">**强烈建议使用的工具**</span><span class="sxs-lookup"><span data-stu-id="a3952-103">**Highly Recommended Tools**</span></span>

- <span data-ttu-id="a3952-104">[设备注册疑难解答](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) 工具 - 一种全面的工具，可帮助解决最常见的设备注册问题。</span><span class="sxs-lookup"><span data-stu-id="a3952-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - A comprehensive tool that helps troubleshoot the most common device registration issues.</span></span>
- <span data-ttu-id="a3952-105">[测试设备注册连接脚本](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - 一种用于确保设备可以访问系统帐户下的设备注册终结点的工具。</span><span class="sxs-lookup"><span data-stu-id="a3952-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - A tool used to ensure that a device can access Device Registration endpoints under the system account.</span></span>
- <span data-ttu-id="a3952-106">[Azure AD 设备清理脚本](https://github.com/mzmaili/AzureADDeviceCleanup) - 一种用于查找和管理环境中过时的设备的工具。</span><span class="sxs-lookup"><span data-stu-id="a3952-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - A tool used to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="a3952-107">以下是条件访问可能会失败（针对合规性设备）的一些常见原因，或者为什么用户可能会收到 **你在向组织资源登录请求期间收到** 邮件。</span><span class="sxs-lookup"><span data-stu-id="a3952-107">Here are some common reasons why Conditional Access may be failing for a compliant device or why your users may be receiving **You can't get there from here** message during a sign-in request to an organizational resource.</span></span>

1. <span data-ttu-id="a3952-108">**设备不是 MDM 要求的设备状态**：</span><span class="sxs-lookup"><span data-stu-id="a3952-108">**Device is not in a required device state with an MDM**:</span></span>

<span data-ttu-id="a3952-109">验证设备是否向批准的 MDM 提供商如 Intune 和 *标记为*。</span><span class="sxs-lookup"><span data-stu-id="a3952-109">Validate that the device is enrolled with an approved MDM provider like Intune and *marked as compliant*.</span></span> <span data-ttu-id="a3952-110">有关 Intune 详细信息，请参阅此 [文档](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment)。</span><span class="sxs-lookup"><span data-stu-id="a3952-110">For more information on Intune see this [document](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment).</span></span> <span data-ttu-id="a3952-111">若要更好地了解设备合规性和 Intune，请参阅 [合规性策略为通过 Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)管理的设备设置规则。</span><span class="sxs-lookup"><span data-stu-id="a3952-111">For better understanding of device compliance and Intune, see [use compliance policy to set rules for devices you manage with Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started).</span></span> <span data-ttu-id="a3952-112">如果在使用 Intune 注册设备时遇到问题，请参阅 在 Microsoft [中解决设备注册问题并查找](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)。</span><span class="sxs-lookup"><span data-stu-id="a3952-112">If you are having issues enrolling a device with Intune, find troubleshooting details at [Troubleshoot device enrollment in Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span> <span data-ttu-id="a3952-113">若要进一步获得 Intune 支持，请创建支持请求。</span><span class="sxs-lookup"><span data-stu-id="a3952-113">For further Intune support, create a support request.</span></span> <span data-ttu-id="a3952-114">若要实现此点，请访问 [的 Intune 帮助和支持页面](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport)。</span><span class="sxs-lookup"><span data-stu-id="a3952-114">To do so, visit the [Intune Help and Support page](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).</span></span>

2. <span data-ttu-id="a3952-115">**设备未加入组织网络**：</span><span class="sxs-lookup"><span data-stu-id="a3952-115">**Device is not joined to the organizations network**:</span></span>

<span data-ttu-id="a3952-116">为访问组织资源，设备必须直接连接或虚拟专用网络 （VPN） 连接到组织的网络，并且还加入本地或 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="a3952-116">For access to organizational resources, the device has to be connected to the organization's network, either through direct connection or a virtual private network (VPN), and also joined to on-premise or Azure Active Directory.</span></span> <span data-ttu-id="a3952-117">若要将工作设备加入组织网络，请参阅 [将工作设备加入组织的网络](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network)。</span><span class="sxs-lookup"><span data-stu-id="a3952-117">To join a work device to the organization network, see [Join your work device to your organization's network](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network).</span></span> <span data-ttu-id="a3952-118">要注册个人/BYOD 设备，请参阅 [组织网络共享设备上注册个人](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)。</span><span class="sxs-lookup"><span data-stu-id="a3952-118">To register a personal/BYOD device, see [Register your personal device on your organization's network](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).</span></span>

- <span data-ttu-id="a3952-119">若要验证设备是否已加入网络，可在[此处](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered)工作设备[步骤](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined)。</span><span class="sxs-lookup"><span data-stu-id="a3952-119">To validate whether the device has joined the network, you can follow the steps for registered devices [here](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) or work devices [here](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined).</span></span> <span data-ttu-id="a3952-120">若要将问题的范围界定到组织网络连接，请按照以下准则操作：</span><span class="sxs-lookup"><span data-stu-id="a3952-120">To scope the issue to Org network connectivity, follow guidelines below:</span></span>

    1. <span data-ttu-id="a3952-121">使用工作或学校帐户（例如 alain@contoso.com）登录 Windows。</span><span class="sxs-lookup"><span data-stu-id="a3952-121">Sign in to Windows using your work or school account,  for example, alain@contoso.com.</span></span>
    2. <span data-ttu-id="a3952-122">通过 VPN 或 DirectAccess 连接到组织的网络。</span><span class="sxs-lookup"><span data-stu-id="a3952-122">Connect to your organization's network through a VPN or DirectAccess.</span></span>
    3. <span data-ttu-id="a3952-123">连接后，按 **Windows 徽标键+L** 锁定设备。</span><span class="sxs-lookup"><span data-stu-id="a3952-123">After you're connected, press the **Windows logo key+L** to lock your device.</span></span>
    4. <span data-ttu-id="a3952-124">使用工作或学校帐户解锁设备，然后再次尝试访问有问题的应用和服务。</span><span class="sxs-lookup"><span data-stu-id="a3952-124">Unlock your device using your work or school account, and then try to access the problematic app or service again.</span></span>

<span data-ttu-id="a3952-125">如果你看到错误消息 **无法从此处再次看到错误消息** ，则问题可能还有其他位置。</span><span class="sxs-lookup"><span data-stu-id="a3952-125">If you see the **You can't get there from here** error message again, issue is likely elsewhere.</span></span>

3. <span data-ttu-id="a3952-126">**不支持操作系统：**：</span><span class="sxs-lookup"><span data-stu-id="a3952-126">**Operating system is not supported**:</span></span>

<span data-ttu-id="a3952-127">请确保正在运行的操作系统版本受支持，其中包括：</span><span class="sxs-lookup"><span data-stu-id="a3952-127">Ensure that you're running a supported version of the operating system, including:</span></span>

- <span data-ttu-id="a3952-128">**Windows 客户端**：Windows 7 或更高版本</span><span class="sxs-lookup"><span data-stu-id="a3952-128">**Windows Client**: Windows 7 or later</span></span>

- <span data-ttu-id="a3952-129">**Windows Server**：Windows Server 2008 R2 或更高版本</span><span class="sxs-lookup"><span data-stu-id="a3952-129">**Windows Server**: Windows Server 2008 R2 or later</span></span>

- <span data-ttu-id="a3952-130">**macOS**：macOS X 或更高版本</span><span class="sxs-lookup"><span data-stu-id="a3952-130">**macOS**: macOS X or later</span></span>

- <span data-ttu-id="a3952-131">**Android 和 iOS**：最新版本的 Android 和 iOS 移动操作系统</span><span class="sxs-lookup"><span data-stu-id="a3952-131">**Android and iOS**: Latest version of Android and iOS mobile operating systems</span></span>

4. <span data-ttu-id="a3952-132">**不支持 Web 浏览器**：</span><span class="sxs-lookup"><span data-stu-id="a3952-132">**Web browser is not supported**:</span></span>

<span data-ttu-id="a3952-133">请在下面找到支持的浏览器。</span><span class="sxs-lookup"><span data-stu-id="a3952-133">Please find supported browsers below.</span></span> <span data-ttu-id="a3952-134">Chrome 支持 Windows 1703 或更高版本，需要 Windows 10 帐户扩展。</span><span class="sxs-lookup"><span data-stu-id="a3952-134">For Chrome support with Windows 1703 or later versions, a Windows 10 Accounts extension is required.</span></span> <span data-ttu-id="a3952-135">对于 Edge 85+，用户需要登录以正确传递设备合规性信息。</span><span class="sxs-lookup"><span data-stu-id="a3952-135">For Edge 85+, the user needs to be signed in to properly pass device compliance information.</span></span> <span data-ttu-id="a3952-136">有关详细信息，请参阅 [此处](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)。</span><span class="sxs-lookup"><span data-stu-id="a3952-136">For more details, see [here](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

- <span data-ttu-id="a3952-137">**Windows 10**：Microsoft Edge、Internet Explorer、Chrome</span><span class="sxs-lookup"><span data-stu-id="a3952-137">**Windows 10**: Microsoft Edge, Internet Explorer, Chrome</span></span>
- <span data-ttu-id="a3952-138">**Windows 8/8.1**：Internet Explorer、Chrome</span><span class="sxs-lookup"><span data-stu-id="a3952-138">**Windows 8 / 8.1**: Internet Explorer, Chrome</span></span>
- <span data-ttu-id="a3952-139">**Windows 7**：Internet Explorer、Chrome</span><span class="sxs-lookup"><span data-stu-id="a3952-139">**Windows 7**: Internet Explorer, Chrome</span></span>
- <span data-ttu-id="a3952-140">**iOS**：Microsoft Edge、Intune 托管浏览器、Safari</span><span class="sxs-lookup"><span data-stu-id="a3952-140">**iOS**: Microsoft Edge, Intune Managed Browser, Safari</span></span>
- <span data-ttu-id="a3952-141">**Android**： **Microsoft Edge**：Intune 托管浏览器，Chrome</span><span class="sxs-lookup"><span data-stu-id="a3952-141">**Android**: **Microsoft Edge**: Intune Managed Browser, Chrome</span></span>
- <span data-ttu-id="a3952-142">**Windows Phone**：Microsoft Edge、Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="a3952-142">**Windows Phone**: Microsoft Edge, Internet Explorer</span></span>
- <span data-ttu-id="a3952-143">**Windows Server 2019**：Microsoft Edge、Internet Explorer、Chrome</span><span class="sxs-lookup"><span data-stu-id="a3952-143">**Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome</span></span>
- <span data-ttu-id="a3952-144">**Windows Server 2016 更新**：Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="a3952-144">**Windows Server 2016**: Internet Explorer</span></span>
- <span data-ttu-id="a3952-145">**Windows Server 2012 R2**：Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="a3952-145">**Windows Server 2012 R2**: Internet Explorer</span></span>
- <span data-ttu-id="a3952-146">**Windows Server 2008 R2**：Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="a3952-146">**Windows Server 2008 R2**: Internet Explorer</span></span>
- <span data-ttu-id="a3952-147">**macOS**：Chrome、Safari</span><span class="sxs-lookup"><span data-stu-id="a3952-147">**macOS**: Chrome, Safari</span></span>

<span data-ttu-id="a3952-148">在此处查找有关 **无法获取你的消息和疑难** 步骤 [此处](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)。</span><span class="sxs-lookup"><span data-stu-id="a3952-148">Find more information on the **You can't get there** message and troubleshooting steps [here](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation).</span></span>
