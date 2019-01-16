---
title: 解决问题注册 Microsoft Intune 中的 Windows 设备
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8d19bbd5a5782c7793c87499baf62b2eb7de82ae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28277855"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="1c01d-102">解决问题注册 Microsoft Intune 中的 Windows 设备</span><span class="sxs-lookup"><span data-stu-id="1c01d-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="1c01d-103">查看下列来解决此问题现在资源。</span><span class="sxs-lookup"><span data-stu-id="1c01d-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="1c01d-104">某些常见错误消息和解决步骤：</span><span class="sxs-lookup"><span data-stu-id="1c01d-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="1c01d-p101">**无法安装该软件，0x80cf4017:** 帐户证书已过期。重新下载 PC 客户端软件程序包 Intune 管理控制台中。查看此文档的详细信息。</span><span class="sxs-lookup"><span data-stu-id="1c01d-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="1c01d-108">**错误代码 0x801c0003:** 在下列情况下可能会发生错误：</span><span class="sxs-lookup"><span data-stu-id="1c01d-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="1c01d-p102">用户具有更多注册超过设备限制的设备。查看这些文档给[删除设备](https://docs.microsoft.com/en-us/intune/devices-wipe)或[更改设备限制](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions)。</span><span class="sxs-lookup"><span data-stu-id="1c01d-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/en-us/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="1c01d-p103">"ヘ ・ 络设备到 Azure AD"设置为"none"。设置为 all，或选择用户。查看[此文档](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="1c01d-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="1c01d-p104">已由另一个用户注册设备。如果是这样，从 Azure Intune 控制台删除设备或手动 unenroll 设备，然后重试。</span><span class="sxs-lookup"><span data-stu-id="1c01d-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="1c01d-p105">设备是主 Windows 10。只有 Windows 10 专业人员、 培训和企业 Sku 可以加入 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="1c01d-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="1c01d-118">更多资源以帮助解决您的问题：</span><span class="sxs-lookup"><span data-stu-id="1c01d-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="1c01d-p106">使用[Intune 疑难解答门户](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)诊断和解决常见注册失败。查看[此文档](https://docs.microsoft.com/en-us/intune/help-desk-operators)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="1c01d-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="1c01d-121">查看这些文档中的每个阻止注册和解析的常见错误列表：[疑难解答指南](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)和[疑难解答文档](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)。</span><span class="sxs-lookup"><span data-stu-id="1c01d-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="1c01d-122">[了解如何注册 Microsoft Intune 中的 Windows 设备](https://docs.microsoft.com/en-us/intune/windows-enroll)。</span><span class="sxs-lookup"><span data-stu-id="1c01d-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).</span></span>
  

