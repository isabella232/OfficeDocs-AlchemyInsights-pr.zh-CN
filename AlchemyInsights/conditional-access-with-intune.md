---
title: 使用 Intune 的条件访问
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069702"
---
# <a name="conditional-access-with-intune"></a>使用 Intune 的条件访问

将  **条件访问与**  Intune 一同使用需要 3 个步骤：

- Create a **Compliance Policy** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android)， [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios)， [Windows)](https://docs.microsoft.com//intune/compliance-policy-create-windows) to define settings that must be met before the device is considered compliand. 例如，设备必须具有至少 6 位数的引脚，然后才能被视为合规。
- 创建 **条件访问**  策略，该策略定义要保护的资源以及访问这些资源需要满足的条件。  [例如，](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  设备在访问公司电子邮件之前必须合规。
- 确保 **合规性策略**  和  **条件访问策略**  都面向所需的用户组。 这可能需要在用户组中创建特定Azure Active Directory。

**有用链接：**

[设备合规性概述](https://docs.microsoft.com/intune/device-compliance-get-started)

[CA 疑难解答](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[疑难解答策略](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

若要防止 (Exchange) 访问电子邮件，必须同时关注这两个文档：

1. [使用 EAS 保护来自设备的电子邮件访问](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [使用新式身份验证客户端（如 Outlook） 保护来自设备的电子邮件Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)