---
title: 使用 Microsoft Intune 安全基线配置 Windows 10 设备
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50641615"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>使用 Microsoft Intune 安全基线配置 Windows 10 设备

Intune 安全基准可帮助保护用户和设备。 安全基准是 Windows 设置的预配置组，用于应用相关安全团队推荐的已知设置和默认值组。 在 Intune 中创建安全基线配置文件，可创建包含多个设备配置文件的模板。

向用户组或设备部署安全基准时，设置将应用于在 Windows 10 或更高版本中运行的设备。 例如，Microsoft 移动设备管理 （MDM） 安全基准会自动 （1） 为可移动驱动器启用 BitLocker，（2） 需要解除锁定设备的密码，并且 （3） 禁用基本身份验证。 当默认值对环境不起作用时，您可以自定义比较基准，以应用所需的设置。

安全基准还有助于在 Microsoft 365 中建立端到端的安全工作流。 以下是此功能的一些好处：
- 安全基准包括影响安全性的设置最佳做法和建议。 由于 Intune 合作伙伴与 Windows 安全团队一起为组策略创建基准，因此这些建议以可靠的指导和广泛的体验为基础。
- 如果第一次使用 Intune 且不确定从何处着手，则安全基准将帮助你快速创建和部署安全配置文件。
- 如果当前正在使用组策略，则通过使用安全基准迁移到 Intune 会更加轻松，因为这些安全基准内置在 Intune 中，并包含用于管理的领先功能。

有关详细信息，请参阅 [Windows 安全基准](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines)[移动设备管理](https://docs.microsoft.com/windows/client-management/mdm/)。