---
title: Intune 条件访问
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704776"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="7e2b0-102">Intune 条件访问</span><span class="sxs-lookup"><span data-stu-id="7e2b0-102">Conditional Access with Intune</span></span>

<span data-ttu-id="7e2b0-103">将  **条件访问与**  Intune 一起使用需要 3 个步骤：</span><span class="sxs-lookup"><span data-stu-id="7e2b0-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="7e2b0-104">在 **Android** [ (、iOS](https://docs.microsoft.com/intune/compliance-policy-create-android) [](https://docs.microsoft.com/intune/compliance-policy-create-ios) [、Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) 创建合规性策略，以定义在设备被视为合规之前必须满足的设置。</span><span class="sxs-lookup"><span data-stu-id="7e2b0-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="7e2b0-105">例如，设备必须具有至少 6 位数字的引脚，然后才能被视为合规。</span><span class="sxs-lookup"><span data-stu-id="7e2b0-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="7e2b0-106">创建 **条件访问**  策略，该策略定义要保护的资源以及访问这些资源需要满足的条件。</span><span class="sxs-lookup"><span data-stu-id="7e2b0-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="7e2b0-107">[例如，](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  设备在访问公司电子邮件之前必须符合标准。</span><span class="sxs-lookup"><span data-stu-id="7e2b0-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="7e2b0-108">确保 **合规性策略**  和  **条件访问策略**  都面向所需的用户组。</span><span class="sxs-lookup"><span data-stu-id="7e2b0-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="7e2b0-109">这可能需要在 Azure Active Directory 中创建特定用户组。</span><span class="sxs-lookup"><span data-stu-id="7e2b0-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="7e2b0-110">**有用链接：**</span><span class="sxs-lookup"><span data-stu-id="7e2b0-110">**Helpful links:**</span></span>

[<span data-ttu-id="7e2b0-111">设备合规性概述</span><span class="sxs-lookup"><span data-stu-id="7e2b0-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="7e2b0-112">CA 疑难解答</span><span class="sxs-lookup"><span data-stu-id="7e2b0-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="7e2b0-113">疑难解答策略</span><span class="sxs-lookup"><span data-stu-id="7e2b0-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="7e2b0-114">若要保护 Exchange (电子邮件) 设备无法访问，必须关注这两个文档：</span><span class="sxs-lookup"><span data-stu-id="7e2b0-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="7e2b0-115">使用 EAS 保护来自设备的电子邮件访问</span><span class="sxs-lookup"><span data-stu-id="7e2b0-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="7e2b0-116">使用新式身份验证客户端（如 Outlook）保护来自设备的电子邮件访问</span><span class="sxs-lookup"><span data-stu-id="7e2b0-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)