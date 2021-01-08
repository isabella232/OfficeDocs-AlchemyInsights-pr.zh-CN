---
title: DataProtection - Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 482c08b31e4d97ca5cc9ec6e35e309cb7536036d
ms.sourcegitcommit: 58ac31a58c956a4d74f66bd4151a2311dc361b78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2021
ms.locfileid: "49778183"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>使用 Intune 启用 Bitlocker 加密

Intune Endpoint Protection 策略可用于为 Windows 设备配置 Bitlocker 加密设置。 有关详细信息，请参阅 Windows 10 (及更高版本) [Intune 保护设备。](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)

除了终结点保护策略之外，还有一个加密报告，它提供设备的加密状态的更详细视图。 此报告可以从 MEM 门户在"设备监控 **>"** 下访问，然后在"配置选择加密"[报告下访问](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport)。

如果发现 Bitlocker 无法按预期启用，或者用于启用 Bitlocker 的配置文件的状态错误，请查看加密报告，以便更好地了解发生此行为的原因。

若要查找有关如何解释报告的详细信息，包括各种加密状态值，请参阅使用 [Intune 监视设备加密](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)。

你应该知道，许多运行 Windows 10 的较新设备都支持自动 Bitlocker 加密，无需应用 MDM 策略即可触发。 如果配置了非默认设置，这可能会影响策略的应用。 有关详细信息，请参阅以下常见问题解答。

有关 bitlocker 问题疑难解答的信息，请参阅 Microsoft Intune 中的 [BitLocker](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)策略疑难解答。
 
 
**常见问题解答**

问：哪些版本的 Windows 支持使用 Endpoint Protection 策略进行设备加密？<br>
答：Intune Endpoint Protection 策略中的设置是使用 [Bitlocker CSP 实现的](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)。 并非所有版本的 Windows 都支持 Bitlocker CSP。 <br><br>

问：如何在无需最终用户交互的情况下在设备上启用 Bitlocker？<br>
答：只要满足必要的先决条件，就可以通过 Intune 启用 Bitlocker"无提示加密"。 请参阅以下文档中的设备要求和示例策略设置的详细信息，以启用无提示加密：无提示 [启用 Bitlocker 加密](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices)。 <br><br>

问：如果设备已使用适用于加密方法和加密强度 (XTS-AES-128) 的操作系统默认设置使用 Bitlocker 进行加密，那么应用不同设置的策略是否将自动触发使用新设置的驱动器重新加密？<br>
答：不可以。 若要应用新的密码设置，必须先解密驱动器。<br><br>
**注意：** 对于使用 Autopilot 注册的设备，在评估 Intune 策略之前，不会触发在 OOBE 期间发生的自动加密，这将允许使用基于策略的设置来更改操作系统默认值。
 
问：如果设备由于 Intune 策略的应用而加密，那么在删除该策略时，设备是否将被解密？<br>
答：删除与加密相关的策略不会解密已配置的驱动器。
 
问：为什么 Intune 合规性策略显示我的设备未启用 Bitlocker，即使它已启用？<br>
答：Intune 合规性策略中的"启用 Bitlocker"设置利用 Windows 设备运行状况证明 (DHA) 客户端。 此客户端仅在启动时测量设备状态。 因此，如果自 Bitlocker 加密完成后设备尚未重新启动，DHA 客户端服务将不会报告 Bitlocker 处于活动状态。
 
 