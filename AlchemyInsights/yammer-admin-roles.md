---
title: 关于 Yammer 管理员
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
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2021
ms.locfileid: "50995236"
---
# <a name="about-yammer-admins"></a>关于 Yammer 管理员

**网络管理员**

全局管理员将自动提升为 Yammer 网络中已验证的管理员角色。 在下列情况下，此升级可能不会正确发生：

- 存在多个 Yammer 网络，管理员登录的网络错误。 [需要网络](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) 整合才能访问一个 Yammer 网络。
- Azure PIM 正在使用中。 用户可能不会被提升为全局管理员，因此无法进行推广。 Yammer 的未来更新可能会解决此问题，但最好是手动将用户提升为全局管理员。
- Yammer 网络存在同步问题。 在这种情况下，需要进一步调查需要支持请求。

有关 Yammer 管理员角色的信息，请参阅 [管理 Yammer 管理员](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins)。

**组管理员**

Microsoft 365 连接的组的组管理员与 Azure AD 中的组成员身份同步。 对于大型组，此同步可能需要一段延长的时间。
