---
title: DataProtection - Bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 3f6e48b9d2f7562d74d60c2901759a7ab359e5c67bd4aa2d556d941a41ab680c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118564"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>使用 Intune 启用 Bitlocker 加密

Intune Endpoint Protection 策略可用于为设备配置 Bitlocker 加密Windows设置。 有关详细信息，请参阅Windows 10 ([和更高版本) Intune 保护设备](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)。

除了安全Endpoint Protection，还有一个加密报告，它提供有关设备的加密状态的更详细视图。 可以从"设备""监视"下的 MEM 门户访问此 **>，然后在**"配置"下选择"加密 [报告"。](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport)

如果发现 Bitlocker 无法按预期启用，或者用于启用 Bitlocker 的配置文件的状态为错误，请查看加密报告以更好地了解发生此行为的原因。

若要查找有关如何解释报告的详细信息，包括各种加密状态值，请参阅使用 [Intune 监视设备加密](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)。

你应该注意，许多运行 bitlocker Windows 10支持自动 Bitlocker 加密，无需应用 MDM 策略即可触发。 如果配置了非默认设置，这可能会影响策略的应用。 有关详细信息，请参阅以下常见问题解答。

有关排查 bitlocker 问题的信息，请参阅[BitLocker 策略](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)疑难解答Microsoft Intune。
 
 
**常见问题解答**

问：哪些版本的 Windows支持使用策略进行Endpoint Protection加密？<br>
答：Intune Endpoint Protection 策略中的设置是使用[Bitlocker CSP 实现的](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)。 并非所有版本或内部版本Windows Bitlocker CSP。 <br><br>

问：如何在无需最终用户交互的情况下在设备上启用 Bitlocker？<br>
答：只要满足必要的先决条件，就可以通过 Intune 启用 Bitlocker"无提示加密"。 请参阅以下文档中的设备要求的详细信息和启用无提示加密的策略设置示例 [：Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices)。 <br><br>

问：如果设备已使用用于加密方法和密码强度 (XTS-AES-128) 的操作系统默认设置使用 Bitlocker 进行加密，那么应用不同设置的策略是否会自动触发使用新设置的驱动器重新加密？<br>
答：否。 若要应用新的密码设置，必须先解密驱动器。<br><br>
**注意：** 对于使用 Autopilot 注册的设备，在评估 Intune 策略之前，不会触发 OOBE 期间发生的自动加密，这将允许使用基于策略的设置来更改操作系统默认值。
 
问：如果设备由于应用 Intune 策略而加密，那么在删除该策略时，设备是否将被解密？<br>
答：删除与加密相关的策略不会解密已配置的驱动器。
 
问：为什么 Intune 合规性策略显示我的设备未启用 Bitlocker，即使已启用？<br>
答：Intune 合规性策略中的"启用 Bitlocker"设置利用 DHA Windows客户端 (设备) 证明。 此客户端仅在启动时测量设备状态。 因此，如果设备在 Bitlocker 加密完成之后尚未重新启动，DHA 客户端服务不会将 Bitlocker 报告为活动状态。
 
 