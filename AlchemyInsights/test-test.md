---
title: SharePoint Online 术语库中缺少术语
ms.author: pebaum
author: Techwriter40
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 0f9efe980987c9ffc64fcf9d5d72a67f0a622867
ms.sourcegitcommit: 23772ebd25a86a879ced40b10566a35e76a79eb5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/05/2019
ms.locfileid: "36762041"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>使用 Intune 启用 Bitlocker 加密

Intune Endpoint Protection 策略可用于为 Windows 设备配置 Boitlocker 加密设置，如中所述： Windows10 （及更高版本）设置以使用 Intune 保护设备

应注意，许多运行 Windows 10 的更新的设备支持自动 bitlocker 加密，而无需应用 MDM 策略触发。 如果配置了非默认设置，这可能会影响策略的应用。 请参阅 FAQ 以了解更多详细信息。


FAQ  Q：哪些版本的 Windows 支持使用 Endpoint Protection 策略进行设备加密？
 A： Intune Endpoint Protection 策略中的设置是使用 Bitlocker CSP 实现的。并非所有版本的 Windows 都支持 Bitlocker CSP。 
      在这段时间，Windows 版本为：企业版;支持教育、移动、移动企业和专业（自内部版本1809）。




问：如果使用 OS 默认设置加密方法和密码强度对设备进行了 Bitlocker 加密（XTS-128），则应用具有不同设置的策略将自动触发对具有新设置的驱动器的重新加密。

答：不可以。 若要应用新密码设置，必须先解密驱动器。

注意：对于使用 Autopilot 注册的设备，在对 Intune 策略进行评估时，将不会触发在 OOBE 期间进行的自动加密，这将允许使用基于策略的设置替代 OS 默认值




问：如果某个设备因 Intune 策略的应用程序而被加密，则在删除该策略时将对其进行解密？

A：删除与加密相关的策略不会导致对配置的驱动器进行解密。




问：为什么 intune 合规性策略显示我的设备不具有 "Bitlocker 已启用"，但它是什么？

A： intune 合规性策略中的 "Bitlocker 已启用" 设置利用 Windows 设备运行状况证明（DHA）客户端。 此客户端仅在引导时测量设备状态。 因此，如果 bitlocker 加密完成后设备尚未重新启动，则 DHA 客户端服务不会将 bitlocker 报告为活动状态。