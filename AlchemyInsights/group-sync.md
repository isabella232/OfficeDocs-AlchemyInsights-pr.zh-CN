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
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2021
ms.locfileid: "50243897"
---
# <a name="group-sync"></a><span data-ttu-id="c1734-102">组同步</span><span class="sxs-lookup"><span data-stu-id="c1734-102">Group sync</span></span>

<span data-ttu-id="c1734-103">本文提供关于组同步的指南。</span><span class="sxs-lookup"><span data-stu-id="c1734-103">This article provides guidance on group synchronization.</span></span>

1. <span data-ttu-id="c1734-104">如果全局管理员或组所有者无法在 Azure 门户中修改组属性或添加成员或分配所有者，请确保组的权限来源是 Azure Active Directory (Azure AD)，以便全局管理员或组所有者修改组。</span><span class="sxs-lookup"><span data-stu-id="c1734-104">If a global admin or group owner is not able to modify group properties or add members or assign owners in the Azure portal, ensure the source of the authority for the group is Azure Active Directory (Azure AD) for the global admin or group owner to modify the group.</span></span>
2. <span data-ttu-id="c1734-105">在尝试删除 Azure AD 中的同步组之前，请确保[已删除所有分配的许可证](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced)以避免错误。</span><span class="sxs-lookup"><span data-stu-id="c1734-105">Before attempting to delete a synced group in Azure AD, ensure you have [deleted all assigned licenses](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) to avoid errors.</span></span>

<span data-ttu-id="c1734-106">如果要了解如何同步用户、组和联系人，请参阅[Azure AD Connect 同步](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)，然后按照 [使用 Azure AD Connect 将预置组同步到 Azure](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support)以用 AD connect 同步预置组。</span><span class="sxs-lookup"><span data-stu-id="c1734-106">For understanding how to sync users, groups and contacts, see [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), and follow [Syncing an on-premises group to Azure using Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to sync on-perm groups using AD connect.</span></span>

<span data-ttu-id="c1734-107">请按照本指南[在同步过程中排除故障](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors)以排除同步过程中的常见故障。</span><span class="sxs-lookup"><span data-stu-id="c1734-107">Follow this guide [Troubleshooting Errors during synchronization](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) to troubleshoot common errors during synchronization.</span></span>

