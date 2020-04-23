---
title: 解决在 Microsoft Intune 中注册 iOS 设备的问题
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736148"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="35535-102">解决在 Microsoft Intune 中注册 iOS 设备的问题</span><span class="sxs-lookup"><span data-stu-id="35535-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="35535-103">立即查看下面列出的资源，以解决问题。</span><span class="sxs-lookup"><span data-stu-id="35535-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="35535-104">一些常见的错误消息和解决步骤：</span><span class="sxs-lookup"><span data-stu-id="35535-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="35535-105">已**达到设备上限**用户已注册的设备超过设备限制。</span><span class="sxs-lookup"><span data-stu-id="35535-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="35535-106">查看这些文档以[删除设备](https://docs.microsoft.com/intune/devices-wipe)或[更改设备限制](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)。</span><span class="sxs-lookup"><span data-stu-id="35535-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="35535-107">**不支持此服务。无注册策略：** 需要配置或续订 Apple 推送通知服务（APNS）。</span><span class="sxs-lookup"><span data-stu-id="35535-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="35535-108">查看[此文档](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get)以了解如何执行此操作的说明。</span><span class="sxs-lookup"><span data-stu-id="35535-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="35535-109">**用户许可证类型无效或无法识别用户名称：** 需要向用户分配 Intune 或 EMS 许可证。</span><span class="sxs-lookup"><span data-stu-id="35535-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="35535-110">查看这些文档以通过以下步骤分配许可证： [Office 管理中心](https://docs.microsoft.com/intune/licenses-assign)或[Azure 门户](https://docs.microsoft.com/azure/active-directory/license-users-groups)。</span><span class="sxs-lookup"><span data-stu-id="35535-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="35535-111">帮助解决你的问题的其他资源：</span><span class="sxs-lookup"><span data-stu-id="35535-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="35535-112">使用[Intune 故障排除门户](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)诊断和解决常见注册故障。</span><span class="sxs-lookup"><span data-stu-id="35535-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="35535-113">有关详细信息，请查看[此文档](https://docs.microsoft.com/intune/help-desk-operators)。</span><span class="sxs-lookup"><span data-stu-id="35535-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="35535-114">查看这些文档，了解阻止对每个的注册和解决的常见错误的列表：[故障排除指南](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune)和[疑难解答文档](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)。</span><span class="sxs-lookup"><span data-stu-id="35535-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="35535-115">[了解如何在 Microsoft Intune 中注册 iOS 设备](https://docs.microsoft.com/intune/ios-enroll)。</span><span class="sxs-lookup"><span data-stu-id="35535-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

