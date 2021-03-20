---
title: 使用身份验证库
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897428"
---
# <a name="working-with-authentication-libraries"></a><span data-ttu-id="baa90-102">使用身份验证库</span><span class="sxs-lookup"><span data-stu-id="baa90-102">Working with Authentication Libraries</span></span>

<span data-ttu-id="baa90-103">如果要解决 Microsoft 身份验证库 (MSAL) 问题，请执行以下建议步骤:</span><span class="sxs-lookup"><span data-stu-id="baa90-103">To resolve Microsoft Authentication Library (MSAL) issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="baa90-104">**使用 MSAL**: [Microsoft 标识平台身份验证库](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - 本文介绍了 Microsoft.认证库对几种应用类型的支持。</span><span class="sxs-lookup"><span data-stu-id="baa90-104">**Working with MSAL**: [Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - This article shows Microsoft Authentication Library support for several application types.</span></span> <span data-ttu-id="baa90-105">它包括指向库源代码的链接、从哪里获取应用项目的程序包、以及库是否支持用户登录(身份验证)、访问受保护的 Web API (授权)，或者两者都支持。</span><span class="sxs-lookup"><span data-stu-id="baa90-105">It includes links to library source code; where to get the package for your app's project; and whether the library supports user sign-in (authentication), access to protected web APIs (authorization), or both.</span></span>

2. <span data-ttu-id="baa90-106">**Troubleshoot Authentication**: MSAL 支持多种身份验证流程，用于不同的应用场景。</span><span class="sxs-lookup"><span data-stu-id="baa90-106">**Troubleshoot Authentication**: The MSAL supports several authentication flows for use in different application scenarios.</span></span> <span data-ttu-id="baa90-107">根据客户应用程序的构建方式，MSAL 可以使用 Microsoft 标识平台支持的一种或多种认证流。</span><span class="sxs-lookup"><span data-stu-id="baa90-107">Depending on how your client application is built, the MSAL can use one or more of the authentication flows supported by the Microsoft identity platform.</span></span> <span data-ttu-id="baa90-108">这些流程可以产生几种类型的令牌和授权码，并需要不同的令牌来使其发挥作用。</span><span class="sxs-lookup"><span data-stu-id="baa90-108">These flows can produce several types of tokens and authorization codes, and require different tokens to make them work.</span></span>

3. <span data-ttu-id="baa90-109">**访问令牌**: [Microsoft 身份平台访问令牌](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - 了解 API 如何验证和使用访问令牌中的声明。</span><span class="sxs-lookup"><span data-stu-id="baa90-109">**Access Tokens**: [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token.</span></span> <span data-ttu-id="baa90-110">本文中除记录外的所有文档都仅适用于已注册的 API 所发布的令牌。</span><span class="sxs-lookup"><span data-stu-id="baa90-110">All documentation in this article, except where noted, applies only to tokens issued for APIs you've registered.</span></span> <span data-ttu-id="baa90-111">此令牌不适用于为 Microsoft 拥有的 API 发布的令牌，也不能用这些令牌来验证 Microsoft 标识平台将如何为所创建的 API 发布令牌。</span><span class="sxs-lookup"><span data-stu-id="baa90-111">It does not apply to tokens issued for Microsoft-owned APIs, nor can those tokens be used to validate how the Microsoft identity platform will issue tokens for an API you create.</span></span>

<span data-ttu-id="baa90-112">**结束对 Azure Active Directory 身份验证库 (ADAL) 的支持**</span><span class="sxs-lookup"><span data-stu-id="baa90-112">**End of support for Azure Active Directory Authentication Library (ADAL)**</span></span>

- <span data-ttu-id="baa90-113">**自 2020 年 6 月 30 日起，** 我们将不再为 ADAL 和 Azure AD Graph 添加任何新功能。</span><span class="sxs-lookup"><span data-stu-id="baa90-113">**Starting June 30th, 2020,** we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="baa90-114">我们将继续提供技术支持和安全更新，但不再提供功能更新。</span><span class="sxs-lookup"><span data-stu-id="baa90-114">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="baa90-115">**自 2022 年 6 月 30 日起，** 我们将终止对 Azure AD Graph 的支持，并且将不再提供技术支持或安全更新。</span><span class="sxs-lookup"><span data-stu-id="baa90-115">**Starting June 30th, 2022,** we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>
- <span data-ttu-id="baa90-116">此时间之后，在现有 OS 版本上使用 ADAL 的应用将继续工作，但将不会 *获得任何技术支持或安全更新*。</span><span class="sxs-lookup"><span data-stu-id="baa90-116">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>
- <span data-ttu-id="baa90-117">此后，使用 Azure AD Graph 的应用可能不再接收来自 Azure AD Graph 端点的响应。</span><span class="sxs-lookup"><span data-stu-id="baa90-117">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="baa90-118">**ADAL 迁移**</span><span class="sxs-lookup"><span data-stu-id="baa90-118">**ADAL Migration**</span></span>

- <span data-ttu-id="baa90-119">我们建议更新到 MSAL，其具有最新的功能和安全更新。</span><span class="sxs-lookup"><span data-stu-id="baa90-119">We recommend updating to the MSAL, which has the latest features and security updates.</span></span>
- <span data-ttu-id="baa90-120">如果使用 Microsoft 应用，请了解 Microsoft 正在支持在结束最后期限之前将其应用程序迁移到 MSAL，以确保它们将受益于 MSAL 持续的安全性和功能改进。</span><span class="sxs-lookup"><span data-stu-id="baa90-120">If you're using Microsoft apps, know that Microsoft is in the process of migrating its apps to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="baa90-121">[请阅读 ADAL 常见问题解答](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)。</span><span class="sxs-lookup"><span data-stu-id="baa90-121">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
2. <span data-ttu-id="baa90-122">[了解如何在不同平台上迁移应用](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance)。</span><span class="sxs-lookup"><span data-stu-id="baa90-122">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span></span>
3. <span data-ttu-id="baa90-123">如果在阅读完应用平台的指南后还有其他问题，可以在 [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html)上以 [azure-ad-adal-deprecation] 为标签发帖，或者在库的 GitHub 储存库中开一个问题。</span><span class="sxs-lookup"><span data-stu-id="baa90-123">If, after reading the guide for your app's platform, you have additional questions, you can post on [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) with the tag [azure-ad-adal-deprecation] or open an issue in library's GitHub repository.</span></span> <span data-ttu-id="baa90-124">请参阅 **MSAL 概述** 文章中的[语言和框架](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks)部分，以获取每个库的报告链接。</span><span class="sxs-lookup"><span data-stu-id="baa90-124">See the [Languages and frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) section of the **MSAL overview** article for links to each library's repo.</span></span>
4. <span data-ttu-id="baa90-125">**如果需要帮助了解哪些应用程序使用 ADAL**，我们建议查看所有应用程序的源代码。</span><span class="sxs-lookup"><span data-stu-id="baa90-125">**If you need help understanding which of your apps use ADAL**, we recommend you review all of your apps' source code.</span></span> <span data-ttu-id="baa90-126">如果适用，请联系任何独立软件供应程序 (ISV) 或应用程序供应程序。</span><span class="sxs-lookup"><span data-stu-id="baa90-126">If applicable, reach out to any Independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="baa90-127">Microsoft 支持部门也可提供租户内所有非 Microsoft ADAL 应用的列表。</span><span class="sxs-lookup"><span data-stu-id="baa90-127">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>







