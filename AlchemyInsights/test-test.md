---
title: SharePoint在线术语库缺少的术语
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: d99458d6f9b65e44ad5945c909b9a8861cf0b1f23463fcdfd5b8351b1c08d670
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54106401"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>使用 Intune 启用 Bitlocker 加密

Intune Endpoint Protection 策略可用于为 Windows 设备配置 Boitlocker 加密设置，如：Windows 10 (及更高版本) 设置中所述，使用 Intune 保护设备

你应该注意，许多运行 Windows 10设备支持自动 bitlocker 加密，无需应用 MDM 策略即可触发。 如果配置了非默认设置，这可能会影响策略的应用。 有关详细信息，请参阅常见问题解答。


FAQ Q： Which editions of Windows support device encryption using the Endpoint Protection Policy？
答：Intune Endpoint Protection策略中的设置是使用 Bitlocker CSP 实现的。  并非所有版本或内部版本Windows Bitlocker CSP。 目前，Windows版本：Enterprise;支持教育版、移动版Enterprise移动版Professional (版本 1809 及) 版本。




问：如果设备已使用加密方法的操作系统默认设置和密码强度 (XTS-AES-128) 使用 Bitlocker 加密) 是否应用不同设置的策略将自动触发使用新设置的驱动器重新加密？

答：否。 要应用新的密码设置，必须先解密驱动器。

注意 对于使用 Autopilot 注册的设备，在评估 Intune 策略（允许使用基于策略的设置来更改操作系统默认值）之前，不会触发在 OOBE 期间发生的自动加密




Q If a device is encrypted as a result of the application of Intune policy will be decrypted when that policy is removed？

答：删除与加密相关的策略不会解密已配置的驱动器。




问：为什么 intune 合规性策略显示我的设备未"启用 Bitlocker"，但它已启用？

答：intune 合规性策略中的"启用 Bitlocker"设置利用 Windows 设备运行状况证明 (DHA) 客户端。 此客户端仅在启动时测量设备状态。 因此，如果设备在 bitlocker 加密完成之后尚未重新启动，DHA 客户端服务将不会报告 bitlocker 处于活动状态。