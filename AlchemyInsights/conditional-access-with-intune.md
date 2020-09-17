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
# <a name="conditional-access-with-intune"></a>使用 Intune 进行条件访问

使用 Intune  **条件访问**  需要3个步骤：

- 创建  **符合性策略**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android)、  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios)、  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) ，用于定义在将设备视为合规之前必须满足的设置。 例如，设备的 pin 必须至少为6位数，然后才认为合规。
- 创建一个 **条件访问策略**  ，用于定义要保护的资源，以及访问这些资源时需要满足的条件。  [例如，](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  在访问公司电子邮件之前，设备必须兼容。
- 确保 **合规性策略**  和  **条件访问策略**  都针对所需的用户组。 这可能需要在 Azure Active Directory 中创建特定的用户组。

**帮助链接：**

[设备合规性概述](https://docs.microsoft.com/intune/device-compliance-get-started)

[对 CA 进行故障排除](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[故障排除策略](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

若要保护电子邮件 (Exchange online) 不受支持的设备的访问，必须遵循这两个文档：

1. [使用 EAS 保护来自设备的电子邮件访问](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [使用新式验证客户端（如 Outlook）保护来自设备的电子邮件访问](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)