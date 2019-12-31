---
title: DataProtection-Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908700"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>使用 Intune 启用 Bitlocker 加密

 Intune Endpoint Protection 策略可用于配置 Windows 设备的 Bitlocker 加密设置。 有关详细信息，请参阅[使用 Intune 保护设备的 Windows 10 （及更高版本）设置](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)。
 
应注意，许多运行 Windows 10 的更新的设备都支持自动 Bitlocker 加密，这是在不应用 MDM 策略的情况下触发的。 如果配置了非默认设置，这可能会影响策略的应用。 有关更多详细信息，请参阅以下 FAQ。
 
有关对 bitlocker 问题进行故障排除的信息，请参阅[Microsoft Intune 中的 bitlocker 策略疑难解答](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)。
 
 
**常见问题解答**

 问：哪些版本的 Windows 支持使用 Endpoint Protection 策略进行设备加密？<br>
 A： Intune Endpoint Protection 策略中的设置是使用[BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)实现的。 并不是所有版本或 Windows 版本都支持 Bitlocker CSP。 <br><br>
      目前，支持以下 Windows 版本：企业版、教育版、移动版、移动企业版和专业版（内部版本1809及更高版本）。
 
问：如果使用 OS 默认设置加密方法和密码强度（XTS-128），设备已使用 Bitlocker 进行了加密，则应用具有不同设置的策略将自动触发对具有新设置的驱动器的重新加密。<br>
答：不可以。 若要应用新密码设置，必须先解密驱动器。<br><br>
**注意：** 对于使用 Autopilot 注册的设备，在对 Intune 策略进行评估之前不会触发在 OOBE 期间进行的自动加密，这将允许使用基于策略的设置来替代 OS 默认值。
 
问：如果某个设备因 Intune 策略的应用程序而被加密，则在删除该策略时是否会对其进行解密？<br>
A：删除与加密相关的策略不会导致对配置的驱动器进行解密。
 
问：为什么 Intune 合规性策略显示我的设备未启用 Bitlocker，尽管它是吗？<br>
A： Intune 合规性策略中的 "Bitlocker 已启用" 设置利用 Windows 设备运行状况证明（DHA）客户端。 此客户端仅在引导时测量设备状态。 因此，如果 Bitlocker 加密完成后设备尚未重新启动，则 DHA 客户端服务不会将 Bitlocker 报告为活动状态。
 
 