---
title: 域服务的密码哈希同步
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 3c00105a67f70ae9ce11cd8bb922c4d84a320010d021414b9159948f7dc87dbc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040856"
---
# <a name="password-hash-synchronization-for-domain-service"></a>域服务的密码哈希同步

**如果 Azure AD DS 实例提示启用密码哈希同步**

所遇到的场景是，你正在运行一个混合环境，用户从预置的 Azure Active Directory 域服务 (AD DS) 环境中进行同步。 尽管已将密码散列同步从预置 AD DS 到 Azure AD 租户，但仍会遇到这种情况。

**原因**

出现这种情况的原因是，Azure AD Connect 默认情况下没有同步 Azure AD DS 所需的传统新技术 LAN Manager (NTLM) 和 Kerberos 密码哈希。

**解决方法** 

需要配置 Azure AD Connect 来同步 NTLM 和 Kerberos 身份验证所需的这些密码哈希。

配置 Azure AD Connect 后，预置账户创建或密码更改事件也会随即将传统密码哈希同步到 Azure AD。 有关这方面的更多信息以及有关如何在 Azure AD DS 混合环境中启用密码同步的指导，请参见[此处](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync)。