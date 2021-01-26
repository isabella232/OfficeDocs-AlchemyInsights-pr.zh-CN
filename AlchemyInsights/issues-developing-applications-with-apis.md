---
title: 使用 API 开发应用程序时的问题
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
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/25/2021
ms.locfileid: "49951874"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="ae8c3-102">使用 API 开发应用程序时的问题</span><span class="sxs-lookup"><span data-stu-id="ae8c3-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="ae8c3-103">若要开始使用 Azure Active Directory Graph API，请参阅 [Azure AD Graph API 快速入门指南](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) ，或查看 [交互式 Azure AD Graph API 参考文档](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)。</span><span class="sxs-lookup"><span data-stu-id="ae8c3-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="ae8c3-104">**停止支持 Azure Active Directory 身份验证库 (ADAL) 和 Azure AD Graph API (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="ae8c3-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="ae8c3-105">**从 2020** 年 6 月 30 日开始，我们将不再向 ADAL 和 Azure AD Graph 添加任何新功能。</span><span class="sxs-lookup"><span data-stu-id="ae8c3-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="ae8c3-106">我们将继续提供技术支持和安全更新，但将不再提供功能更新。</span><span class="sxs-lookup"><span data-stu-id="ae8c3-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="ae8c3-107">**从 2022** 年 6 月 30 日开始，我们将停止对 ADAL 和 Azure AD Graph 的支持，并且将不再提供技术支持或安全更新。</span><span class="sxs-lookup"><span data-stu-id="ae8c3-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="ae8c3-108">在现有的操作系统版本上使用 ADAL 的应用在此时间之后将继续工作，但将不会获得任何技术支持或安全更新。</span><span class="sxs-lookup"><span data-stu-id="ae8c3-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="ae8c3-109">在此时间之后使用 Azure AD Graph 的应用可能不再收到来自 Azure AD Graph 终结点的响应。</span><span class="sxs-lookup"><span data-stu-id="ae8c3-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="ae8c3-110">**ADAL 迁移**</span><span class="sxs-lookup"><span data-stu-id="ae8c3-110">**ADAL Migration**</span></span>

<span data-ttu-id="ae8c3-111">我们建议更新到 [具有最新功能和安全更新 (MSAL) ](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)Microsoft 身份验证库。</span><span class="sxs-lookup"><span data-stu-id="ae8c3-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="ae8c3-112">如果你使用的是 Microsoft 应用，请知道 Microsoft 正在将应用程序迁移到 MSAL（在支持终止截止时间之前）以确保他们将受益于 MSAL 正在进行的安全和功能改进。</span><span class="sxs-lookup"><span data-stu-id="ae8c3-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="ae8c3-113">[阅读 ADAL 常见问题解答](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)。</span><span class="sxs-lookup"><span data-stu-id="ae8c3-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="ae8c3-114">[了解如何基于每个平台迁移应用](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)。</span><span class="sxs-lookup"><span data-stu-id="ae8c3-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="ae8c3-115">如果你需要了解哪些应用使用 ADAL 的帮助，我们建议你查看所有应用的源代码，如果适用，请联系任何 ISV 或应用提供商。</span><span class="sxs-lookup"><span data-stu-id="ae8c3-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="ae8c3-116">Microsoft 支持还可以提供租户中所有非 Microsoft ADAL 应用的列表。</span><span class="sxs-lookup"><span data-stu-id="ae8c3-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="ae8c3-117">**AAD Graph 迁移**</span><span class="sxs-lookup"><span data-stu-id="ae8c3-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="ae8c3-118">对于使用 Azure AD Graph 的应用程序，请按照我们的指南将[Azure AD Graph 应用迁移到 Microsoft Graph。](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="ae8c3-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="ae8c3-119">[我们的迁移清单提供了一个入门点](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)。</span><span class="sxs-lookup"><span data-stu-id="ae8c3-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="ae8c3-120">Azure 应用注册门户显示哪些应用程序正在使用 AAD Graph。</span><span class="sxs-lookup"><span data-stu-id="ae8c3-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="ae8c3-121">我们建议你查看所有应用的源代码，如果适用，请联系任何 ISV 或应用提供商。</span><span class="sxs-lookup"><span data-stu-id="ae8c3-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="ae8c3-122">Microsoft 支持还可以提供租户中所有 AAD Graph 使用情况的列表。</span><span class="sxs-lookup"><span data-stu-id="ae8c3-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="ae8c3-123">若要使你的应用可访问 Microsoft Graph 中的数据，用户或管理员必须通过同意过程向其授予正确的权限。</span><span class="sxs-lookup"><span data-stu-id="ae8c3-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="ae8c3-124">[Microsoft Graph 权限参考](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true)列出了与每组主要 Microsoft Graph API 关联的权限。</span><span class="sxs-lookup"><span data-stu-id="ae8c3-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="ae8c3-125">它还提供有关如何使用权限的指导。</span><span class="sxs-lookup"><span data-stu-id="ae8c3-125">It also provides guidance about how to use the permissions.</span></span>
