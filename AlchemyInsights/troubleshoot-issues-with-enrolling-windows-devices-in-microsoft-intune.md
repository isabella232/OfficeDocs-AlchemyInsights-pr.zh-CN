---
title: 解决问题注册 Microsoft Intune 中的 Windows 设备
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: aa2262ed487ae4160f13490e92163a145e657862
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934766"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="93838-102">解决问题注册 Microsoft Intune 中的 Windows 设备</span><span class="sxs-lookup"><span data-stu-id="93838-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="93838-103">查看下列来解决此问题现在资源。</span><span class="sxs-lookup"><span data-stu-id="93838-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="93838-104">某些常见错误消息和解决步骤：</span><span class="sxs-lookup"><span data-stu-id="93838-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="93838-p101">**无法安装该软件，0x80cf4017:** 帐户证书已过期。重新下载 PC 客户端软件程序包 Intune 管理控制台中。查看此文档的详细信息。</span><span class="sxs-lookup"><span data-stu-id="93838-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="93838-108">**错误代码 0x801c0003:** 在下列情况下可能会发生错误：</span><span class="sxs-lookup"><span data-stu-id="93838-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="93838-p102">用户具有更多注册超过设备限制的设备。查看这些文档给[删除设备](https://docs.microsoft.com/intune/devices-wipe)或[更改设备限制](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)。</span><span class="sxs-lookup"><span data-stu-id="93838-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="93838-p103">"ヘ ・ 络设备到 Azure AD"设置为"none"。设置为 all，或选择用户。查看[此文档](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="93838-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="93838-p104">已由另一个用户注册设备。如果是这样，从 Azure Intune 控制台删除设备或手动 unenroll 设备，然后重试。</span><span class="sxs-lookup"><span data-stu-id="93838-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="93838-p105">设备是主 Windows 10。只有 Windows 10 专业人员、 培训和企业 Sku 可以加入 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="93838-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="93838-118">更多资源以帮助解决您的问题：</span><span class="sxs-lookup"><span data-stu-id="93838-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="93838-p106">使用[Intune 疑难解答门户](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)诊断和解决常见注册失败。查看[此文档](https://docs.microsoft.com/intune/help-desk-operators)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="93838-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="93838-121">查看这些文档中的每个阻止注册和解析的常见错误列表：[疑难解答指南](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)和[疑难解答文档](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)。</span><span class="sxs-lookup"><span data-stu-id="93838-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="93838-122">[了解如何注册 Microsoft Intune 中的 Windows 设备](https://docs.microsoft.com/intune/windows-enroll)。</span><span class="sxs-lookup"><span data-stu-id="93838-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
  

