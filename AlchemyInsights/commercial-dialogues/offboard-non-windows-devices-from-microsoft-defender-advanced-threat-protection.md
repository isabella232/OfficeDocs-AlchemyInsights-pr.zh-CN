---
title: '从 Microsoft Defender 高级威胁Windows ATP 设备 (非) '
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
ms.openlocfilehash: fbaab348e06691b73db68492a0083c4a5a54c4504e03d27ec53f2a9f5047266d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53967791"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>从 Microsoft Defender 高级威胁Windows ATP 设备 (非) 

操作步骤如下：

1. 按照第三方文档将第三方解决方案与 Microsoft Defender ATP 断开连接。
2. 从Azure Active Directory租户删除第三方解决方案的权限：

    1. 登录 [Azure 门户](https://go.microsoft.com/fwlink/?linkid=2125612)。
    1. 选择 **"所有服务**  >  **Azure Active Directory Enterprise**  >  **应用程序"。**
    1. 选择要离开的应用程序。
    1. 选择“**删除**”。

若要了解更多信息，请参阅非Windows[设备](https://go.microsoft.com/fwlink/?linkid=2143630)。
