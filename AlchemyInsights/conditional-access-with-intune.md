---
title: 使用 Intune 进行条件访问
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807649"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="f61c0-102">使用 Intune 进行条件访问</span><span class="sxs-lookup"><span data-stu-id="f61c0-102">Conditional Access with Intune</span></span>

<span data-ttu-id="f61c0-103">使用 Intune  **条件访问**  需要3个步骤：</span><span class="sxs-lookup"><span data-stu-id="f61c0-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="f61c0-104">创建  **符合性策略**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android)、  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios)、  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) ，用于定义在将设备视为合规之前必须满足的设置。</span><span class="sxs-lookup"><span data-stu-id="f61c0-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="f61c0-105">例如，设备的 pin 必须至少为6位数，然后才认为合规。</span><span class="sxs-lookup"><span data-stu-id="f61c0-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="f61c0-106">创建一个 **条件访问策略**  ，用于定义要保护的资源，以及访问这些资源时需要满足的条件。</span><span class="sxs-lookup"><span data-stu-id="f61c0-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="f61c0-107">[例如，](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  在访问公司电子邮件之前，设备必须兼容。</span><span class="sxs-lookup"><span data-stu-id="f61c0-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="f61c0-108">确保 **合规性策略**  和  **条件访问策略**  都针对所需的用户组。</span><span class="sxs-lookup"><span data-stu-id="f61c0-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="f61c0-109">这可能需要在 Azure Active Directory 中创建特定的用户组。</span><span class="sxs-lookup"><span data-stu-id="f61c0-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="f61c0-110">**帮助链接：**</span><span class="sxs-lookup"><span data-stu-id="f61c0-110">**Helpful links:**</span></span>

[<span data-ttu-id="f61c0-111">设备合规性概述</span><span class="sxs-lookup"><span data-stu-id="f61c0-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="f61c0-112">对 CA 进行故障排除</span><span class="sxs-lookup"><span data-stu-id="f61c0-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="f61c0-113">故障排除策略</span><span class="sxs-lookup"><span data-stu-id="f61c0-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="f61c0-114">若要保护电子邮件 (Exchange online) 不受支持的设备的访问，必须遵循这两个文档：</span><span class="sxs-lookup"><span data-stu-id="f61c0-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="f61c0-115">使用 EAS 保护来自设备的电子邮件访问</span><span class="sxs-lookup"><span data-stu-id="f61c0-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="f61c0-116">使用新式验证客户端（如 Outlook）保护来自设备的电子邮件访问</span><span class="sxs-lookup"><span data-stu-id="f61c0-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)