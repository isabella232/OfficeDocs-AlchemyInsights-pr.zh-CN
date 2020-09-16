---
title: SharePoint Online 术语库中缺少术语
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
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750441"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>使用 Intune 启用 Bitlocker 加密

Intune Endpoint Protection 策略可用于为 Windows 设备配置 Boitlocker 加密设置，如中所述： Windows10 (and 更高版本使用 Intune 保护设备) 设置

应注意，许多运行 Windows 10 的更新的设备支持自动 bitlocker 加密，而无需应用 MDM 策略触发。 如果配置了非默认设置，这可能会影响策略的应用。 请参阅 FAQ 以了解更多详细信息。


FAQ   Q：哪些版本的 Windows 支持使用 Endpoint Protection 策略进行设备加密？
 A： Intune Endpoint Protection 策略中的设置是使用 Bitlocker CSP 实现的。并非所有版本的 Windows 都支持 Bitlocker CSP。 
      在这段时间，Windows 版本为：企业版;支持从内部版本1809开始) 教育、移动、移动企业和专业 (。




问：如果已使用 OS 默认的加密方法和密码强度的 XTS 默认设置为设备加密了一个设备，则 (-128) 将应用具有不同设置的策略自动触发对该驱动器的重新加密使用新设置？

答：不可以。 若要应用新密码设置，必须先解密驱动器。

注意：对于使用 Autopilot 注册的设备，在对 Intune 策略进行评估时，将不会触发在 OOBE 期间进行的自动加密，这将允许使用基于策略的设置替代 OS 默认值




问：如果某个设备因 Intune 策略的应用程序而被加密，则在删除该策略时将对其进行解密？

A：删除与加密相关的策略不会导致对配置的驱动器进行解密。




问：为什么 intune 合规性策略显示我的设备不具有 "Bitlocker 已启用"，但它是什么？

A： intune 合规性策略中的 "Bitlocker enabled" 设置利用 Windows 设备运行状况证明 (DHA) 客户端。 此客户端仅在引导时测量设备状态。 因此，如果 bitlocker 加密完成后设备尚未重新启动，则 DHA 客户端服务不会将 bitlocker 报告为活动状态。