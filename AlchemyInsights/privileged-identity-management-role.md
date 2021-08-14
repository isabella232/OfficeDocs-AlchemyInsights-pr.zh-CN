---
title: Privileged Identity Management角色
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
- "9003230"
- "6825"
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973219"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management (PIM) 角色

**激活角色后不授予权限**

在 PIM Privileged Identity Management (Azure AD) 中激活角色时，激活可能不会立即传播到需要特权角色的所有门户。 有时，即使传播了更改，门户中的 Web 缓存也可能会导致更改不会立即生效。

如果激活延迟，请按照以下步骤操作：

1. 注销 Azure 门户，然后重新登录。 当你激活 Azure AD 角色或 Azure 资源角色时，你将看到激活的阶段。 完成所有阶段后，你将看到"注销"链接。 可以使用此链接进行注销。这将解决激活延迟的大多数情况下。
2. 在 PIM 中，验证是否列出了该角色的成员。
3. 如果要激活 Exchange 管理员角色，请确保注销并重新登录。 如果问题仍然存在，请打开支持票证，并作为问题提出。 如果使用管理员角色Exchange安全与合规中心，请参阅下一步。
4. 如果要激活角色以访问安全与合规中心，或者要激活 SharePoint 管理员角色，将遇到一些激活延迟，从几分钟到几小时。 这是一个已知问题，我们正在积极与这些团队合作，尽快解决此问题。

有关详细信息，请参阅：

- [在 PIM 中激活我的 Azure AD 角色](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [在 PIM 中激活我的 Azure 资源角色](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**停用角色或角色激活过期后不会删除权限**

在 Azure AD Privileged Identity Management中停用角色时，或当角色激活期到期时，可能会存在继续具有访问权限的延迟。

如果停用延迟，请按照以下步骤操作：

1. 如果要停用 Exchange 管理员角色或角色激活期过期，并且发现权限删除前有明显延迟，请打开支持票证，并通知支持工程师帮助你向 Office 内的 Privileged Access Management (PAM) 团队提交票证。
2. 如果激活期已过期，但仍打开浏览器会话，请关闭浏览器。 在关闭该会话之前，可以继续使用该角色。 这是一个已知问题，我们正在寻找在激活到期后主动撤销每个会话的潜在解决方法。

如果你的延迟不同于这两种方案，请打开支持票证。
