---
title: 解决在 Microsoft Intune 中注册 Windows 设备时出现的问题
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658868"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="c2ac7-102">解决在 Microsoft Intune 中注册 Windows 设备时出现的问题</span><span class="sxs-lookup"><span data-stu-id="c2ac7-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="c2ac7-103">立即查看下面列出的资源，以解决问题。</span><span class="sxs-lookup"><span data-stu-id="c2ac7-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="c2ac7-104">一些常见的错误消息和解决步骤：</span><span class="sxs-lookup"><span data-stu-id="c2ac7-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="c2ac7-105">**无法安装软件，0x80cf4017：** 你的帐户证书已过期。</span><span class="sxs-lookup"><span data-stu-id="c2ac7-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="c2ac7-106">在 Intune 管理控制台中重新下载 PC 客户端软件程序包。</span><span class="sxs-lookup"><span data-stu-id="c2ac7-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="c2ac7-107">有关详细信息，请参阅本文档。</span><span class="sxs-lookup"><span data-stu-id="c2ac7-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="c2ac7-108">**错误代码0x801c0003：** 在下列情况下可能会发生此错误：</span><span class="sxs-lookup"><span data-stu-id="c2ac7-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="c2ac7-109">用户已注册的设备超过设备限制。</span><span class="sxs-lookup"><span data-stu-id="c2ac7-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="c2ac7-110">查看这些文档以 [删除设备](https://docs.microsoft.com/intune/devices-wipe) 或 [更改设备限制](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)。</span><span class="sxs-lookup"><span data-stu-id="c2ac7-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="c2ac7-111">"用户可以将设备加入 Azure AD" 设置为 "无"。</span><span class="sxs-lookup"><span data-stu-id="c2ac7-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="c2ac7-112">将其设置为 "所有用户" 或 "选择用户"。</span><span class="sxs-lookup"><span data-stu-id="c2ac7-112">Set it to all or select users.</span></span> <span data-ttu-id="c2ac7-113">有关详细信息，请参阅 [本文档](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) 。</span><span class="sxs-lookup"><span data-stu-id="c2ac7-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="c2ac7-114">设备已由其他用户注册。</span><span class="sxs-lookup"><span data-stu-id="c2ac7-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="c2ac7-115">如果是这种情况，请从 Azure Intune 控制台中删除该设备，或手动取消注册该设备，然后重试。</span><span class="sxs-lookup"><span data-stu-id="c2ac7-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="c2ac7-116">设备是 Windows 10 家庭版。</span><span class="sxs-lookup"><span data-stu-id="c2ac7-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="c2ac7-117">仅 Windows 10 专业版、教育版和企业版 Sku 可以加入 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="c2ac7-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="c2ac7-118">帮助解决你的问题的其他资源：</span><span class="sxs-lookup"><span data-stu-id="c2ac7-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="c2ac7-119">使用 [Intune 故障排除门户](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) 诊断和解决常见注册故障。</span><span class="sxs-lookup"><span data-stu-id="c2ac7-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="c2ac7-120">有关详细信息，请查看 [此文档](https://docs.microsoft.com/intune/help-desk-operators) 。</span><span class="sxs-lookup"><span data-stu-id="c2ac7-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="c2ac7-121">有关阻止注册的一系列常见错误及其解决方案，请查看以下文档：[故障排除指南](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)和[疑难解答文档](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)。</span><span class="sxs-lookup"><span data-stu-id="c2ac7-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="c2ac7-122">[了解如何在 Microsoft Intune 中注册 Windows 设备](https://docs.microsoft.com/intune/windows-enroll)。</span><span class="sxs-lookup"><span data-stu-id="c2ac7-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
