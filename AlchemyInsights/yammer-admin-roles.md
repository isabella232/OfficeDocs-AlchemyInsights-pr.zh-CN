---
title: 关于Yammer管理员
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
ms.openlocfilehash: a5d71f509b7006264b15549c7e8450d4ed7025b7dea3cfd80fe6f0fdf50b0b9c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989689"
---
# <a name="about-yammer-admins"></a>关于Yammer管理员

**网络管理员**

全局管理员将自动提升为安全网络中已验证Yammer角色。 在下列情况下，此升级可能不会正确发生：

- 存在Yammer个网络，管理员登录到错误网络。 [需要网络](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)合并才能到达一个Yammer网络。
- Azure PIM 正在使用中。 用户可能不会被提升为全局管理员，因此无法进行推广。 以后更新Yammer可能会解决此问题，但最好是手动将用户提升为全局管理员。
- 网络中存在同步Yammer问题。 在这种情况下，需要进一步调查需要支持请求。

有关管理员角色Yammer，请参阅管理Yammer[管理员。](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins)

**组管理员**

已连接组的Microsoft 365管理员通过 Azure AD 中的组成员身份进行同步。 对于大型组，此同步可能需要一段延长的时间。
