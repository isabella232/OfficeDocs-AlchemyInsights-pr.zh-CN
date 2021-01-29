---
title: 身份验证库问题
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
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2021
ms.locfileid: "50037210"
---
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="84271-102">身份验证库问题</span><span class="sxs-lookup"><span data-stu-id="84271-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="84271-103">[Microsoft 标识平台身份验证库](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) 列出了 Microsoft 支持的兼容客户端和中间件库。</span><span class="sxs-lookup"><span data-stu-id="84271-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="84271-104">Microsoft 身份验证库 (MSAL) [支持多个](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) 身份验证流，以用于不同的应用程序方案。</span><span class="sxs-lookup"><span data-stu-id="84271-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="84271-105">若要进行身份验证和获取令牌，您可以在代码中初始化新的公共或机密客户端应用程序。</span><span class="sxs-lookup"><span data-stu-id="84271-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="84271-106">在 MICROSOFT 身份验证库或 MSAL (中初始化客户端应用时，可以设置) 。</span><span class="sxs-lookup"><span data-stu-id="84271-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="84271-107">若要了解详细信息，请参阅 [应用程序配置选项](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)。</span><span class="sxs-lookup"><span data-stu-id="84271-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="84271-108">**停止支持 Azure Active Directory 身份验证库 (ADAL) 和 Azure AD Graph API (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="84271-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="84271-109">**从 2020** 年 6 月 30 日开始，我们将不再向 ADAL 和 Azure AD Graph 添加任何新功能。</span><span class="sxs-lookup"><span data-stu-id="84271-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="84271-110">我们将继续提供技术支持和安全更新，但不再提供功能更新。</span><span class="sxs-lookup"><span data-stu-id="84271-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="84271-111">**从 2022** 年 6 月 30 日开始，我们将停止对 ADAL 和 Azure AD Graph 的支持，并且将不再提供技术支持或安全更新。</span><span class="sxs-lookup"><span data-stu-id="84271-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="84271-112">在现有的操作系统版本上使用 ADAL 的应用在此时间之后将继续工作，但将不会获得 *任何技术支持或安全更新*。</span><span class="sxs-lookup"><span data-stu-id="84271-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="84271-113">在此时间之后使用 Azure AD Graph 的应用可能不再收到来自 Azure AD Graph 终结点的响应。</span><span class="sxs-lookup"><span data-stu-id="84271-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="84271-114">**ADAL 迁移**</span><span class="sxs-lookup"><span data-stu-id="84271-114">**ADAL Migration**</span></span>

<span data-ttu-id="84271-115">我们建议更新到具有最新功能和安全更新的 [Microsoft 身份验证库 (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)。</span><span class="sxs-lookup"><span data-stu-id="84271-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="84271-116">如果你使用的是 Microsoft 应用，请知道 Microsoft 正在将应用程序迁移到 MSAL，直到支持期限结束，确保他们将受益于 MSAL 正在进行的安全和功能改进。</span><span class="sxs-lookup"><span data-stu-id="84271-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="84271-117">有关详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="84271-117">For more information, see:</span></span>

1. [<span data-ttu-id="84271-118">请阅读 ADAL 常见问题解答</span><span class="sxs-lookup"><span data-stu-id="84271-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="84271-119">了解如何在不同平台上迁移应用</span><span class="sxs-lookup"><span data-stu-id="84271-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="84271-120">如果你需要了解哪些应用使用 ADAL 的帮助，我们建议你查看所有应用的源代码，如果适用，请联系任何 ISV 或应用提供商。</span><span class="sxs-lookup"><span data-stu-id="84271-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="84271-121">Microsoft 支持部门也可提供租户内所有非 Microsoft ADAL 应用的列表。</span><span class="sxs-lookup"><span data-stu-id="84271-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="84271-122">**AAD Graph 迁移**</span><span class="sxs-lookup"><span data-stu-id="84271-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="84271-123">对于使用 Azure AD Graph 的应用程序，请按照我们的指南将[Azure AD Graph 应用迁移到 Microsoft Graph。](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)</span><span class="sxs-lookup"><span data-stu-id="84271-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="84271-124">我们的迁移清单提供了一个入门点。</span><span class="sxs-lookup"><span data-stu-id="84271-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="84271-125">你的 Azure 应用注册门户显示了哪些应用正在使用 AAD Graph。</span><span class="sxs-lookup"><span data-stu-id="84271-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="84271-126">我们建议查看应用的全部源代码，并且如果适用，请联系任何 ISV 或应用提供商。</span><span class="sxs-lookup"><span data-stu-id="84271-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="84271-127">Microsoft 支持还可以提供租户中所有 AAD Graph 使用情况的列表。</span><span class="sxs-lookup"><span data-stu-id="84271-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="84271-128">若要使你的应用可访问 Microsoft Graph 中的数据，用户或管理员必须通过同意过程向其授予正确的权限。</span><span class="sxs-lookup"><span data-stu-id="84271-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="84271-129">[Microsoft Graph 权限参考](https://docs.microsoft.com/graph/permissions-reference)列出了与每组主要 Microsoft Graph API 关联的权限。</span><span class="sxs-lookup"><span data-stu-id="84271-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="84271-130">它还提供有关如何使用权限的指导。</span><span class="sxs-lookup"><span data-stu-id="84271-130">It also provides guidance about how to use the permissions.</span></span>
