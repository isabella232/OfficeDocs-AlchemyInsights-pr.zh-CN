---
title: 使用Microsoft Intune安全基线配置Windows 10设备
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783166"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>使用Microsoft Intune安全基线配置Windows 10设备

Intune 安全基准可帮助保护用户和设备。 安全基线Windows设置预配置的组，用于应用相关安全团队建议的已知设置组和默认值。 在 Intune 中创建安全基线配置文件，可创建包含多个设备配置文件的模板。

将安全基线部署到用户组或设备组时，这些设置将应用于在 Windows 10 或更高版本运行的设备。 例如，Microsoft 移动设备管理 (MDM) 安全基线自动为可移动驱动器启用 BitLocker、需要用于解锁设备的密码以及禁用基本身份验证。 当默认值对环境不起作用时，您可以自定义比较基准，以应用所需的设置。

安全基准还有助于在 Microsoft 365 中建立端到端的安全工作流。 安全基准包括影响安全性的设置最佳做法和建议。 Intune 合作伙伴与Windows团队合作，为组策略创建基线，因此这些建议基于可靠指导和广泛的经验。

如果你是 Intune 的新增用户，并且不确定从何处开始，安全基线可帮助你快速创建和部署安全配置文件。 如果当前使用组策略，则迁移到 Intune 以用于管理目的会更加轻松使用安全基线，因为它们内置于 Intune 中，并且包括最边缘的管理功能。

若要了解更多信息，请参阅Windows[基线和](/windows/security/threat-protection/windows-security-baselines)[移动设备管理](/windows/client-management/mdm/)。

