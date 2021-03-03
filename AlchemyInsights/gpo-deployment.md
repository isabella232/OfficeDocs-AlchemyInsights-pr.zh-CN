---
title: GPO 部署
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416937"
---
# <a name="gpo-deployment"></a>GPO 部署

Azure Active Directory 域服务（Azure AD DS）中用户和计算机对象的设置通常使用组策略对象（GPO）进行管理。 Azure Active Directory 域服务包含AADDC用户和AADDC计算机容器的内置GPO。 可以自定义这些内置的GPO，根据环境需要配置组策略。 Azure AD DC 管理员组的成员在 Azure AD DS 域中拥有组策略管理权限，还可以创建自定义 GPO 和组织单位（OU）。 有关什么是组策略及其工作方式详细信息，请参阅 [组策略概述](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))。

在混合环境中，在本地 AD DS 环境中配置的组策略不会同步到 Azure AD DS。 如果要为 Azure AD DS 中的用户或计算机定义配置设置，请编辑其中一个默认 GPO 或创建自定义 GPO。

本文 [管理组策略](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) 展示了如何安装组策略管理工具，如何编辑内置的GPO，以及如何创建自定义GPO。
