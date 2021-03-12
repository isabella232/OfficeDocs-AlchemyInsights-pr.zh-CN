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
# <a name="conditional-access-with-intune"></a>Intune 条件访问

将  **条件访问与**  Intune 一起使用需要 3 个步骤：

- 在 **Android** [ (、iOS](https://docs.microsoft.com/intune/compliance-policy-create-android) [](https://docs.microsoft.com/intune/compliance-policy-create-ios) [、Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) 创建合规性策略，以定义在设备被视为合规之前必须满足的设置。 例如，设备必须具有至少 6 位数字的引脚，然后才能被视为合规。
- 创建 **条件访问**  策略，该策略定义要保护的资源以及访问这些资源需要满足的条件。  [例如，](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  设备在访问公司电子邮件之前必须符合标准。
- 确保 **合规性策略**  和  **条件访问策略**  都面向所需的用户组。 这可能需要在 Azure Active Directory 中创建特定用户组。

**有用链接：**

[设备合规性概述](https://docs.microsoft.com/intune/device-compliance-get-started)

[CA 疑难解答](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[疑难解答策略](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

若要保护 Exchange (电子邮件) 设备无法访问，必须关注这两个文档：

1. [使用 EAS 保护来自设备的电子邮件访问](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [使用新式身份验证客户端（如 Outlook）保护来自设备的电子邮件访问](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)