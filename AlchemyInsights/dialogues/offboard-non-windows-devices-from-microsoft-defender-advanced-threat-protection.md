---
title: '从 Microsoft Defender 高级威胁防护和 ATP 设备 (非 Windows) '
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529969"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>从 Microsoft Defender 高级威胁防护和 ATP 设备 (非 Windows) 

操作步骤如下：

1. 按照第三方文档，断开第三方解决方案与 Microsoft Defender ATP 连接。
2. 从 Azure Active Directory 租户中删除第三方解决方案的权限：

    1. 登录到 [Azure 门户](https://go.microsoft.com/fwlink/?linkid=2125612)。
    1. 选择 **所有**  >  **服务 Azure Active Directory**  >  **企业应用程序**。
    1. 选择要离开的应用程序。
    1. 选择“删除”。

若要了解更多信息，请参阅 [Offboard 非 Windows 设备](https://go.microsoft.com/fwlink/?linkid=2143630)。
