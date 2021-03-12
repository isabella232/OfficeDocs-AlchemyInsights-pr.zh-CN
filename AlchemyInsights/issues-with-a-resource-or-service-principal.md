---
title: 资源或服务主体的问题
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
- "9004336"
- "7741"
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2021
ms.locfileid: "50716121"
---
# <a name="issues-with-a-resource-or-service-principal"></a><span data-ttu-id="f7c68-102">资源或服务主体的问题</span><span class="sxs-lookup"><span data-stu-id="f7c68-102">Issues with a Resource or Service Principal</span></span>

1. <span data-ttu-id="f7c68-103">如果你刚刚开始 [，Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) 中的应用程序和服务主体对象将描述 Azure Active Directory 中的应用程序注册、应用程序对象和服务主体：它们是什么、如何使用以及它们如何相互关联。</span><span class="sxs-lookup"><span data-stu-id="f7c68-103">If you are just getting started, [Application and service principal objects in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) describes application registration, application objects, and service principals in Azure Active Directory: what they are, how they are used, and how they are related to each other.</span></span> <span data-ttu-id="f7c68-104">还演示了多租户示例方案，以说明应用程序的应用程序对象与相应的服务主体对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="f7c68-104">A multi-tenant example scenario is also presented to illustrate the relationship between an application's application object and corresponding service principal objects.</span></span>
2. <span data-ttu-id="f7c68-105">通过读取 Azure Active Directory 中的应用程序和服务主体对象，可以了解有关应用程序和服务主体之间的关系 [的更多信息](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)。</span><span class="sxs-lookup"><span data-stu-id="f7c68-105">You can learn more about the relationship between applications and service principals by reading [applications and service principal objects in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).</span></span>
3. <span data-ttu-id="f7c68-106">如何：使用门户创建可以访问资源的[Azure AD](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)应用程序和服务主体，将演示如何创建新的 Azure Active Directory (Azure AD) 应用程序和服务主体，这些应用程序和服务主体可用于基于角色的访问控制。</span><span class="sxs-lookup"><span data-stu-id="f7c68-106">[How to: Use the portal to create an Azure AD application and service principal that can access resources](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) shows you how to create a new Azure Active Directory (Azure AD) application and service principal that can be used with the role-based access control.</span></span>
4. <span data-ttu-id="f7c68-107">使用 [服务主体 API，](https://docs.microsoft.com/graph/api/resources/serviceprincipal)可以编程方式管理应用程序实例，并控制应用程序可以在租户内执行哪些操作。</span><span class="sxs-lookup"><span data-stu-id="f7c68-107">With the [service principal API](https://docs.microsoft.com/graph/api/resources/serviceprincipal), you can programmatically manage instances of applications and control what an application can do within your tenant.</span></span>
5. <span data-ttu-id="f7c68-108">[servicePrincipal 资源](https://docs.microsoft.com/graph/api/resources/serviceprincipal) 类型列出了 servicePrincipal 资源类型的所有属性和方法。</span><span class="sxs-lookup"><span data-stu-id="f7c68-108">[servicePrincipal resource type](https://docs.microsoft.com/graph/api/resources/serviceprincipal) lists all properties and methods for the servicePrincipal resource type.</span></span>
6. <span data-ttu-id="f7c68-109">[Azure AD Graph 和 Microsoft Graph 之间的](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) 资源类型差异突出显示了 Azure AD Graph 和 Microsoft Graph 资源之间的差异。</span><span class="sxs-lookup"><span data-stu-id="f7c68-109">[Resource type differences between Azure AD Graph and Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) highlights differences between Azure AD Graph and Microsoft Graph resources.</span></span> <span data-ttu-id="f7c68-110">它显示名称不同或不可用的资源;它还突出显示 Microsoft Graph beta 版本（而非 v1.0 版本）中可用的资源。</span><span class="sxs-lookup"><span data-stu-id="f7c68-110">It shows resources that have different names or are not available; it also highlights resources available in the beta version of Microsoft Graph but not in the v1.0 version.</span></span>

<span data-ttu-id="f7c68-111">**来宾用户的问题**</span><span class="sxs-lookup"><span data-stu-id="f7c68-111">**Issues with Guest Users**</span></span>

- <span data-ttu-id="f7c68-112">[快速入门：在 Azure](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) 门户中向目录添加来宾用户可展示如何通过 Azure 门户向 Azure AD 目录添加新来宾用户、发送邀请，以及查看来宾用户的邀请兑换过程。</span><span class="sxs-lookup"><span data-stu-id="f7c68-112">[Quickstart: Add guest users to your directory in the Azure portal](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) shows you how to add a new guest user to your Azure AD directory via the Azure portal, send an invitation, and see what the guest user's invitation redemption process looks like.</span></span>
- <span data-ttu-id="f7c68-113">[教程：在 Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) 中创建用户流介绍如何使用 Azure 门户创建一些建议的用户流。</span><span class="sxs-lookup"><span data-stu-id="f7c68-113">[Tutorial: Create user flows in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) shows you how to create some recommended user flows by using the Azure portal.</span></span> <span data-ttu-id="f7c68-114">若要了解如何在应用程序中设置资源所有者密码凭据 (ROPC) 流，请参阅在 Azure AD B2C 中配置资源所有者密码凭据流。</span><span class="sxs-lookup"><span data-stu-id="f7c68-114">If you are looking for information about how to set up a resource owner password credentials (ROPC) flow in your application, see Configure the resource owner password credentials flow in Azure AD B2C.</span></span>
