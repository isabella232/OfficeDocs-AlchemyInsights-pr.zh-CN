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
ms.openlocfilehash: 92d4aa46c8385035275d7ccbb361a9199e7f5924a87998f3beba32a2b02bbcc9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938613"
---
# <a name="access-reviews"></a>访问审查

1. **启用访问评审**：可以在创建新的访问包或编辑现有访问包时启用评价。 [Create an access review of an access package in Azure AD entitlement management](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) 介绍如何启用访问包的访问评审。

1. **查看访问**：Azure AD 权利管理简化了企业如何管理对组、应用程序和网站SharePoint访问。 [Review access of an access package in Azure AD entitlement management](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) 介绍如何为分配了访问包的其他用户（作为指定审阅者）执行访问评审。

1. **Review Access for Yourself**： [Self-review of an access package in Azure AD entitlement management](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-self-review) 描述用户如何自行审阅其分配的访问权限包 () 。

1. 在大多数情况下，最终用户将在访问面板中发现其回复等待 **审阅**。 这仅适用于组和应用程序审阅，不适用于角色。 对于角色的所有访问评审，最终用户必须导航到 AZURE AD Privileged Identity Management (PIM) 才能完成审查。

    1. 登录到 Azure 门户。
    2. 导航到 Azure AD PIM。
    3. 在左侧导航窗格中，选择"**任务**  >  **""审阅访问权限"。**
    
有关详细信息，请参阅：

- [在 PIM 中执行 Azure AD 目录角色的访问评审 ](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-perform-security-review/)
- [在 PIM 中执行 Azure 资源角色的访问评审](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-perform-access-review/)