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
ms.openlocfilehash: 23afea21668191093d612d68ca6e9ab2a844f4a14977631d33f4fd956fc3c4e7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005764"
---
# <a name="using-conditional-access-with-intune"></a>将条件访问与 Intune 一同使用

将条件访问与 Intune 一同使用需要 3 个步骤：

- [创建合规性策略以定义在设备被视为合规之前必须符合的设置。例如，设备必须具有至少 6 位数的引脚，然后才能被视为合规。](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [创建条件访问策略，该策略定义要保护的资源以及访问这些资源需要满足的条件。例如，设备在访问公司电子邮件之前必须合规。](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [确保合规性策略和条件访问策略都面向所需的用户组。这可能需要在用户组中创建特定Azure Active Directory。](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[阅读详细信息...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
