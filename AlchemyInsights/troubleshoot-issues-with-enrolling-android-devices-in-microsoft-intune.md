---
title: 解决问题注册中 Microsoft Intune Android 设备
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 0e727bd47a7d549a439e4666fa9dbb8a02e39778
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29939338"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="eac8f-102">解决问题注册中 Microsoft Intune Android 设备</span><span class="sxs-lookup"><span data-stu-id="eac8f-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="eac8f-103">查看下列来解决此问题现在资源。</span><span class="sxs-lookup"><span data-stu-id="eac8f-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="eac8f-104">一些常见的问题和解决步骤：</span><span class="sxs-lookup"><span data-stu-id="eac8f-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="eac8f-p101">**设备不加密的公司门户中的错误：** 较新版本的 Android，特别开头 7.0 版，需要启动密码以确保您的设备完全进行加密。常见的解决方案是启用启动 pin 或完全加密设备。查看[此文档](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="eac8f-p101">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted. Common solutions are to enable a startup pin or fully encrypt the device. Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span> 
  
 <span data-ttu-id="eac8f-p102">**设备无法检查使用 Intune 服务或 Intune 管理控制台中显示为"不正常":** 某些三星 4.4 和 5.5 设备可能未签入该服务。有 3 于此问题可能的解决方案：</span><span class="sxs-lookup"><span data-stu-id="eac8f-p102">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service. There are 3 possible solutions to this issue:</span></span> 
  
1. <span data-ttu-id="eac8f-110">手动打开 Intune 的公司门户应用程序，将自动启动设备同步。</span><span class="sxs-lookup"><span data-stu-id="eac8f-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>
    
2. <span data-ttu-id="eac8f-111">更新为 Android 6.0 或更高的设备。</span><span class="sxs-lookup"><span data-stu-id="eac8f-111">Update the device to Android 6.0 or higher.</span></span>
    
3. <span data-ttu-id="eac8f-p103">从管理 Intune 的公司门户中禁用三星智能管理器。查看[此文档](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console)有关的详细信息这些问题和解决方法。</span><span class="sxs-lookup"><span data-stu-id="eac8f-p103">Disable Samsung Smart Manager from managing the Intune Company Portal. Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span> 
    
 <span data-ttu-id="eac8f-p104">**用户许可证类型无效**或**用户名称无法识别错误：** ，用户需要分配一个 Intune 或 EMS 许可证。查看这些文档，以将通过许可证分配： Office 管理中心或 Azure 门户。</span><span class="sxs-lookup"><span data-stu-id="eac8f-p104">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span> 
  
<span data-ttu-id="eac8f-116">更多资源以帮助解决您的问题：</span><span class="sxs-lookup"><span data-stu-id="eac8f-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="eac8f-p105">使用[Intune 疑难解答门户](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)诊断和解决常见注册失败。查看[此文档](https://docs.microsoft.com/intune/help-desk-operators)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="eac8f-p105">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="eac8f-119">查看[此文档](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune)的每个阻止注册和解析的常见错误列表。</span><span class="sxs-lookup"><span data-stu-id="eac8f-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span> 
    
3. <span data-ttu-id="eac8f-120">[了解如何注册 Microsoft Intune 中的 Android 设备](https://docs.microsoft.com/intune/android-enroll)。</span><span class="sxs-lookup"><span data-stu-id="eac8f-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
    

