---
title: 删除租户
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2020
ms.locfileid: "49477647"
---
# <a name="delete-tenant"></a><span data-ttu-id="0cbf3-102">删除租户</span><span class="sxs-lookup"><span data-stu-id="0cbf3-102">Delete tenant</span></span>

<span data-ttu-id="0cbf3-103">若要删除 Azure AD，请确保：</span><span class="sxs-lookup"><span data-stu-id="0cbf3-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="0cbf3-104">您是目录的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="0cbf3-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="0cbf3-105">您未使用在登录帐户中具有默认目录（如 contoso.onmicrosoft.com）的帐户登录，如 admin@contoso.onmicrosoft.com。</span><span class="sxs-lookup"><span data-stu-id="0cbf3-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="0cbf3-106">删除前删除目录中所有活动的应用程序。</span><span class="sxs-lookup"><span data-stu-id="0cbf3-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="0cbf3-107">若要删除活动的应用程序，请导航到 "应用注册" 并删除现有的应用程序。</span><span class="sxs-lookup"><span data-stu-id="0cbf3-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="0cbf3-108">没有任何 Microsoft Online Services 的活动订阅，例如 Microsoft Azure、Office 365 或与目录关联的 Azure AD Premium。</span><span class="sxs-lookup"><span data-stu-id="0cbf3-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="0cbf3-109">通过 Azure 支持和帐单转移订阅或加快活动订阅的取消。</span><span class="sxs-lookup"><span data-stu-id="0cbf3-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="0cbf3-110">了解有关如何取消 Office 365 和 Azure 订阅的详细信息。</span><span class="sxs-lookup"><span data-stu-id="0cbf3-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="0cbf3-111">有关将现有订阅关联或添加到租户的指南，请参阅 [将 azure 订阅关联或添加到 AZURE AD 租户](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)。</span><span class="sxs-lookup"><span data-stu-id="0cbf3-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="0cbf3-112">没有活动的许可证。</span><span class="sxs-lookup"><span data-stu-id="0cbf3-112">There are no Active license.</span></span> <span data-ttu-id="0cbf3-113">若要删除许可证，请参阅 how [to Remove 订阅 To remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)。</span><span class="sxs-lookup"><span data-stu-id="0cbf3-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="0cbf3-114">在尝试删除 Azure AD 时，目录中没有其他任何活动用户，而是将自己作为全局管理员。</span><span class="sxs-lookup"><span data-stu-id="0cbf3-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="0cbf3-115">删除任何其他活动用户，同时还需要删除租户中的自定义域名的任何依赖项，如使用 admin@contoso.com 创建的用户。</span><span class="sxs-lookup"><span data-stu-id="0cbf3-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="0cbf3-116">有关如何执行以下操作的更多详细步骤：</span><span class="sxs-lookup"><span data-stu-id="0cbf3-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="0cbf3-117">删除 "Azure Active Directory" 或 "订阅"，请参阅 [删除 Azure Active directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)。</span><span class="sxs-lookup"><span data-stu-id="0cbf3-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="0cbf3-118">删除目录中的应用程序，请参阅 [删除应用程序](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app)。</span><span class="sxs-lookup"><span data-stu-id="0cbf3-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
