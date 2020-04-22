---
title: 解决在 Microsoft Intune 中注册 Android 设备时出现的问题
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759610"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="e489a-102">解决在 Microsoft Intune 中注册 Android 设备时出现的问题</span><span class="sxs-lookup"><span data-stu-id="e489a-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="e489a-103">立即查看下面列出的资源，以解决问题。</span><span class="sxs-lookup"><span data-stu-id="e489a-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="e489a-104">一些常见的问题和解决步骤：</span><span class="sxs-lookup"><span data-stu-id="e489a-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="e489a-105">**公司门户中的设备未加密错误：** 较新版本的 Android （特别是从7.0 开始）需要启动密码，以确保您的设备已完全加密。</span><span class="sxs-lookup"><span data-stu-id="e489a-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="e489a-106">常见的解决方案是启用启动 pin 或完全加密设备。</span><span class="sxs-lookup"><span data-stu-id="e489a-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="e489a-107">有关详细信息，请查看[此文档](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android)。</span><span class="sxs-lookup"><span data-stu-id="e489a-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="e489a-108">在**intune 管理控制台中，设备无法签入 intune 服务或显示为 "不正常"：** 某些 Samsung 4.4 和5.5 设备可能无法签入服务。</span><span class="sxs-lookup"><span data-stu-id="e489a-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="e489a-109">有3种可能的解决方案可解决此问题：</span><span class="sxs-lookup"><span data-stu-id="e489a-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="e489a-110">手动打开 Intune 公司门户应用程序，这将自动启动设备同步。</span><span class="sxs-lookup"><span data-stu-id="e489a-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="e489a-111">将设备更新到 Android 6.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="e489a-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="e489a-112">禁用 Samsung Smart Manager 管理 Intune 公司门户。</span><span class="sxs-lookup"><span data-stu-id="e489a-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="e489a-113">有关这些问题和解决方法的详细信息，请参阅[本文档](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console)。</span><span class="sxs-lookup"><span data-stu-id="e489a-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="e489a-114">**用户许可证类型无效**或**无法识别用户名称错误：** 需要为用户分配 Intune 或 EMS 许可证。</span><span class="sxs-lookup"><span data-stu-id="e489a-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="e489a-115">查看这些文档以通过以下步骤分配许可证： Office 管理中心或 Azure 门户。</span><span class="sxs-lookup"><span data-stu-id="e489a-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="e489a-116">帮助解决你的问题的其他资源：</span><span class="sxs-lookup"><span data-stu-id="e489a-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="e489a-117">使用[Intune 故障排除门户](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)诊断和解决常见注册故障。</span><span class="sxs-lookup"><span data-stu-id="e489a-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="e489a-118">有关详细信息，请查看[此文档](https://docs.microsoft.com/intune/help-desk-operators)。</span><span class="sxs-lookup"><span data-stu-id="e489a-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="e489a-119">查看[此文档](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune)，了解阻止对每个的注册和解决的常见错误的列表。</span><span class="sxs-lookup"><span data-stu-id="e489a-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="e489a-120">[了解如何在 Microsoft Intune 中注册 Android 设备](https://docs.microsoft.com/intune/android-enroll)。</span><span class="sxs-lookup"><span data-stu-id="e489a-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
