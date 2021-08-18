---
title: 配置 LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090402"
---
# <a name="configure-ldap"></a>配置 LDAP

若要配置 LDAP，请执行下列操作：

1. 在 Azure 门户上检查域 [的运行状况](https://aka.ms/aadds-health)。
1. 确保有效的 Azure AD 订阅可用，并且已启用 Azure AD 域服务。
1. 启用安全 LDAP 所需的证书必须从受信任的公共证书颁发机构获得，或者是自签名证书。
1. 确保证书遵循所需的 [准则](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)。

**证书无效**
1. 若要续订证书，请按照步骤创建新证书并重新加载： [配置 LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)。
1. 若要解决 Azure Active directory 域服务中安全 LDAP 警报的已知问题，请参阅解决 [LDAP 警报](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)。
