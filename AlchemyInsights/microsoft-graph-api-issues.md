---
title: Microsoft Graph API 问题
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
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/29/2021
ms.locfileid: "50716193"
---
# <a name="microsoft-graph-api-issues"></a><span data-ttu-id="70dac-102">Microsoft Graph API 问题</span><span class="sxs-lookup"><span data-stu-id="70dac-102">Microsoft Graph API issues</span></span>

<span data-ttu-id="70dac-103">本主题还适用于仍在使用 Azure AD Graph API 的开发人员。</span><span class="sxs-lookup"><span data-stu-id="70dac-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="70dac-104">但是， **强烈建议** 将 Microsoft Graph 用于所有目录、标识和访问管理方案。</span><span class="sxs-lookup"><span data-stu-id="70dac-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="70dac-105">**身份验证或授权问题**</span><span class="sxs-lookup"><span data-stu-id="70dac-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="70dac-106">如果你的应用无法获取令牌来调用 Microsoft Graph，请选择"获取访问令牌 (身份验证) Microsoft **Graph"** 类别以获取有关本主题的更具体的帮助和支持。</span><span class="sxs-lookup"><span data-stu-id="70dac-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="70dac-107">如果你的应用在调用 Microsoft Graph 时收到 **401 或 403** 授权错误，请选取"获取拒绝访问错误 **(授权)** Microsoft Graph API"类别，获取有关本主题的更具体的帮助和支持。</span><span class="sxs-lookup"><span data-stu-id="70dac-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="70dac-108">**我想要使用 Microsoft Graph，但不确定从何处开始**</span><span class="sxs-lookup"><span data-stu-id="70dac-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

- [<span data-ttu-id="70dac-109">Microsoft Graph 概述</span><span class="sxs-lookup"><span data-stu-id="70dac-109">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="70dac-110">Microsoft Graph 中的标识和访问管理概述</span><span class="sxs-lookup"><span data-stu-id="70dac-110">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="70dac-111">构建 Microsoft Graph 应用入门</span><span class="sxs-lookup"><span data-stu-id="70dac-111">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="70dac-112">**Microsoft Graph 资源管理器** - 在租户或演示租户中测试 Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="70dac-112">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="70dac-113">**我想要使用 Microsoft Graph，但它是否支持所需的 v1.0 目录 API？**</span><span class="sxs-lookup"><span data-stu-id="70dac-113">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="70dac-114">Microsoft Graph 是目录、标识和访问管理的推荐 API。</span><span class="sxs-lookup"><span data-stu-id="70dac-114">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="70dac-115">但是，Azure AD Graph 和 Microsoft Graph 中的可能功能之间仍有一些差异。</span><span class="sxs-lookup"><span data-stu-id="70dac-115">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="70dac-116">查看以下文章，其中重点介绍了最新的差异，以帮助你做出选择：</span><span class="sxs-lookup"><span data-stu-id="70dac-116">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="70dac-117">Azure AD Graph 和 Microsoft Graph 之间的资源类型差异</span><span class="sxs-lookup"><span data-stu-id="70dac-117">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="70dac-118">Azure AD Graph 和 Microsoft Graph 之间的属性差异</span><span class="sxs-lookup"><span data-stu-id="70dac-118">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="70dac-119">Azure AD 和 Microsoft Graph 之间的方法差异</span><span class="sxs-lookup"><span data-stu-id="70dac-119">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="70dac-120">**我调用的 API 不起作用 - 在哪里可以执行更多测试？**</span><span class="sxs-lookup"><span data-stu-id="70dac-120">**The API I am calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="70dac-121">**Microsoft Graph 资源管理器**- 在租户或演示租户中测试 Microsoft Graph API，并查看 Microsoft Graph 资源管理器中的示例查询。 </span><span class="sxs-lookup"><span data-stu-id="70dac-121">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="70dac-122">**我的应用过慢，并且正被限制。我可以进行哪些改进？**</span><span class="sxs-lookup"><span data-stu-id="70dac-122">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="70dac-123">根据你的方案，有多种选项可供选择，使应用程序更具有性能;在某些情况下，当您对应用程序执行过多调用时，服务 (将不太容易) 。</span><span class="sxs-lookup"><span data-stu-id="70dac-123">Depending on your scenario, there are a variety of options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

- [<span data-ttu-id="70dac-124">Microsoft Graph 最佳做法</span><span class="sxs-lookup"><span data-stu-id="70dac-124">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="70dac-125">批处理请求</span><span class="sxs-lookup"><span data-stu-id="70dac-125">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="70dac-126">通过增量查询跟踪更改</span><span class="sxs-lookup"><span data-stu-id="70dac-126">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="70dac-127">通过 Webhook 获取更改通知</span><span class="sxs-lookup"><span data-stu-id="70dac-127">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="70dac-128">限制指南</span><span class="sxs-lookup"><span data-stu-id="70dac-128">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="70dac-129">**在哪里可以找到有关错误和已知问题的详细信息？**</span><span class="sxs-lookup"><span data-stu-id="70dac-129">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="70dac-130">Microsoft Graph 错误响应信息</span><span class="sxs-lookup"><span data-stu-id="70dac-130">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="70dac-131">Microsoft Graph 已知问题</span><span class="sxs-lookup"><span data-stu-id="70dac-131">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="70dac-132">**在哪里可以检查服务可用性和连接状态？**</span><span class="sxs-lookup"><span data-stu-id="70dac-132">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="70dac-133">可通过 Microsoft Graph 访问的基础服务的服务可用性和连接性可能会影响 Microsoft Graph 的总体可用性和性能。</span><span class="sxs-lookup"><span data-stu-id="70dac-133">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="70dac-134">对于 Azure Active Directory 服务运行状况，请检查 Azure 状态页中列出的安全 **+** [标识服务的状态](https://azure.microsoft.com/status/)。</span><span class="sxs-lookup"><span data-stu-id="70dac-134">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="70dac-135">对于参与 Microsoft Graph 的 Office 服务，请检查 Office 服务运行状况仪表板中列出的服务 [的状态](https://portal.office.com/adminportal/home#/servicehealth)。</span><span class="sxs-lookup"><span data-stu-id="70dac-135">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="70dac-136">Microsoft Graph 授权错误可能是多个不同问题的结果，大多数问题会产生 401 或 403 错误。</span><span class="sxs-lookup"><span data-stu-id="70dac-136">Microsoft Graph authorization errors can be a result of several different issues, most of which generate a 401 or 403 error.</span></span> <span data-ttu-id="70dac-137">例如，以下情况可能会导致授权错误：</span><span class="sxs-lookup"><span data-stu-id="70dac-137">For example, the following can all lead to authorization errors:</span></span>

- <span data-ttu-id="70dac-138">不正确的[访问令牌获取流](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span><span class="sxs-lookup"><span data-stu-id="70dac-138">Incorrect [access token acquisition flows](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span></span>
- <span data-ttu-id="70dac-139">配置不当的[权限范围](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span><span class="sxs-lookup"><span data-stu-id="70dac-139">Poorly configured [permission scopes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span></span>
- <span data-ttu-id="70dac-140">缺乏[许可](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span><span class="sxs-lookup"><span data-stu-id="70dac-140">Lack of [consent](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span></span>

<span data-ttu-id="70dac-141">\**_对 Azure Active Directory 身份验证库 (ADAL) 和 Azure AD Graph API (AAD Graph) 的支持终止_* _</span><span class="sxs-lookup"><span data-stu-id="70dac-141">\**_End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)_* _</span></span>

<span data-ttu-id="70dac-142">_\*自 2020 年 6 月 30 日起，我们将不再向 ADAL 和 Azure AD Graph 添加任何新功能。</span><span class="sxs-lookup"><span data-stu-id="70dac-142">_\*Starting June 30th, 2020\*\*, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="70dac-143">我们将继续提供技术支持和安全更新，但不再提供功能更新。</span><span class="sxs-lookup"><span data-stu-id="70dac-143">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="70dac-144">**从 2022** 年 6 月 30 日开始，我们将停止支持 ADAL 和 Azure AD Graph，并且将不再提供技术支持或安全更新。</span><span class="sxs-lookup"><span data-stu-id="70dac-144">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="70dac-145">在现有的操作系统版本上使用 ADAL 的应用在此时间之后将继续工作，但将不会获得 *任何技术支持或安全更新*。</span><span class="sxs-lookup"><span data-stu-id="70dac-145">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="70dac-146">在此时间之后，使用 Azure AD Graph 的应用可能不再收到来自 Azure AD Graph 终结点的响应。</span><span class="sxs-lookup"><span data-stu-id="70dac-146">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="70dac-147">**ADAL 迁移**</span><span class="sxs-lookup"><span data-stu-id="70dac-147">**ADAL Migration**</span></span>

<span data-ttu-id="70dac-148">我们建议更新到具有最新功能和安全更新的 [Microsoft 身份验证库 (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)。</span><span class="sxs-lookup"><span data-stu-id="70dac-148">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="70dac-149">如果你使用的是 Microsoft 应用，请了解 Microsoft 正在将应用程序迁移到 MSAL（在支持终止截止时间之前）以确保他们将受益于 MSAL 正在进行的安全和功能改进。</span><span class="sxs-lookup"><span data-stu-id="70dac-149">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="70dac-150">请阅读 ADAL 常见问题解答</span><span class="sxs-lookup"><span data-stu-id="70dac-150">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="70dac-151">了解如何在不同平台上迁移应用</span><span class="sxs-lookup"><span data-stu-id="70dac-151">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="70dac-152">如果你需要帮助了解哪些应用使用 ADAL，我们建议你查看所有应用的源代码，如果适用，请联系任何 ISV 或应用提供商。</span><span class="sxs-lookup"><span data-stu-id="70dac-152">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="70dac-153">Microsoft 支持部门也可提供租户内所有非 Microsoft ADAL 应用的列表。</span><span class="sxs-lookup"><span data-stu-id="70dac-153">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="70dac-154">**AAD Graph 迁移**</span><span class="sxs-lookup"><span data-stu-id="70dac-154">**AAD Graph Migration**</span></span>

<span data-ttu-id="70dac-155">对于使用 Azure AD Graph 的应用程序，请按照我们的指南将[Azure AD Graph 应用迁移到 Microsoft Graph。](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)</span><span class="sxs-lookup"><span data-stu-id="70dac-155">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. <span data-ttu-id="70dac-156">[我们的迁移清单提供了入门起点](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)。</span><span class="sxs-lookup"><span data-stu-id="70dac-156">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span>
2. <span data-ttu-id="70dac-157">你的 Azure 应用注册门户显示了哪些应用正在使用 AAD Graph。</span><span class="sxs-lookup"><span data-stu-id="70dac-157">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="70dac-158">我们建议查看应用的全部源代码，并且如果适用，请联系任何 ISV 或应用提供商。</span><span class="sxs-lookup"><span data-stu-id="70dac-158">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="70dac-159">Microsoft 支持还可以提供租户中所有 AAD Graph 使用情况的列表。</span><span class="sxs-lookup"><span data-stu-id="70dac-159">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="70dac-160">若要使你的应用可访问 Microsoft Graph 中的数据，用户或管理员必须通过同意过程向其授予正确的权限。</span><span class="sxs-lookup"><span data-stu-id="70dac-160">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="70dac-161">[Microsoft Graph 权限参考](https://docs.microsoft.com/graph/permissions-reference)列出了与每组主要 Microsoft Graph API 关联的权限。</span><span class="sxs-lookup"><span data-stu-id="70dac-161">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="70dac-162">它还提供有关如何使用权限的指导。</span><span class="sxs-lookup"><span data-stu-id="70dac-162">It also provides guidance about how to use the permissions.</span></span>
