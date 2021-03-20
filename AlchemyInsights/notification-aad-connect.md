---
title: 通知 AAD Connect
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
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897540"
---
# <a name="notification-aad-connect"></a>通知 AAD Connect

- 确保你有权执行此操作。 默认情况下，全局管理员具有访问权限。 此外，您可以使用基于 [角色的访问控制](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) 将注册权限委派给参与者。
- 确保所需的终结点已启用，并且不会因防火墙而受阻。 有关详细信息，请参阅 [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)。
- 由于出站通信受到网络层 SSL 检查，注册可能会失败。
- 确保你已验证 Azure AD Connect Health 的通知设置并查看你的设置。 若要了解如何配置 Azure AD Connect Health 通知的通知设置，请参阅 [本指南](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)。
- 若要了解有关 AAD Connect Health 同步报告以及如何下载它，请参阅对象 [级同步报告](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)。

若要解决 AAD Connect 运行状况警报问题，请按照 [AAD Connect Health 数据](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) 新鲜度警报疑难解答指南操作，有关常见问题，请参阅 [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)。
