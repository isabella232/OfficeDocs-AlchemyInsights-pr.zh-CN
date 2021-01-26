---
title: 查询 Microsoft Graph API
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
- "9004345"
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950665"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="678ef-102">查询 Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="678ef-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="678ef-103">本主题还适用于仍在使用 Azure AD Graph API 的开发人员。</span><span class="sxs-lookup"><span data-stu-id="678ef-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="678ef-104">但是， **强烈建议** 将 Microsoft Graph 用于所有目录、标识和访问管理方案。</span><span class="sxs-lookup"><span data-stu-id="678ef-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="678ef-105">**身份验证或授权问题**</span><span class="sxs-lookup"><span data-stu-id="678ef-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="678ef-106">如果你的应用无法获取令牌来调用 Microsoft Graph，请选择"获取访问令牌 **(身份验证)** Microsoft Graph"类别以获取有关本主题的更具体的帮助和支持。</span><span class="sxs-lookup"><span data-stu-id="678ef-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="678ef-107">如果你的应用在调用 Microsoft Graph 时收到 **401 或 403** 授权错误，请选择"获取访问被拒绝错误 **(授权)** Microsoft Graph API"类别，获取有关本主题的更具体的帮助和支持。</span><span class="sxs-lookup"><span data-stu-id="678ef-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="678ef-108">**我想要使用 Microsoft Graph，但不确定从何处开始**</span><span class="sxs-lookup"><span data-stu-id="678ef-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="678ef-109">若要了解有关 Microsoft Graph 的更多信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="678ef-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="678ef-110">Microsoft Graph 概述</span><span class="sxs-lookup"><span data-stu-id="678ef-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="678ef-111">Microsoft Graph 中的标识和访问管理概述</span><span class="sxs-lookup"><span data-stu-id="678ef-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="678ef-112">开始构建 Microsoft Graph 应用</span><span class="sxs-lookup"><span data-stu-id="678ef-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="678ef-113">**Microsoft Graph 资源管理器** - 在租户或演示租户中测试 Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="678ef-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="678ef-114">**我想要使用 Microsoft Graph，但它是否支持所需的 v1.0 目录 API？**</span><span class="sxs-lookup"><span data-stu-id="678ef-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="678ef-115">Microsoft Graph 是推荐的目录、标识和访问管理的 API。</span><span class="sxs-lookup"><span data-stu-id="678ef-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="678ef-116">但是，Azure AD Graph 和 Microsoft Graph 中可能存在一些差异。</span><span class="sxs-lookup"><span data-stu-id="678ef-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="678ef-117">请查看以下文章，其中重点介绍了最新的差异，以帮助你做出选择：</span><span class="sxs-lookup"><span data-stu-id="678ef-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="678ef-118">Azure AD Graph 和 Microsoft Graph 之间的资源类型差异</span><span class="sxs-lookup"><span data-stu-id="678ef-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="678ef-119">Azure AD Graph 和 Microsoft Graph 之间的属性差异</span><span class="sxs-lookup"><span data-stu-id="678ef-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="678ef-120">Azure AD 和 Microsoft Graph 之间的方法差异</span><span class="sxs-lookup"><span data-stu-id="678ef-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="678ef-121">**当我查询 *用户对象* 时，其许多属性都缺失**</span><span class="sxs-lookup"><span data-stu-id="678ef-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="678ef-122">`GET https://graph.microsoft.com/v1.0/users` 仅返回 11 个属性，因为 Microsoft Graph 自动选择要返回的默认 *用户* 属性集。</span><span class="sxs-lookup"><span data-stu-id="678ef-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="678ef-123">如果需要其他用户 *属性，* 请使用$select来选取应用程序所需的属性。</span><span class="sxs-lookup"><span data-stu-id="678ef-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="678ef-124">首先在 **Microsoft Graph 资源管理器中试用** 。</span><span class="sxs-lookup"><span data-stu-id="678ef-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="678ef-125">**一些用户属性值 *为 null，* 即使我们知道它们已设置**</span><span class="sxs-lookup"><span data-stu-id="678ef-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="678ef-126">最可能的解释是应用程序已被授予 *User.ReadBasic.All* 权限。</span><span class="sxs-lookup"><span data-stu-id="678ef-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="678ef-127">这允许应用程序读取一组有限的用户属性，将所有其他属性返回为 null，即使之前已设置这些属性。</span><span class="sxs-lookup"><span data-stu-id="678ef-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="678ef-128">请尝试改为授予应用程序 *User.Read.All* 权限。</span><span class="sxs-lookup"><span data-stu-id="678ef-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="678ef-129">有关详细信息，请参阅 [Microsoft Graph 用户权限](https://docs.microsoft.com/graph/permissions-reference#user-permissions)。</span><span class="sxs-lookup"><span data-stu-id="678ef-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="678ef-130">**我在使用 OData 查询参数筛选请求中数据时遇到问题**</span><span class="sxs-lookup"><span data-stu-id="678ef-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="678ef-131">虽然 Microsoft Graph 支持各种 OData 查询参数，但从 Microsoft Graph 中的 *directoryObject*) 继承的目录服务 (资源并不完全支持这些参数。</span><span class="sxs-lookup"><span data-stu-id="678ef-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="678ef-132">在 Microsoft Graph 中，Azure AD Graph 中的大多数限制仍然存在：</span><span class="sxs-lookup"><span data-stu-id="678ef-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="678ef-133">**不支持**：$count、$search，$filter null 值 *或不\*\*为 null* 值时返回</span><span class="sxs-lookup"><span data-stu-id="678ef-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="678ef-134">**不支持：$filter** 某些属性 (查看有关哪些属性可筛选的资源) </span><span class="sxs-lookup"><span data-stu-id="678ef-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="678ef-135">**不支持**：同时分页、筛选和排序</span><span class="sxs-lookup"><span data-stu-id="678ef-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="678ef-136">**不支持：** 对关系进行筛选。</span><span class="sxs-lookup"><span data-stu-id="678ef-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="678ef-137">例如，查找英国工程组的所有成员。</span><span class="sxs-lookup"><span data-stu-id="678ef-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="678ef-138">**部分支持**：$orderby *displayName* 和 userPrincipalName (displayName 和 userPrincipalName *) 组*</span><span class="sxs-lookup"><span data-stu-id="678ef-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="678ef-139">**部分支持**：$filter (仅支持 *eq* *、startswith\*\*或*，*以及*，并限制任何 *)* 支持，$expand (展开单个对象的关系将返回所有关系，但扩展对象的关系集合是有限的) </span><span class="sxs-lookup"><span data-stu-id="678ef-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="678ef-140">有关详细信息，请参阅使用 [查询参数自定义响应](https://docs.microsoft.com/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="678ef-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="678ef-141">**我调用的 API 不起作用 - 在哪里可以执行更多测试？**</span><span class="sxs-lookup"><span data-stu-id="678ef-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="678ef-142">**Microsoft Graph 资源管理器**- 在租户或演示租户中测试 Microsoft Graph API，并查看 Microsoft Graph 资源管理器中的示例查询。 </span><span class="sxs-lookup"><span data-stu-id="678ef-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="678ef-143">**当我查询数据时，似乎我重新设置了不完整的数据**</span><span class="sxs-lookup"><span data-stu-id="678ef-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="678ef-144">如果要像用户 (查询集合) ，Microsoft Graph将使用服务器端页面限制，以便始终返回具有默认页面大小的结果。</span><span class="sxs-lookup"><span data-stu-id="678ef-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="678ef-145">你的应用应始终希望浏览从服务返回的集合。</span><span class="sxs-lookup"><span data-stu-id="678ef-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="678ef-146">有关详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="678ef-146">For more information, see:</span></span>

- [<span data-ttu-id="678ef-147">Microsoft Graph 最佳实践</span><span class="sxs-lookup"><span data-stu-id="678ef-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="678ef-148">在应用中对 Microsoft Graph 数据进行分页</span><span class="sxs-lookup"><span data-stu-id="678ef-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="678ef-149">**我的应用过慢，并且也受到限制。我可以进行哪些改进？**</span><span class="sxs-lookup"><span data-stu-id="678ef-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="678ef-150">根据你的方案，有多种不同的选项可供选择，使应用程序更具有性能;在某些情况下，当您对应用程序进行过多调用时，服务 (很容易受到) 。</span><span class="sxs-lookup"><span data-stu-id="678ef-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="678ef-151">有关详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="678ef-151">To learn more, see:</span></span>

- [<span data-ttu-id="678ef-152">Microsoft Graph 最佳实践</span><span class="sxs-lookup"><span data-stu-id="678ef-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="678ef-153">批处理请求</span><span class="sxs-lookup"><span data-stu-id="678ef-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="678ef-154">通过 delta 查询跟踪更改</span><span class="sxs-lookup"><span data-stu-id="678ef-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="678ef-155">通过 Webhook 获取更改通知</span><span class="sxs-lookup"><span data-stu-id="678ef-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="678ef-156">限制指南</span><span class="sxs-lookup"><span data-stu-id="678ef-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="678ef-157">**在哪里可以找到有关错误和已知问题的详细信息？**</span><span class="sxs-lookup"><span data-stu-id="678ef-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="678ef-158">Microsoft Graph 错误响应信息</span><span class="sxs-lookup"><span data-stu-id="678ef-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="678ef-159">Microsoft Graph 已知问题</span><span class="sxs-lookup"><span data-stu-id="678ef-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="678ef-160">**在哪里可以检查服务可用性和连接状态？**</span><span class="sxs-lookup"><span data-stu-id="678ef-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="678ef-161">可通过 Microsoft Graph 访问的基础服务的服务可用性和连接可能会影响 Microsoft Graph 的总体可用性和性能。</span><span class="sxs-lookup"><span data-stu-id="678ef-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="678ef-162">对于 Azure Active Directory 服务运行状况，请检查 Azure 状态页中列出的安全 **+** [标识服务的状态](https://azure.microsoft.com/status/)。</span><span class="sxs-lookup"><span data-stu-id="678ef-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="678ef-163">对于参与 Microsoft Graph 的 Office 服务，请检查 Office 服务运行状况仪表板中列出的 [服务的状态](https://portal.office.com/adminportal/home#/servicehealth)。</span><span class="sxs-lookup"><span data-stu-id="678ef-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
