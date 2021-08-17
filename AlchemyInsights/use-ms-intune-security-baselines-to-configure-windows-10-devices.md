---
title: 使用Microsoft Intune安全基线配置Windows 10设备
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: a94c6b72df3874ee80413adac86d60306175734b6ff28b2e015e05eec6f3838b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104334"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>使用Microsoft Intune安全基线配置Windows 10设备

Intune 安全基准可帮助保护用户和设备。 安全基准是 Windows 设置的预配置组，用于应用相关安全团队推荐的已知设置和默认值组。 在 Intune 中创建安全基线配置文件，可创建包含多个设备配置文件的模板。

将安全基线部署到用户组或设备组时，这些设置将应用于在 Windows 10 或更高版本运行的设备。 例如，MDM 安全基线自动 (1) 为可移动驱动器启用 BitLocker， (2) 需要密码才能解锁设备， (3) 禁用基本身份验证。 如果默认值不适用于您的环境，请自定义基线以应用所需的设置。

安全基准还有助于在 Microsoft 365 中建立端到端的安全工作流。 以下是此操作的一些好处：

- 安全基准包括影响安全性的设置最佳做法和建议。 由于 Intune 合作伙伴与 Windows 安全团队一起为组策略创建基准，因此这些建议以可靠的指导和广泛的体验为基础。
- 如果第一次使用 Intune 且不确定从何处着手，则安全基准将帮助你快速创建和部署安全配置文件。
- 如果当前使用组策略，那么使用安全基线迁移到 Intune 以用于管理会容易得多，因为它们内置于 Intune 中，并且包括用于管理的领先功能。

若要了解更多信息，请参阅Windows[基线和](https://go.microsoft.com/fwlink/?linkid=2141503)[移动设备管理](https://go.microsoft.com/fwlink/?linkid=2141701)。