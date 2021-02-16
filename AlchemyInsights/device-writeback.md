---
title: 设备写回
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2021
ms.locfileid: "50255147"
---
# <a name="device-writeback"></a>设备写回

设备写回用于以下方案：

- 使用 [混合证书信任部署启用 Windows Hello 企业应用](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- 启用基于设备的条件访问 ADFS (2012 R2 或更高版本) 受信赖方信任 (应用程序) 

    > [!NOTE]
    > 设备写回需要订阅 Azure AD Premium。

这提供额外的安全和保证，即仅向受信任的设备授予对应用程序的访问权限。 有关条件访问详细信息，请参阅 [使用条件](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) 访问管理风险，以及使用 [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview)设备注册设置本地条件访问。

有关为设备启用设备写回功能详细信息，请参阅["启用设备写回"。](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)
