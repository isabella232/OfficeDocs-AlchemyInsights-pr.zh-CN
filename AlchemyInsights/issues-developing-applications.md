---
title: 开发应用程序的问题
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
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950689"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="a0328-102">开发应用程序的问题</span><span class="sxs-lookup"><span data-stu-id="a0328-102">Issues developing applications</span></span>

<span data-ttu-id="a0328-103">若要在构建 Azure Active Directory (AD) 应用时解决最常见问题，请参阅下列文章：</span><span class="sxs-lookup"><span data-stu-id="a0328-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="a0328-104">我仅在使用 Chrome 浏览器登录应用程序时遇到问题</span><span class="sxs-lookup"><span data-stu-id="a0328-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="a0328-105">我不知道如何更改我的应用程序令牌生存期默认值</span><span class="sxs-lookup"><span data-stu-id="a0328-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="a0328-106">我不清楚应用程序许可的工作方式</span><span class="sxs-lookup"><span data-stu-id="a0328-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="a0328-107">我不知道如何向我的应用程序授予权限</span><span class="sxs-lookup"><span data-stu-id="a0328-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="a0328-108">我不了解委派和应用程序权限的区别</span><span class="sxs-lookup"><span data-stu-id="a0328-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="a0328-109">\***对 Azure Active Directory 身份验证库 (ADAL) 和 Azure AD Graph API (AAD Graph) 的支持终止** _</span><span class="sxs-lookup"><span data-stu-id="a0328-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="a0328-110">自 2020 年 6 月 30 日起，我们将不再向 Azure Active Directory 身份验证库 (ADAL) 和 Azure AD Graph API (AAD Graph) 添加任何新功能。</span><span class="sxs-lookup"><span data-stu-id="a0328-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="a0328-111">我们将继续提供技术支持和安全更新，但不再提供功能更新。</span><span class="sxs-lookup"><span data-stu-id="a0328-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="a0328-112">自 2022 年 6 月 30 日起，我们将终止对 ADAL 和 AAD Graph 的支持，并且将不再提供技术支持或安全更新。</span><span class="sxs-lookup"><span data-stu-id="a0328-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="a0328-113">此条件的含义如下所述：</span><span class="sxs-lookup"><span data-stu-id="a0328-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="a0328-114">此时间之后，在现有 OS 版本上使用 ADAL 的应用将继续工作，但将不会获得任何技术支持或安全更新。</span><span class="sxs-lookup"><span data-stu-id="a0328-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="a0328-115">此时间之后，使用 AAD Graph 的应用将不再接收来自 AAD Graph 终结点的响应。</span><span class="sxs-lookup"><span data-stu-id="a0328-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="a0328-116">_ *ADAL 迁移*\*</span><span class="sxs-lookup"><span data-stu-id="a0328-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="a0328-117">如果正在使用 Microsoft 应用，我们建议更新到具有最新功能和安全更新的 Microsoft 身份验证库 (MSAL)。</span><span class="sxs-lookup"><span data-stu-id="a0328-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="a0328-118">此建议是在 Microsoft 启动在支持结束截止日期之前将其应用迁移到 MSAL 的过程背景下提出的。</span><span class="sxs-lookup"><span data-stu-id="a0328-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="a0328-119">Microsoft 将应用迁移到 MSAL 可确保应用从 MSAL 持续的安全与功能改进中受益。</span><span class="sxs-lookup"><span data-stu-id="a0328-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="a0328-120">请阅读 ADAL 常见问题解答</span><span class="sxs-lookup"><span data-stu-id="a0328-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="a0328-121">了解如何在不同平台上迁移应用</span><span class="sxs-lookup"><span data-stu-id="a0328-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="a0328-122">如果在了解哪些应用使用 ADAL 方面需要帮助，我们建议查看应用的全部源代码，如果适用，还请联系任何独立软件供应商 (ISV) 或应用提供商。</span><span class="sxs-lookup"><span data-stu-id="a0328-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="a0328-123">Microsoft 支持部门也可提供租户内所有非 Microsoft ADAL 应用的列表。</span><span class="sxs-lookup"><span data-stu-id="a0328-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="a0328-124">**AAD Graph 迁移**</span><span class="sxs-lookup"><span data-stu-id="a0328-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="a0328-125">对于使用 AAD Graph 的应用程序，请遵循我们关于迁移 AAD Graph 应用到 Microsoft Graph 的指南：</span><span class="sxs-lookup"><span data-stu-id="a0328-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="a0328-126">[我们的迁移清单提供了入门起点](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)。</span><span class="sxs-lookup"><span data-stu-id="a0328-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="a0328-127">你的 Azure 应用注册门户显示了哪些应用正在使用 AAD Graph。</span><span class="sxs-lookup"><span data-stu-id="a0328-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="a0328-128">我们建议查看应用的全部源代码，并且如果适用，请联系任何独立软件销售商 (ISV) 或应用提供商。</span><span class="sxs-lookup"><span data-stu-id="a0328-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="a0328-129">Microsoft 支持部门也可提供租户内 AAD Graph 使用情况的信息。</span><span class="sxs-lookup"><span data-stu-id="a0328-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







