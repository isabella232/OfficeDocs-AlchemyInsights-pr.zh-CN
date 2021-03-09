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
# <a name="using-conditional-access-with-intune"></a>将条件访问与 Intune 一同使用

将条件访问与 Intune 一起使用需要 3 个步骤：

- [创建合规性策略以定义在将设备视为合规之前必须满足的设置。例如，设备必须具有至少 6 位数字的引脚，然后才能被视为合规。](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [创建条件访问策略，该策略定义要保护的资源以及访问这些资源需要满足的条件。例如，设备在访问公司电子邮件之前必须符合标准。](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [确保合规性策略和条件访问策略都面向所需的用户组。这可能需要在 Azure Active Directory 中创建特定用户组。](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[阅读详细信息...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
