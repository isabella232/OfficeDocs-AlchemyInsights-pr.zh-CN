---
title: 解决问题注册 Microsoft Intune 在 iOS 设备
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: cd1afc83fe98f363aee4c3324a634c200cd08947
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29658429"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="57fa1-102">解决问题注册 Microsoft Intune 在 iOS 设备</span><span class="sxs-lookup"><span data-stu-id="57fa1-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="57fa1-103">查看下列来解决此问题现在资源。</span><span class="sxs-lookup"><span data-stu-id="57fa1-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="57fa1-104">某些常见错误消息和解决步骤：</span><span class="sxs-lookup"><span data-stu-id="57fa1-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="57fa1-p101">**设备帽达到**用户具有更多注册超过设备限制的设备。查看这些文档给[删除设备](https://docs.microsoft.com/intune/devices-wipe)或[更改设备限制](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)。</span><span class="sxs-lookup"><span data-stu-id="57fa1-p101">**Device Cap Reached** The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="57fa1-p102">不支持**此服务。没有注册策略：** Apple 推送通知服务 (APNS) 需要配置或续订。查看[此文档](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get)有关执行该操作的说明。</span><span class="sxs-lookup"><span data-stu-id="57fa1-p102">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed. Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="57fa1-p103">**用户许可证类型无效或无法识别用户名称：** 用户需要分配一个 Intune 或 EMS 许可证。查看这些文档，以将通过许可证分配： [Office 管理中心](https://docs.microsoft.com/intune/licenses-assign)或[Azure 门户](https://docs.microsoft.com/azure/active-directory/license-users-groups)。</span><span class="sxs-lookup"><span data-stu-id="57fa1-p103">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="57fa1-111">更多资源以帮助解决您的问题：</span><span class="sxs-lookup"><span data-stu-id="57fa1-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="57fa1-p104">使用[Intune 疑难解答门户](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)诊断和解决常见注册失败。查看[此文档](https://docs.microsoft.com/intune/help-desk-operators)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="57fa1-p104">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="57fa1-114">查看这些文档中的每个阻止注册和解析的常见错误列表：[疑难解答指南](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune)和[疑难解答文档](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)。</span><span class="sxs-lookup"><span data-stu-id="57fa1-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="57fa1-115">[了解如何注册 Microsoft Intune 在 iOS 设备](https://docs.microsoft.com/intune/ios-enroll)。</span><span class="sxs-lookup"><span data-stu-id="57fa1-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

