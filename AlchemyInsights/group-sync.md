---
title: 组同步
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 7e5ed69c34f8e7b922d7eef202af508152a7e04d7773581b32e43395571c6fbc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53987637"
---
# <a name="group-sync"></a>组同步

本文提供关于组同步的指南。

1. 如果全局管理员或组所有者无法在 Azure 门户中修改组属性或添加成员或分配所有者，请确保组的权限来源是 Azure Active Directory (Azure AD)，以便全局管理员或组所有者修改组。
2. 在尝试删除 Azure AD 中的同步组之前，请确保[已删除所有分配的许可证](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced)以避免错误。

如果要了解如何同步用户、组和联系人，请参阅[Azure AD Connect 同步](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)，然后按照 [使用 Azure AD Connect 将预置组同步到 Azure](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support)以用 AD connect 同步预置组。

请按照本指南[在同步过程中排除故障](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors)以排除同步过程中的常见故障。

