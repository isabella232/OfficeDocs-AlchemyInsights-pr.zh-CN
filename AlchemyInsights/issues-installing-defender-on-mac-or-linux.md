---
title: 有关在 Mac 或 Linux 上安装 Microsoft Defender 的问题
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: ae17caa4be7809b591be9f9c042186f67828aa3c36a3d17332806e4d92545dc6
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898598"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>有关在 Mac 或 Linux 上安装 Microsoft Defender 的问题

**Mac**

- 在安装 Mac 版 Microsoft Defender ATP 前确保满足系统要求。 有关更多信息，请参阅[如何安装 Mac 版 Microsoft Defender ATP](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)。  
- 检查此文件中的信息："/Library/Logs/Microsoft/mdatp/install.log"。

**Linux**

- 在安装 Linux 版 Microsoft Defender ATP 前确保满足系统要求。 有关详细信息，请参阅[如何安装 Linux 版 MDATP](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)。 
- 要验证 MDATP 服务正在允许，请参阅[安装失败](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)。  
    如果服务未运行，要故障排除和解决问题，请参阅[mdatp 服务未运行时故障排除步骤](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)。
- 客户端配置用于验证产品的健康，有关检查客户端配置步骤和运行检测测试 EICAR 文本文件的信息，请参阅[客户端配置](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)。  

    **注意** 要查看受支持的文件系统的访问活动列表，请参与 [Linux 版 Microsoft Defender ATP](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)。