---
title: 关于 Yammer 中的标识
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146748"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="8cb2c-102">关于 Yammer 中的标识</span><span class="sxs-lookup"><span data-stu-id="8cb2c-102">About identity in Yammer</span></span>

<span data-ttu-id="8cb2c-103">建议所有网络均执行以下步骤以避免标识相关问题：</span><span class="sxs-lookup"><span data-stu-id="8cb2c-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="8cb2c-104">为 Azure AD 中的用户预配 Microsoft 365 帐户后强制使用 Office 365 标识，以确保所有用户都使用其主要 Microsoft 365 帐户登录。</span><span class="sxs-lookup"><span data-stu-id="8cb2c-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="8cb2c-105">有关详细信息，请参阅[强制 Yammer 用户使用 Office 365 标识](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)。</span><span class="sxs-lookup"><span data-stu-id="8cb2c-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="8cb2c-106">合并多个 Yammer 网络。</span><span class="sxs-lookup"><span data-stu-id="8cb2c-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="8cb2c-107">传统 Yammer 配置允许将多个 Yammer 网络连接到一个租户。</span><span class="sxs-lookup"><span data-stu-id="8cb2c-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="8cb2c-108">有关详细信息，请参阅[网络迁移 - 合并多个 Yammer 网络](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)。</span><span class="sxs-lookup"><span data-stu-id="8cb2c-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="8cb2c-109">（可选）强制执行 Yammer 许可，以阻止没有许可证的 Yammer 用户。</span><span class="sxs-lookup"><span data-stu-id="8cb2c-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="8cb2c-110">有关详细信息，请参阅[在 Office 365 中管理 Yammer 用户许可](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)。</span><span class="sxs-lookup"><span data-stu-id="8cb2c-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="8cb2c-111">最后，审核旧 Yammer 网络的用户列表，并挂起旧用户。</span><span class="sxs-lookup"><span data-stu-id="8cb2c-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="8cb2c-112">建议你挂起（停用）用户，而不是将其删除，因为删除操作是不可逆的。</span><span class="sxs-lookup"><span data-stu-id="8cb2c-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="8cb2c-113">有关详细信息，请参阅[在连接到 Office 365 的网络中审核 Yammer 用户](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365)和[删除用户](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)。</span><span class="sxs-lookup"><span data-stu-id="8cb2c-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="8cb2c-114">通过使用这些步骤配置 Yammer，你还可以将 Yammer 网络配置为适用于 Microsoft 365 的本机模式。</span><span class="sxs-lookup"><span data-stu-id="8cb2c-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="8cb2c-115">有关详细信息，请参阅[将 Yammer 网络配置为适用于 Microsoft 365 的本机模式](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode)。</span><span class="sxs-lookup"><span data-stu-id="8cb2c-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>