---
title: 解决在 Microsoft Intune 中注册 iOS 设备的问题
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823453"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="e47bd-102">解决在 Microsoft Intune 中注册 iOS 设备的问题</span><span class="sxs-lookup"><span data-stu-id="e47bd-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="e47bd-103">查看下面列出的资源，以现在解决问题。</span><span class="sxs-lookup"><span data-stu-id="e47bd-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="e47bd-104">一些常见的错误消息和解决方法步骤：</span><span class="sxs-lookup"><span data-stu-id="e47bd-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="e47bd-105">**已达到设备上限** 用户注册的设备数超过设备限制。</span><span class="sxs-lookup"><span data-stu-id="e47bd-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="e47bd-106">查看这些文档[以删除设备](https://docs.microsoft.com/intune/devices-wipe)[或更改设备限制](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)。</span><span class="sxs-lookup"><span data-stu-id="e47bd-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="e47bd-107">**不支持此服务。无注册策略：** 需要 (或续订 APNS) Apple 推送通知服务。</span><span class="sxs-lookup"><span data-stu-id="e47bd-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="e47bd-108">查看 [本文档](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) ，了解如何操作。</span><span class="sxs-lookup"><span data-stu-id="e47bd-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="e47bd-109">**用户许可证类型无效或用户名无法识别：** 需要为用户分配 Intune 或 EMS 许可证。</span><span class="sxs-lookup"><span data-stu-id="e47bd-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="e47bd-110">查看以下文档以通过以下方式分配许可证 [：Office 管理中心或](https://docs.microsoft.com/intune/licenses-assign) [Azure 门户](https://docs.microsoft.com/azure/active-directory/license-users-groups)。</span><span class="sxs-lookup"><span data-stu-id="e47bd-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="e47bd-111">有助于解决问题的其他资源：</span><span class="sxs-lookup"><span data-stu-id="e47bd-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="e47bd-112">使用 [Intune 疑难解答门户](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) 诊断和解决常见的注册失败。</span><span class="sxs-lookup"><span data-stu-id="e47bd-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="e47bd-113">有关详细信息 [，](https://docs.microsoft.com/intune/help-desk-operators) 请查看本文档。</span><span class="sxs-lookup"><span data-stu-id="e47bd-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="e47bd-114">有关阻止注册的一系列常见错误及其解决方案，请查看以下文档：[故障排除指南](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune)和[疑难解答文档](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)。</span><span class="sxs-lookup"><span data-stu-id="e47bd-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="e47bd-115">[了解如何在 Microsoft Intune 中注册 iOS 设备](https://docs.microsoft.com/intune/ios-enroll)。</span><span class="sxs-lookup"><span data-stu-id="e47bd-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

