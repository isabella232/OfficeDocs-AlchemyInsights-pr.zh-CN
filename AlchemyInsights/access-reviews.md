---
title: 访问审查
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7767"
ms.openlocfilehash: b2ba50c4f8e667f81b638ba480fa846e149c3d43
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013919"
---
# <a name="access-reviews"></a>访问审查

1. **启用访问评审**：可以在创建新的访问包或编辑现有访问包时启用评价。 [在 Azure AD 权利](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) 管理中创建访问包的访问评审，介绍如何启用访问包的访问评审。

1. **Review Access**： Azure AD entitlement management simplifies how enterprises manage access to groups， applications， and SharePoint sites. [在 Azure AD](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) 权利管理中查看访问包的访问描述如何对分配了访问包的其他用户执行访问评审，这些用户访问是指定的审阅者。

1. **自行查看** 访问：在 [Azure AD](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-self-review) 权利管理中自审阅访问包描述用户如何自行查看其分配的访问权限 (包) 。

1. 在大多数情况下，最终用户将在访问面板中查找等待其 **回复的审阅**。 这仅适用于组和应用程序审阅，不适用于角色。 对于角色的所有访问评审，最终用户必须导航到 PIM (Azure AD Privileged Identity Management) 完成审阅。

    1. 登录到 Azure 门户。
    2. 导航到 Azure AD PIM。
    3. 在左侧导航窗格中，选择 **"任务**  >  **审阅访问权限"。**
    
有关详细信息，请参阅：

- [在 PIM 中执行对 Azure AD 目录角色的访问评审 ](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-perform-security-review/)
- [在 PIM 中执行 Azure 资源角色的访问评审](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-perform-access-review/)