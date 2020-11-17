---
title: 特权标识管理角色
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
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086230"
---
# <a name="privileged-identity-managementpim-role"></a> (PIM) 角色的特权身份管理

**激活角色后不授予权限**

当您在 Azure AD 特权标识管理 (PIM) 中激活角色时，激活可能不会立即传播到需要特权角色的所有门户。 有时，即使更改已传播，门户中的 web 缓存也可能导致更改不会立即生效。

如果你的激活延迟，请按照以下步骤操作：

1. 注销 Azure 门户，然后重新登录。 当您激活 Azure AD 角色或 Azure 资源角色时，您将看到激活的阶段。 完成所有阶段后，您将看到 "注销" 链接。 您可以使用此链接注销。这将解决激活延迟的大多数情况。
2. 在 PIM 中，验证您是否列为角色的成员。
3. 如果要激活 Exchange 管理员角色，请确保注销并重新登录。 如果问题仍然存在，请打开支持票证并将其作为问题引发。 如果您使用您的 Exchange 管理员角色来访问安全与合规中心，请参阅下一步。
4. 如果要激活某个角色以访问安全与合规中心，或者如果要激活 SharePoint 管理员角色，您将在几分钟内经历几分钟的激活延迟。 这是一个已知问题，我们正在与这些团队积极合作，尽快解决此问题。

有关更多信息，请参阅：

- [在 PIM 中激活我的 Azure AD 角色](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [在 PIM 中激活我的 Azure 资源角色](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**停用角色或角色激活过期后不删除权限**

在 Azure AD 特权标识管理中停用角色或在角色激活期到期后，可能会有延迟，你仍可以继续访问。

如果您的停用延迟，请按照以下步骤操作：

1. 如果要停用 Exchange 管理员角色或角色激活期已过期，并且在删除权限之前发现了一个严重的延迟，请打开支持票证，并告知支持工程师，以帮助您使用特权访问管理 (PAM) 团队在 Office 内部解决此问题。
2. 如果激活期已过，但您仍在浏览器会话打开，请关闭浏览器。 您可以继续使用该角色，直到您关闭该会话。 这是一个已知问题，在激活过期后，我们会看到一个潜在的修补程序，以主动吊销每个会话。

如果您的延迟与这两个场景不同，请打开支持票证。
