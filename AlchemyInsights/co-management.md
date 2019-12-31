---
title: 协同管理
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1556"
- "9000080"
ms.openlocfilehash: fe7dcebf847fbd7d91632e93e2253bf62ac659aa
ms.sourcegitcommit: 4ed431b2e1aed26d07bd7eba282531537d29ad0e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/30/2019
ms.locfileid: "40910196"
---
# <a name="co-management"></a>协同管理

**从 Config Manager 混合到 Intune 进行迁移的先决条件**

- 查看[本文](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-hybridmdm-to-intunesa)。
- 向[您的用户添加 Intune 许可证](https://docs.microsoft.com/intune/licenses-assign)。
- 配置共同管理时使用[边缘浏览器](https://www.microsoft.com/windows/microsoft-edge)。

**如何在 Intune 管理的设备上安装配置管理器客户端**

请参阅[INTUNE MDM 托管 Windows 设备](https://docs.microsoft.com/sccm/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm)。

**如果我只想更改 MDM 颁发机构，该怎么办？**

在不打开支持案例的情况下，可以更改 MDM 证书颁发机构。 请查看以下文档以帮助更改你的 MDM 证书颁发机构：
- [将 MDM 颁发机构从 Config Manager 更改为 Intune 独立](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-change-mdm-authority)
- [将 MDM 颁发机构从 Intune 独立更改为配置管理器](https://docs.microsoft.com/intune-classic/deploy-use/prerequisites-for-enrollment#what-to-do-if-you-choose-the-wrong-mdm-authority-setting)