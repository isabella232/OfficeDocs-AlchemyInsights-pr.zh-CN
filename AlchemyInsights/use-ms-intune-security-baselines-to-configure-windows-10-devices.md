---
title: 使用 Microsoft Intune 安全基准配置 Windows 10 设备
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
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571779"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>使用 Microsoft Intune 安全基准配置 Windows 10 设备

Intune 安全基准可帮助保护用户和设备。 安全基准是 Windows 设置预配置的组，用于应用已知的设置组和相关安全团队建议的默认值。 通过在 Intune 中创建安全基准配置文件，可以创建一个包含多个设备配置配置文件的模板。

当您将安全基准部署到用户组或设备组时，这些设置将应用于在 Windows 10 或更高版本上运行的设备。 例如，MDM 安全基准自动 (1) 为可移动驱动器启用 BitLocker， (2) 需要用于解锁设备的密码， (3) 禁用基本身份验证。 如果默认值不适用于您的环境，请自定义比较基准以应用所需的设置。

安全基准还有助于在 Microsoft 365 中建立端到端的安全工作流。 以下是一些优点：

- 安全基准包括影响安全性的设置的最佳实践和建议。 由于具有 Windows 安全团队的 Intune 合作伙伴创建组策略的基准，因此这些建议以坚实的指导和广泛的体验为依据。
- 如果你刚开始使用 Intune 并不确定从何处开始，安全基准将帮助你快速创建和部署安全配置文件。
- 如果你当前使用的是组策略，则将安全基准迁移到 Intune 以进行管理将更加简单，因为它们内置于 Intune 中，并包括用于管理的先进功能。

若要了解详细信息，请参阅 [Windows 安全基准](https://go.microsoft.com/fwlink/?linkid=2141503) 和 [移动设备管理](https://go.microsoft.com/fwlink/?linkid=2141701)。