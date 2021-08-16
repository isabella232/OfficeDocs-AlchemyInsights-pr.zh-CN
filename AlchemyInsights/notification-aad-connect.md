---
title: 通知 AAD 连接
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "9326"
ms.openlocfilehash: b8713700ee4fc8863a269c99b92954e1df45e1e647c491fb9b439ab83c49f2ff
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54097296"
---
# <a name="notification-aad-connect"></a>通知 AAD 连接

- 确保你有权执行此操作。 默认情况下，全局管理员具有访问权限。 此外，您可以使用基于 [角色的访问控制](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) 将注册权限委派给参与者。
- 确保所需的终结点已启用，并且不会因防火墙而受阻。 有关详细信息，请参阅 [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)。
- 由于出站通信受到网络层 SSL 检查，注册可能会失败。
- 确保你已验证 Azure AD 连接运行状况的通知设置并查看你的设置。 若要了解如何为 Azure AD 配置通知设置连接运行状况通知，请参阅[本指南](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)。
- 若要了解有关 AAD 连接运行状况同步报告以及如何下载它，请参阅对象[级同步报告](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)。

若要解决 AAD 连接运行状况警报问题，请按照[AAD 连接 运行状况](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness)数据新鲜度警报疑难解答指南操作，有关常见问题，请参阅 Common [AAD 连接 Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)。
