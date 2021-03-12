---
title: 解决在 Microsoft Intune 中注册 Android 设备的问题
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708988"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="ddade-102">解决在 Microsoft Intune 中注册 Android 设备的问题</span><span class="sxs-lookup"><span data-stu-id="ddade-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="ddade-103">查看下面列出的资源，以现在解决问题。</span><span class="sxs-lookup"><span data-stu-id="ddade-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="ddade-104">一些常见问题和解决步骤：</span><span class="sxs-lookup"><span data-stu-id="ddade-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="ddade-105">**公司门户中的设备未加密错误：** 较新版本的 Android（尤其是从 v7.0 开始）需要启动密码，以确保设备已完全加密。</span><span class="sxs-lookup"><span data-stu-id="ddade-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="ddade-106">常见解决方案是启用启动引脚或完全加密设备。</span><span class="sxs-lookup"><span data-stu-id="ddade-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="ddade-107">有关详细信息 [，](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) 请查看本文档。</span><span class="sxs-lookup"><span data-stu-id="ddade-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="ddade-108">**设备无法签入 Intune** 服务或在 Intune 管理控制台中显示为"不正常"：某些 Samsung 4.4 和 5.5 设备可能无法签入服务。</span><span class="sxs-lookup"><span data-stu-id="ddade-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="ddade-109">此问题有 3 种可能的解决方案：</span><span class="sxs-lookup"><span data-stu-id="ddade-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="ddade-110">手动打开 Intune 公司门户应用，该应用将自动启动设备同步。</span><span class="sxs-lookup"><span data-stu-id="ddade-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="ddade-111">将设备更新到 Android 6.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="ddade-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="ddade-112">禁用 Samsung Smart Manager 管理 Intune 公司门户。</span><span class="sxs-lookup"><span data-stu-id="ddade-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="ddade-113">请查看 [本文档](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) ，进一步详细了解这些问题和解决方法。</span><span class="sxs-lookup"><span data-stu-id="ddade-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="ddade-114">**用户许可证类型无效** 或用户名无法 **识别错误** ：需要为用户分配 Intune 或 EMS 许可证。</span><span class="sxs-lookup"><span data-stu-id="ddade-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="ddade-115">查看以下文档以通过以下方式分配许可证：Office 管理中心或 Azure 门户。</span><span class="sxs-lookup"><span data-stu-id="ddade-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="ddade-116">有助于解决问题的其他资源：</span><span class="sxs-lookup"><span data-stu-id="ddade-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="ddade-117">使用 [Intune 故障排除门户](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) 诊断和解决常见的注册失败。</span><span class="sxs-lookup"><span data-stu-id="ddade-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="ddade-118">有关详细信息 [，](https://docs.microsoft.com/intune/help-desk-operators) 请查看本文档。</span><span class="sxs-lookup"><span data-stu-id="ddade-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="ddade-119">请查看 [本文档，](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) 了解阻止注册和解决每个错误常见错误的列表。</span><span class="sxs-lookup"><span data-stu-id="ddade-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="ddade-120">[了解如何在 Microsoft Intune 中注册 Android 设备](https://docs.microsoft.com/intune/android-enroll)。</span><span class="sxs-lookup"><span data-stu-id="ddade-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
