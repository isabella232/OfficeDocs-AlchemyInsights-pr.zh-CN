---
title: 应用程序错误
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976881"
---
# <a name="application-errors"></a><span data-ttu-id="e044e-102">应用程序错误</span><span class="sxs-lookup"><span data-stu-id="e044e-102">Application errors</span></span>

<span data-ttu-id="e044e-103">要查找有关从 Azure Active Directory (Azure AD) STS (返回的 **AADSTS** 错误代码) ？</span><span class="sxs-lookup"><span data-stu-id="e044e-103">Looking for info about the **AADSTS error codes** that are returned from the Azure Active Directory (Azure AD) security token service (STS)?</span></span> <span data-ttu-id="e044e-104">阅读 [Azure AD 身份验证和授权错误代码](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) ，查找 AADSTS 错误说明、修补程序和一些建议解决方法。</span><span class="sxs-lookup"><span data-stu-id="e044e-104">Read [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>

<span data-ttu-id="e044e-105">授权错误可能是多个不同问题的结果，大多数问题都会生成 401 或 403 错误。</span><span class="sxs-lookup"><span data-stu-id="e044e-105">Authorization errors can be a result of several different issues, most of which generate a 401 or 403 error.</span></span> <span data-ttu-id="e044e-106">例如，以下情况可能会导致授权错误：</span><span class="sxs-lookup"><span data-stu-id="e044e-106">For example, the following can all lead to authorization errors:</span></span>

- <span data-ttu-id="e044e-107">不正确的[访问令牌获取流](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes)</span><span class="sxs-lookup"><span data-stu-id="e044e-107">Incorrect [access token acquisition flows](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes)</span></span> 
- <span data-ttu-id="e044e-108">配置不当的[权限范围](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span><span class="sxs-lookup"><span data-stu-id="e044e-108">Poorly configured [permission scopes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span></span> 
- <span data-ttu-id="e044e-109">缺乏[许可](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span><span class="sxs-lookup"><span data-stu-id="e044e-109">Lack of [consent](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span></span>

<span data-ttu-id="e044e-110">若要解决常见的授权错误，请尝试下面提供的步骤，这些步骤与您收到的错误最匹配。</span><span class="sxs-lookup"><span data-stu-id="e044e-110">To resolve common authorization errors, try the steps provided below that most closely matches the error you are receiving.</span></span> <span data-ttu-id="e044e-111">多个可能适用。</span><span class="sxs-lookup"><span data-stu-id="e044e-111">More than one may apply.</span></span>

<span data-ttu-id="e044e-112">**401 未授权错误：你的令牌是否有效？**</span><span class="sxs-lookup"><span data-stu-id="e044e-112">**401 Unauthorized error: Is your token valid?**</span></span>

<span data-ttu-id="e044e-113">确保应用程序在请求中向 Microsoft Graph 提供有效的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="e044e-113">Ensure that your application is presenting a valid access token to Microsoft Graph as part of the request.</span></span> <span data-ttu-id="e044e-114">此错误通常意味着 HTTP 身份验证请求标头中缺少访问令牌，或者令牌无效或已过期。</span><span class="sxs-lookup"><span data-stu-id="e044e-114">This error often means that the access token may be missing in the HTTP authenticate request header or that the token is invalid or has expired.</span></span> <span data-ttu-id="e044e-115">强烈建议使用 [Microsoft 身份验证库 (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) 获取访问令牌。</span><span class="sxs-lookup"><span data-stu-id="e044e-115">We strongly recommend that you use the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) for access token acquisition.</span></span> <span data-ttu-id="e044e-116">此外，如果你尝试使用授予个人 Microsoft 帐户的委派访问令牌访问仅支持工作或学校帐户的 API， (组织帐户) 。</span><span class="sxs-lookup"><span data-stu-id="e044e-116">Additionally this error may occur if you try to use a delegated access token granted to a personal Microsoft account to access an API that only supports work or school accounts (organizational accounts).</span></span>

<span data-ttu-id="e044e-117">**403 禁止错误：你是否选择了正确的权限集？**</span><span class="sxs-lookup"><span data-stu-id="e044e-117">**403 Forbidden error: Have you chosen the right set of permissions?**</span></span>

<span data-ttu-id="e044e-118">检查你已基于应用调用的 Microsoft Graph API 请求了正确的权限集。</span><span class="sxs-lookup"><span data-stu-id="e044e-118">Check that you have requested the correct set of permissions based on the Microsoft Graph APIs your app calls.</span></span> <span data-ttu-id="e044e-119">建议最小特权权限在所有 Microsoft Graph API 参考方法主题中提供。</span><span class="sxs-lookup"><span data-stu-id="e044e-119">Recommended least privileged permissions are provided in all the Microsoft Graph API reference method topics.</span></span> <span data-ttu-id="e044e-120">此外，这些权限必须由用户或管理员向应用程序授予。</span><span class="sxs-lookup"><span data-stu-id="e044e-120">Additionally, those permissions must be granted to the application by a user or an administrator.</span></span> <span data-ttu-id="e044e-121">授予权限通常通过同意页进行，也可使用 Azure 门户应用程序注册边栏选项卡授予权限。</span><span class="sxs-lookup"><span data-stu-id="e044e-121">Granting permissions normally happens through a consent page or by granting permissions using the Azure Portal application registration blade.</span></span> <span data-ttu-id="e044e-122">从应用程序的“**设置**”边栏选项卡，单击“**所需权限**”，然后单击“**授予权限**”。</span><span class="sxs-lookup"><span data-stu-id="e044e-122">From the **Settings** blade for the application, click **Required Permissions**, and then click **Grant Permissions**.</span></span>

- [<span data-ttu-id="e044e-123">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="e044e-123">Microsoft Graph permissions</span></span>](https://docs.microsoft.com/graph/permissions-reference) 
- [<span data-ttu-id="e044e-124">了解 Azure AD 权限和许可</span><span class="sxs-lookup"><span data-stu-id="e044e-124">Understanding Azure AD permissions and consent</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

<span data-ttu-id="e044e-125">**403 禁止错误：你的应用是否获取了与所选权限匹配的令牌？**</span><span class="sxs-lookup"><span data-stu-id="e044e-125">**403 Forbidden error: Did your app acquire a token to match chosen permissions?**</span></span>

<span data-ttu-id="e044e-126">确保请求或授予的权限类型与你的应用获取的访问令牌类型相匹配。</span><span class="sxs-lookup"><span data-stu-id="e044e-126">Make sure that the type of permissions requested or granted matches the type of access token that your app acquires.</span></span> <span data-ttu-id="e044e-127">你可能正在请求和授予应用程序权限，但使用的是委派的交互式代码流令牌而不是客户端凭据流令牌，或者正在请求和授予委派权限，但使用的是客户端凭据流令牌而不是委派的代码流令牌。</span><span class="sxs-lookup"><span data-stu-id="e044e-127">You might be requesting and granting application permissions but using delegated interactive code flow tokens instead of client credential flow tokens, or requesting and granting delegated permissions but using client credential flow tokens instead of delegated code flow tokens.</span></span>

- [<span data-ttu-id="e044e-128">代表用户获取访问权限和委派权限</span><span class="sxs-lookup"><span data-stu-id="e044e-128">Get access on behalf of users and delegated permissions</span></span>](https://docs.microsoft.com/graph/auth_v2_user) 
- [<span data-ttu-id="e044e-129">Azure AD v2.0 - OAuth 2.0 授权代码流</span><span class="sxs-lookup"><span data-stu-id="e044e-129">Azure AD v2.0 - OAuth 2.0 authorization code flow</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [<span data-ttu-id="e044e-130">在没有用户的情况下获取访问权限（守护程序服务）和应用程序权限</span><span class="sxs-lookup"><span data-stu-id="e044e-130">Get access without a user (daemon service) and application permissions</span></span>](https://docs.microsoft.com/graph/auth_v2_service) 
- [<span data-ttu-id="e044e-131">Azure AD v2.0 - OAuth 2.0 客户端凭据流</span><span class="sxs-lookup"><span data-stu-id="e044e-131">Azure AD v2.0 - OAuth 2.0 client credentials flow</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

<span data-ttu-id="e044e-132">**403 禁止访问错误：重置密码**</span><span class="sxs-lookup"><span data-stu-id="e044e-132">**403 Forbidden error: Resetting password**</span></span>

<span data-ttu-id="e044e-133">目前，没有应用程序权限守护程序服务到服务权限允许重置用户密码。</span><span class="sxs-lookup"><span data-stu-id="e044e-133">Currently, there are no application permission daemon service-to-service permissions that allow resetting user passwords.</span></span> <span data-ttu-id="e044e-134">这些 API 仅支持对登录的管理员使用交互式委派代码流。</span><span class="sxs-lookup"><span data-stu-id="e044e-134">These APIs are only supported using the interactive delegated code flows with a signed-in administrator.</span></span>

- [<span data-ttu-id="e044e-135">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="e044e-135">Microsoft Graph permissions</span></span>](https://docs.microsoft.com/graph/permissions-reference)

<span data-ttu-id="e044e-136">**403 禁止：用户是否具有访问权限，是否获得许可？**</span><span class="sxs-lookup"><span data-stu-id="e044e-136">**403 Forbidden: Does the user have access and are they licensed?**</span></span>

<span data-ttu-id="e044e-137">对于委派代码流，Microsoft Graph 根据授予应用的权限和登录用户具有的权限评估是否允许请求。</span><span class="sxs-lookup"><span data-stu-id="e044e-137">For delegated code flows, Microsoft Graph evaluates if the request is allowed based on the permissions granted to the app and the permissions that the signed-in user has.</span></span> <span data-ttu-id="e044e-138">通常，此错误表示用户没有足够的特权执行请求或者用户没有获得所访问数据的许可。</span><span class="sxs-lookup"><span data-stu-id="e044e-138">Generally, this error indicates that the user is not privileged enough to perform the request or the user is not licensed for the data being accessed.</span></span> <span data-ttu-id="e044e-139">只有具有所需权限或许可证的用户才能成功发出请求。</span><span class="sxs-lookup"><span data-stu-id="e044e-139">Only users with the required permissions or licenses can make the request successfully.</span></span>

<span data-ttu-id="e044e-140">**403 禁止：是否选择了正确的资源 API？**</span><span class="sxs-lookup"><span data-stu-id="e044e-140">**403 Forbidden: Did you select the correct resource API?**</span></span>

<span data-ttu-id="e044e-141">Microsoft Graph 等 API 服务检查收到的访问令牌中的 aud (受众) 是否与它本身期望的值匹配，如果未匹配，则会导致 403 禁止错误。</span><span class="sxs-lookup"><span data-stu-id="e044e-141">API services like Microsoft Graph check that the aud claim (audience) in the received access token matches the value it expects for itself, and if not, it results in a 403 Forbidden error.</span></span> <span data-ttu-id="e044e-142">导致此错误的常见错误是尝试使用为 Azure AD Graph API、Outlook API 或 SharePoint/OneDrive API 获取的令牌调用 Microsoft Graph (，反之亦然) 。</span><span class="sxs-lookup"><span data-stu-id="e044e-142">A common mistake resulting in this error is trying to use a token acquired for Azure AD Graph APIs, Outlook APIs, or SharePoint/OneDrive APIs to call Microsoft Graph (or vice versa).</span></span> <span data-ttu-id="e044e-143">确保你的应用为其获取令牌的资源（或范围）与应用调用的 API 匹配。</span><span class="sxs-lookup"><span data-stu-id="e044e-143">Ensure that the resource (or scope) your app is acquiring a token for matches the API that the app is calling.</span></span>

<span data-ttu-id="e044e-144">**400 错误请求或 403 禁止：用户是否符合其组织的条件访问 (CA) 策略？**</span><span class="sxs-lookup"><span data-stu-id="e044e-144">**400 Bad Request or 403 Forbidden: Does the user comply with their organization's conditional access (CA) policies?**</span></span>

<span data-ttu-id="e044e-145">根据组织的 CA 策略，可能要求用户通过你的应用访问 Microsoft Graph 资源，获取你的应用最初获取的访问令牌中不存在的其他信息。</span><span class="sxs-lookup"><span data-stu-id="e044e-145">Based on an organization's CA policies, a user accessing Microsoft Graph resources via your app may be challenged for additional information that is not present in the access token your app originally acquired.</span></span> <span data-ttu-id="e044e-146">在这种情况下，你的应用在获取访问令牌期间会收到 400 以及 *interaction_required* 错误，或者在调用 Microsoft Graph 时收到 403 以及 *insufficient_claims* 错误。</span><span class="sxs-lookup"><span data-stu-id="e044e-146">In this case, your app receives a 400 with an *interaction_required* error during access token acquisition or a 403 with *insufficient_claims* error when calling Microsoft Graph.</span></span> <span data-ttu-id="e044e-147">在这两种情况下，错误响应都包含可呈现给授权终结点的附加信息，以便向用户质询其他信息（如多重身份验证或设备注册）。</span><span class="sxs-lookup"><span data-stu-id="e044e-147">In both cases, the error response contains additional information that can be presented to the authorize endpoint to challenge the user for additional information (like multi-factor authentication or device enrollment).</span></span>

- [<span data-ttu-id="e044e-148">使用 MSAL 处理条件访问挑战 </span><span class="sxs-lookup"><span data-stu-id="e044e-148">Handling conditional access challenges using MSAL </span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [<span data-ttu-id="e044e-149">Azure Active Directory 条件访问开发人员指南</span><span class="sxs-lookup"><span data-stu-id="e044e-149">Developer guidance for Azure Active Directory conditional access</span></span>](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)