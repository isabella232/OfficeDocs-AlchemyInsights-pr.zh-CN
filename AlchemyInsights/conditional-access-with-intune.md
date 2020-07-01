---
title: 使用 Intune 进行条件访问
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931420"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="03dea-102">使用 Intune 进行条件访问</span><span class="sxs-lookup"><span data-stu-id="03dea-102">Conditional Access with Intune</span></span>

<span data-ttu-id="03dea-103">使用 Intune**条件访问**需要3个步骤：</span><span class="sxs-lookup"><span data-stu-id="03dea-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="03dea-104">创建**符合性策略**（[Android](https://docs.microsoft.com/intune/compliance-policy-create-android)、 [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios)、 [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)），以定义在将设备视为合规之前必须满足的设置。</span><span class="sxs-lookup"><span data-stu-id="03dea-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="03dea-105">例如，设备的 pin 必须至少为6位数，然后才认为合规。</span><span class="sxs-lookup"><span data-stu-id="03dea-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="03dea-106">创建一个**条件访问策略**，用于定义要保护的资源，以及访问这些资源时需要满足的条件。</span><span class="sxs-lookup"><span data-stu-id="03dea-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="03dea-107">[例如，](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)在访问公司电子邮件之前，设备必须兼容。</span><span class="sxs-lookup"><span data-stu-id="03dea-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="03dea-108">确保**合规性策略**和**条件访问策略**都针对所需的用户组。</span><span class="sxs-lookup"><span data-stu-id="03dea-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="03dea-109">这可能需要在 Azure Active Directory 中创建特定的用户组。</span><span class="sxs-lookup"><span data-stu-id="03dea-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="03dea-110">**帮助链接：**</span><span class="sxs-lookup"><span data-stu-id="03dea-110">**Helpful links:**</span></span>

[<span data-ttu-id="03dea-111">设备合规性概述</span><span class="sxs-lookup"><span data-stu-id="03dea-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="03dea-112">对 CA 进行故障排除</span><span class="sxs-lookup"><span data-stu-id="03dea-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="03dea-113">故障排除策略</span><span class="sxs-lookup"><span data-stu-id="03dea-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="03dea-114">若要保护电子邮件（Exchange online）不受不符合的设备的访问，必须遵循这两个文档：</span><span class="sxs-lookup"><span data-stu-id="03dea-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="03dea-115">使用 EAS 保护来自设备的电子邮件访问</span><span class="sxs-lookup"><span data-stu-id="03dea-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="03dea-116">使用新式验证客户端（如 Outlook）保护来自设备的电子邮件访问</span><span class="sxs-lookup"><span data-stu-id="03dea-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)