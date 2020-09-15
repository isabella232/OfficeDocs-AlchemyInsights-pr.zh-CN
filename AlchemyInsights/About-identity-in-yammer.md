---
title: 关于 Yammer 中的标识
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664160"
---
# <a name="about-identity-in-yammer"></a>关于 Yammer 中的标识

建议所有网络均执行以下步骤以避免标识相关问题：

1. 为 Azure AD 中的用户预配 Microsoft 365 帐户后强制使用 Office 365 标识，以确保所有用户都使用其主要 Microsoft 365 帐户登录。 有关详细信息，请参阅[强制 Yammer 用户使用 Office 365 标识](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)。
2. 合并多个 Yammer 网络。 传统 Yammer 配置允许将多个 Yammer 网络连接到一个租户。 有关详细信息，请参阅[网络迁移 - 合并多个 Yammer 网络](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)。
3. （可选）强制执行 Yammer 许可，以阻止没有许可证的 Yammer 用户。 有关详细信息，请参阅[在 Office 365 中管理 Yammer 用户许可](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)。
4. 最后，审核旧 Yammer 网络的用户列表，并挂起旧用户。 建议你挂起（停用）用户，而不是将其删除，因为删除操作是不可逆的。 有关详细信息，请参阅[在连接到 Office 365 的网络中审核 Yammer 用户](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365)和[删除用户](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)。

通过使用这些步骤配置 Yammer，你还可以将 Yammer 网络配置为适用于 Microsoft 365 的本机模式。 有关详细信息，请参阅[将 Yammer 网络配置为适用于 Microsoft 365 的本机模式](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode)。