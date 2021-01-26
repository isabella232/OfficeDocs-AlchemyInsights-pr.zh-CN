---
title: 身份验证问题
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: 2f413e863e6aa23548e425de5901f8158e1d48ab
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976839"
---
# <a name="authentication-issues"></a><span data-ttu-id="9a5b7-102">身份验证问题</span><span class="sxs-lookup"><span data-stu-id="9a5b7-102">Authentication issues</span></span>

<span data-ttu-id="9a5b7-103">**查找关于从 Azure Active Directory (Azure AD) 安全令牌服务 (STS) 返回的 AADSTS 错误代码的信息？**</span><span class="sxs-lookup"><span data-stu-id="9a5b7-103">**Looking for information about the AADSTS error codes that are returned from the Azure Active Directory (Azure AD) security token service (STS)?**</span></span> <span data-ttu-id="9a5b7-104">请参阅 [Azure AD 身份验证和授权错误代码](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 以查找 AADSTS 错误说明、修复和一些建议的解决方法。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-104">See [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>

<span data-ttu-id="9a5b7-105">授权错误可能是由多个不同的问题造成的，其中大多数问题会产生 401 或 403 错误。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-105">Authorization errors can be a result of several different issues, most of which generate a 401 or 403 error.</span></span> <span data-ttu-id="9a5b7-106">例如，以下问题可能会导致授权错误：</span><span class="sxs-lookup"><span data-stu-id="9a5b7-106">For example, the following issues can all lead to authorization errors:</span></span>

- <span data-ttu-id="9a5b7-107">不正确的[访问令牌获取流](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization)</span><span class="sxs-lookup"><span data-stu-id="9a5b7-107">Incorrect [access token acquisition flows](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization)</span></span> 
- <span data-ttu-id="9a5b7-108">配置不当的[权限范围](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)</span><span class="sxs-lookup"><span data-stu-id="9a5b7-108">Poorly configured [permission scopes](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)</span></span> 
- <span data-ttu-id="9a5b7-109">缺乏[许可](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)</span><span class="sxs-lookup"><span data-stu-id="9a5b7-109">Lack of [consent](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)</span></span>

<span data-ttu-id="9a5b7-110">若要解决常见授权错误，请尝试执行以下与你遇到的错误最接近的步骤。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-110">To resolve common authorization errors, try the steps provided below which most closely match the error you are receiving.</span></span> <span data-ttu-id="9a5b7-111">可能有多个步骤适用于你所遇到的某个错误。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-111">More than one step may apply for an error you are receiving.</span></span>

<span data-ttu-id="9a5b7-112">**401 未授权错误：你的令牌是否有效？**</span><span class="sxs-lookup"><span data-stu-id="9a5b7-112">**401 Unauthorized error: Is your token valid?**</span></span>

<span data-ttu-id="9a5b7-113">请确保应用在请求中向 Microsoft Graph 提供有效的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-113">Ensure that your app is presenting a valid access token to Microsoft Graph as part of the request.</span></span> <span data-ttu-id="9a5b7-114">此错误通常意味着 HTTP 身份验证请求标头中缺少访问令牌，或者令牌无效或已过期。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-114">This error often means that the access token may be missing in the HTTP authenticate request header or that the token is invalid or has expired.</span></span> <span data-ttu-id="9a5b7-115">强烈建议使用 Microsoft 身份验证库 (MSAL) 获取访问令牌。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-115">We strongly recommend that you use the Microsoft Authentication Library (MSAL) for access token acquisition.</span></span> <span data-ttu-id="9a5b7-116">此外，如果尝试使用授予个人 Microsoft 帐户的委派访问令牌来访问仅支持工作或学校帐户（组织帐户）的 API，也可能会发生此错误。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-116">Additionally, this error may occur if you try to use a delegated access token granted to a personal Microsoft account to access an API that only supports work or school accounts (organizational accounts).</span></span>

<span data-ttu-id="9a5b7-117">**403 禁止错误：你是否选择了正确的权限集？**</span><span class="sxs-lookup"><span data-stu-id="9a5b7-117">**403 Forbidden error: Have you chosen the right set of permissions?**</span></span>

<span data-ttu-id="9a5b7-118">确保根据应用调用的 Microsoft Graph API 来请求正确的权限集。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-118">Ensure that you have requested the correct set of permissions based on the Microsoft Graph APIs your app calls.</span></span> <span data-ttu-id="9a5b7-119">所有 Microsoft Graph API 参考方法主题中都提供了我们建议的最低特权权限。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-119">Recommended least-privileged permissions are provided in all the Microsoft Graph API reference method topics.</span></span> <span data-ttu-id="9a5b7-120">此外，这些权限必须由用户或管理员向应用程序授予。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-120">Additionally, those permissions must be granted to the application by a user or an administrator.</span></span> <span data-ttu-id="9a5b7-121">授予权限通常通过同意页面进行，也可使用 Azure 门户应用程序注册边栏选项卡授予进行。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-121">Granting permissions normally happens through a consent page or usage of the Azure Portal application registration blade.</span></span> <span data-ttu-id="9a5b7-122">从应用程序的“**设置**”边栏选项卡，单击“**所需权限**”，然后单击“**授予权限**”。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-122">From the **Settings** blade for the application, click **Required Permissions**, and then click **Grant Permissions**.</span></span> <span data-ttu-id="9a5b7-123">有关详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="9a5b7-123">For more information, see:</span></span>

- [<span data-ttu-id="9a5b7-124">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="9a5b7-124">Microsoft Graph permissions</span></span>](https://docs.microsoft.com/graph/permissions-reference) 
- [<span data-ttu-id="9a5b7-125">了解 Azure AD 权限和许可</span><span class="sxs-lookup"><span data-stu-id="9a5b7-125">Understanding Azure AD permissions and consent</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

<span data-ttu-id="9a5b7-126">**403 禁止错误：你的应用是否获取了与所选权限匹配的令牌？**</span><span class="sxs-lookup"><span data-stu-id="9a5b7-126">**403 Forbidden error: Did your app acquire a token to match chosen permissions?**</span></span>

<span data-ttu-id="9a5b7-127">确保请求或授予的权限类型与应用获取的访问令牌类型相匹配。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-127">Ensure that the types of permissions requested or granted match the type of access token that your app acquires.</span></span> <span data-ttu-id="9a5b7-128">你可能正在请求和授予应用权限，但使用的是委派交互式代码流令牌，而不是客户端凭据流令牌，或者正在请求和授予委派权限，但使用的是客户端凭据流令牌，而不是委派代码流令牌。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-128">You might be requesting and granting app permissions but using delegated interactive code flow tokens instead of client credential flow tokens, or requesting and granting delegated permissions but using client credential flow tokens instead of delegated code flow tokens.</span></span>

<span data-ttu-id="9a5b7-129">有关于获取令牌相关的详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="9a5b7-129">For more information related to acquiring tokens, see:</span></span>

- [<span data-ttu-id="9a5b7-130">代表用户获取访问权限和委派权限</span><span class="sxs-lookup"><span data-stu-id="9a5b7-130">Get access on behalf of users and delegated permissions</span></span>](https://docs.microsoft.com/graph/auth-v2-user) 
- [<span data-ttu-id="9a5b7-131">Azure AD v2.0 - OAuth 2.0 授权代码流</span><span class="sxs-lookup"><span data-stu-id="9a5b7-131">Azure AD v2.0 - OAuth 2.0 authorization code flow</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [<span data-ttu-id="9a5b7-132">在没有用户的情况下获取访问权限（守护程序服务）和应用程序权限</span><span class="sxs-lookup"><span data-stu-id="9a5b7-132">Get access without a user (daemon service) and application permissions</span></span>](https://docs.microsoft.com/graph/auth-v2-service) 
- [<span data-ttu-id="9a5b7-133">Azure AD v2.0 - OAuth 2.0 客户端凭据流</span><span class="sxs-lookup"><span data-stu-id="9a5b7-133">Azure AD v2.0 - OAuth 2.0 client credentials flow</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

<span data-ttu-id="9a5b7-134">**403 禁止访问错误：重置密码**</span><span class="sxs-lookup"><span data-stu-id="9a5b7-134">**403 Forbidden error: Resetting password**</span></span>

<span data-ttu-id="9a5b7-135">目前，没有应用程序权限守护程序服务到服务权限允许重置用户密码。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-135">Currently, there are no application permission daemon service-to-service permissions that allow resetting user passwords.</span></span> <span data-ttu-id="9a5b7-136">这些 API 仅支持对登录的管理员使用交互式委派代码流。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-136">These APIs are only supported using the interactive delegated code flows with a signed-in administrator.</span></span> <span data-ttu-id="9a5b7-137">有关详细信息，请参阅 [Microsoft Graph 权限](https://docs.microsoft.com/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-137">For more information, see [Microsoft Graph permissions](https://docs.microsoft.com/graph/permissions-reference).</span></span>

<span data-ttu-id="9a5b7-138">**403 禁止：用户是否具有访问权限，是否获得许可？**</span><span class="sxs-lookup"><span data-stu-id="9a5b7-138">**403 Forbidden: Does the user have access and are they licensed?**</span></span>

<span data-ttu-id="9a5b7-139">对于委派代码流，Microsoft Graph 将根据向应用授予的权限以及登录用户具有的权限来评估是否允许请求。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-139">For delegated code flows, Microsoft Graph evaluates whether the request has been allowed based on the permissions granted to the app and the permissions that the signed-in user has.</span></span> <span data-ttu-id="9a5b7-140">通常，此错误表示用户没有足够的特权执行请求 **或者** 用户没有获得所访问数据的许可。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-140">Generally, this error indicates that the user is not privileged enough to perform the request **or** the user is not licensed for the data being accessed.</span></span> <span data-ttu-id="9a5b7-141">只有具有所需权限或许可证的用户才能成功发出请求。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-141">Only users with the required permissions or licenses can make the request successfully.</span></span>

<span data-ttu-id="9a5b7-142">**403 禁止：是否选择了正确的资源 API？**</span><span class="sxs-lookup"><span data-stu-id="9a5b7-142">**403 Forbidden: Did you select the correct resource API?**</span></span>

<span data-ttu-id="9a5b7-143">API 服务（如 Microsoft Graph）检查接收的访问令牌中的 *aud* 声明 (audience) 是否与其本身的预期值匹配，如果不匹配，则会出现 403 禁止错误。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-143">API services like Microsoft Graph check that the *aud* claim (audience) in the received access token matches the value it expects for itself, and if not, a 403 Forbidden error occurs.</span></span> <span data-ttu-id="9a5b7-144">导致此错误的常见错误是尝试使用为 Azure AD Graph API、Outlook API 或 SharePoint/OneDrive API 获取的令牌调用 Microsoft Graph（或反之）。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-144">A common mistake resulting in this error is trying to use a token acquired for Azure AD Graph APIs, Outlook APIs, or SharePoint/OneDrive APIs to call Microsoft Graph (or vice versa).</span></span> <span data-ttu-id="9a5b7-145">确保你的应用为其获取令牌的资源（或范围）与应用调用的 API 匹配。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-145">Ensure that the resource (or scope) your app is acquiring a token for matches the API that the app is calling.</span></span>

<span data-ttu-id="9a5b7-146">**400 错误请求或 403 禁止：用户是否符合其组织的条件访问 (CA) 策略？**</span><span class="sxs-lookup"><span data-stu-id="9a5b7-146">**400 Bad Request or 403 Forbidden: Does the user comply with their organization's conditional access (CA) policies?**</span></span>

<span data-ttu-id="9a5b7-147">根据组织的条件访问 (CA) 策略，通过你的应用访问 Microsoft Graph 资源的用户可能会被要求提供附加信息，而这些信息在应用最初获取的访问令牌中并不存在。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-147">Based on an organization's conditional access (CA) policies, a user accessing Microsoft Graph resources via your app may be challenged for additional information that is not present in the access token your app originally acquired.</span></span> <span data-ttu-id="9a5b7-148">在这种情况下，你的应用在获取访问令牌期间会收到 **400 以及 *interaction_required*** 错误，或者在调用 Microsoft Graph 时收到 **403 以及 *insufficient_claims*** 错误。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-148">In this case, your app receives a **400 with an *interaction_required*** error during access token acquisition or a **403 with *insufficient_claims*** error when calling Microsoft Graph.</span></span> <span data-ttu-id="9a5b7-149">在这两种情况下，错误响应都包含可呈现给授权终结点的附加信息，以便要求用户提供其他信息（如多重身份验证或设备注册）。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-149">In both cases, the error response contains additional information that can be presented to the authorized endpoint to challenge the user for additional information (like multi-factor authentication or device enrollment).</span></span>

<span data-ttu-id="9a5b7-150">有关条件访问相关的详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="9a5b7-150">For more information related to conditional access, see:</span></span>

- [<span data-ttu-id="9a5b7-151">使用 MSAL 处理条件访问质询</span><span class="sxs-lookup"><span data-stu-id="9a5b7-151">Handling conditional access challenges using MSAL</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [<span data-ttu-id="9a5b7-152">Azure Active Directory 条件访问开发人员指南</span><span class="sxs-lookup"><span data-stu-id="9a5b7-152">Developer guidance for Azure Active Directory conditional access</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

<span data-ttu-id="9a5b7-153">\**_对 Azure Active Directory 身份验证库 (ADAL) 和 Azure AD Graph API (AAD Graph) 的支持终止_* _</span><span class="sxs-lookup"><span data-stu-id="9a5b7-153">\**_End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)_* _</span></span>

- <span data-ttu-id="9a5b7-154">自 2020 年 6 月 30 日起，我们将不再向 Azure Active Directory 身份验证库 (ADAL) 和 Azure AD Graph API (AAD Graph) 添加任何新功能。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-154">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="9a5b7-155">我们将继续提供技术支持和安全更新，但不再提供功能更新。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-155">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="9a5b7-156">自 2022 年 6 月 30 日起，我们将终止对 ADAL 和 Azure AD Graph 的支持，并且将不再提供技术支持或安全更新。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-156">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span>
    - <span data-ttu-id="9a5b7-157">此时间之后，在现有 OS 版本上使用 ADAL 的应用将继续工作，但将不会获得任何技术支持或安全更新。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-157">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>
    - <span data-ttu-id="9a5b7-158">此时间之后，使用 Azure AD Graph 的应用将不再接收来自 AAD Graph 终结点的响应。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-158">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint.</span></span>

<span data-ttu-id="9a5b7-159">_ *ADAL 迁移*\*</span><span class="sxs-lookup"><span data-stu-id="9a5b7-159">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="9a5b7-160">我们建议更新到具有最新功能和安全更新的 [Microsoft 身份验证库 (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-160">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span> <span data-ttu-id="9a5b7-161">此建议是在 Microsoft 在支持结束截止期限之前将其应用程序迁移到 MSAL 的背景下提出的。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-161">This recommendation is in the context of Microsoft migrating its applications to MSAL by the end-of-support deadline.</span></span> <span data-ttu-id="9a5b7-162">Microsoft 应用向 MSAL 迁移的目标时确保应用能够从 MSAL 的持续安全和功能改进中获益。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-162">The objective of Microsoft apps' migration to MSAL is to ensure that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

- [<span data-ttu-id="9a5b7-163">请阅读 ADAL 常见问题解答</span><span class="sxs-lookup"><span data-stu-id="9a5b7-163">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [<span data-ttu-id="9a5b7-164">了解在不同平台上如何迁移应用</span><span class="sxs-lookup"><span data-stu-id="9a5b7-164">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- <span data-ttu-id="9a5b7-165">如果在了解哪些应用使用 ADAL 方面需要帮助，我们建议查看应用的全部源代码，如果适用，还请联系任何独立软件供应商 (ISV) 或应用提供商。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-165">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="9a5b7-166">Microsoft 支持部门也可提供租户内所有非 Microsoft ADAL 应用的列表。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-166">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="9a5b7-167">**AAD Graph 迁移**</span><span class="sxs-lookup"><span data-stu-id="9a5b7-167">**AAD Graph Migration**</span></span>

<span data-ttu-id="9a5b7-168">对于使用 AAD Graph 的应用程序，请按照我们关于 [迁移 Azure AD Graph 应用到 Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true) 的指南操作。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-168">For applications that are using AAD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).</span></span>

- <span data-ttu-id="9a5b7-169">[我们的迁移清单提供了入门起点](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-169">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
- <span data-ttu-id="9a5b7-170">你的 Azure 应用注册门户显示了哪些应用正在使用 AAD Graph。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-170">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="9a5b7-171">我们建议查看应用的全部源代码，并且如果适用，请联系任何 ISV 或应用提供商。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-171">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="9a5b7-172">Microsoft 支持部门也可提供租户内所有 AAD Graph 使用情况的信息。</span><span class="sxs-lookup"><span data-stu-id="9a5b7-172">Microsoft support can also provide you the information of all AAD Graph usage in your tenant.</span></span>

 










