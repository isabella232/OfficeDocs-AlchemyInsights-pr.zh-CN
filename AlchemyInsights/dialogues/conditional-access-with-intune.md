---
title: 将条件访问与 Intune 一同使用
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529206"
---
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="ea1c0-102">将条件访问与 Intune 一同使用</span><span class="sxs-lookup"><span data-stu-id="ea1c0-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="ea1c0-103">将条件访问与 Intune 一起使用需要 3 个步骤：</span><span class="sxs-lookup"><span data-stu-id="ea1c0-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="ea1c0-104">创建合规性策略以定义在将设备视为合规之前必须满足的设置。例如，设备必须具有至少 6 位数字的引脚，然后才能被视为合规。</span><span class="sxs-lookup"><span data-stu-id="ea1c0-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="ea1c0-105">创建条件访问策略，该策略定义要保护的资源以及访问这些资源需要满足的条件。例如，设备在访问公司电子邮件之前必须符合标准。</span><span class="sxs-lookup"><span data-stu-id="ea1c0-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="ea1c0-106">确保合规性策略和条件访问策略都面向所需的用户组。这可能需要在 Azure Active Directory 中创建特定用户组。</span><span class="sxs-lookup"><span data-stu-id="ea1c0-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="ea1c0-107">阅读详细信息...</span><span class="sxs-lookup"><span data-stu-id="ea1c0-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
