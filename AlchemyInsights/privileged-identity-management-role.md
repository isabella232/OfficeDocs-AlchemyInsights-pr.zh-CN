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
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="a3a28-102"> (PIM) 角色的特权身份管理</span><span class="sxs-lookup"><span data-stu-id="a3a28-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="a3a28-103">**激活角色后不授予权限**</span><span class="sxs-lookup"><span data-stu-id="a3a28-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="a3a28-104">当您在 Azure AD 特权标识管理 (PIM) 中激活角色时，激活可能不会立即传播到需要特权角色的所有门户。</span><span class="sxs-lookup"><span data-stu-id="a3a28-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="a3a28-105">有时，即使更改已传播，门户中的 web 缓存也可能导致更改不会立即生效。</span><span class="sxs-lookup"><span data-stu-id="a3a28-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="a3a28-106">如果你的激活延迟，请按照以下步骤操作：</span><span class="sxs-lookup"><span data-stu-id="a3a28-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="a3a28-107">注销 Azure 门户，然后重新登录。</span><span class="sxs-lookup"><span data-stu-id="a3a28-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="a3a28-108">当您激活 Azure AD 角色或 Azure 资源角色时，您将看到激活的阶段。</span><span class="sxs-lookup"><span data-stu-id="a3a28-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="a3a28-109">完成所有阶段后，您将看到 "注销" 链接。</span><span class="sxs-lookup"><span data-stu-id="a3a28-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="a3a28-110">您可以使用此链接注销。这将解决激活延迟的大多数情况。</span><span class="sxs-lookup"><span data-stu-id="a3a28-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="a3a28-111">在 PIM 中，验证您是否列为角色的成员。</span><span class="sxs-lookup"><span data-stu-id="a3a28-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="a3a28-112">如果要激活 Exchange 管理员角色，请确保注销并重新登录。</span><span class="sxs-lookup"><span data-stu-id="a3a28-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="a3a28-113">如果问题仍然存在，请打开支持票证并将其作为问题引发。</span><span class="sxs-lookup"><span data-stu-id="a3a28-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="a3a28-114">如果您使用您的 Exchange 管理员角色来访问安全与合规中心，请参阅下一步。</span><span class="sxs-lookup"><span data-stu-id="a3a28-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="a3a28-115">如果要激活某个角色以访问安全与合规中心，或者如果要激活 SharePoint 管理员角色，您将在几分钟内经历几分钟的激活延迟。</span><span class="sxs-lookup"><span data-stu-id="a3a28-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="a3a28-116">这是一个已知问题，我们正在与这些团队积极合作，尽快解决此问题。</span><span class="sxs-lookup"><span data-stu-id="a3a28-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="a3a28-117">有关更多信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="a3a28-117">For more information, see:</span></span>

- [<span data-ttu-id="a3a28-118">在 PIM 中激活我的 Azure AD 角色</span><span class="sxs-lookup"><span data-stu-id="a3a28-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="a3a28-119">在 PIM 中激活我的 Azure 资源角色</span><span class="sxs-lookup"><span data-stu-id="a3a28-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="a3a28-120">**停用角色或角色激活过期后不删除权限**</span><span class="sxs-lookup"><span data-stu-id="a3a28-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="a3a28-121">在 Azure AD 特权标识管理中停用角色或在角色激活期到期后，可能会有延迟，你仍可以继续访问。</span><span class="sxs-lookup"><span data-stu-id="a3a28-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="a3a28-122">如果您的停用延迟，请按照以下步骤操作：</span><span class="sxs-lookup"><span data-stu-id="a3a28-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="a3a28-123">如果要停用 Exchange 管理员角色或角色激活期已过期，并且在删除权限之前发现了一个严重的延迟，请打开支持票证，并告知支持工程师，以帮助您使用特权访问管理 (PAM) 团队在 Office 内部解决此问题。</span><span class="sxs-lookup"><span data-stu-id="a3a28-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="a3a28-124">如果激活期已过，但您仍在浏览器会话打开，请关闭浏览器。</span><span class="sxs-lookup"><span data-stu-id="a3a28-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="a3a28-125">您可以继续使用该角色，直到您关闭该会话。</span><span class="sxs-lookup"><span data-stu-id="a3a28-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="a3a28-126">这是一个已知问题，在激活过期后，我们会看到一个潜在的修补程序，以主动吊销每个会话。</span><span class="sxs-lookup"><span data-stu-id="a3a28-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="a3a28-127">如果您的延迟与这两个场景不同，请打开支持票证。</span><span class="sxs-lookup"><span data-stu-id="a3a28-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
