---
title: 更改默认 Yammer 域
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002662"
- "5162"
ms.openlocfilehash: 099feb5c58a2b1068a2ec501ff966c6ac73d804d
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991097"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a><span data-ttu-id="78d38-102">更改默认/主 Yammer 域</span><span class="sxs-lookup"><span data-stu-id="78d38-102">Changing the default/primary Yammer domain</span></span>

<span data-ttu-id="78d38-103">Yammer URL 包含 Yammer 网络的当前主域名。</span><span class="sxs-lookup"><span data-stu-id="78d38-103">The Yammer URL contains the current primary domain name for your Yammer network.</span></span> <span data-ttu-id="78d38-104">此域名可能与 Office 365 或 Azure AD 中设置的主域名不匹配。</span><span class="sxs-lookup"><span data-stu-id="78d38-104">This domain name may not match the primary domain name set in Office 365 or Azure AD.</span></span> <span data-ttu-id="78d38-105">根据添加到租户的自定义域数目，以及 Yammer 是否在受支持的配置中（1 个租户：1 个网络，即 1:1），行为上存在差异。</span><span class="sxs-lookup"><span data-stu-id="78d38-105">There are differences in behavior based on the number of custom domains added to the tenant, and whether Yammer is in a supported configuration (1 Tenant: 1 Network, or 1:1).</span></span> <span data-ttu-id="78d38-106">提供了有关 [Yammer 域和 Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) 的文档。</span><span class="sxs-lookup"><span data-stu-id="78d38-106">Documentation on [Yammer domains and Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) is available.</span></span>

<span data-ttu-id="78d38-107">显示错误域的最常见原因是存在多个 Yammer 网络，需要进行合并。</span><span class="sxs-lookup"><span data-stu-id="78d38-107">The most common reason that you see an incorrect domain is that multiple Yammer networks exist and need to be consolidated.</span></span> <span data-ttu-id="78d38-108">使用网络迁移工具[向下整合到单个网络中](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)是至关重要的第一步。</span><span class="sxs-lookup"><span data-stu-id="78d38-108">[Consolidating down to a single network](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) using the network migration tool is an important first step.</span></span> <span data-ttu-id="78d38-109">完成此操作后，再尝试设置主域。</span><span class="sxs-lookup"><span data-stu-id="78d38-109">Complete this before attempting to set your primary domain.</span></span>

<span data-ttu-id="78d38-110">**无自定义域**</span><span class="sxs-lookup"><span data-stu-id="78d38-110">**No custom domains**</span></span>

<span data-ttu-id="78d38-111">对于新租户，来自租户的默认域（例如 fabrikam.onmicrosoft.com）将用于 Yammer。</span><span class="sxs-lookup"><span data-stu-id="78d38-111">For new tenants, the default domain (e.g. fabrikam.onmicrosoft.com) from the tenant will be used for Yammer.</span></span> <span data-ttu-id="78d38-112">主域设置为 yammer.com/fabrikam.onmicrosoft.com。</span><span class="sxs-lookup"><span data-stu-id="78d38-112">The primary domain is set to yammer.com/fabrikam.onmicrosoft.com.</span></span>

<span data-ttu-id="78d38-113">**单个自定义域**</span><span class="sxs-lookup"><span data-stu-id="78d38-113">**Single custom domain**</span></span>

<span data-ttu-id="78d38-114">Yammer 将自动从租户中选择自定义域（例如 fabrikam.com）作为 Yammer 中的主域。</span><span class="sxs-lookup"><span data-stu-id="78d38-114">Yammer will automatically select the custom domain (e.g. fabrikam.com) from the tenant as the primary domain in Yammer.</span></span> <span data-ttu-id="78d38-115">它设置为 yammer.com/fabrikam.com。</span><span class="sxs-lookup"><span data-stu-id="78d38-115">It is set to yammer.com/fabrikam.com.</span></span> <span data-ttu-id="78d38-116">此更改是由域同步服务进行的，可能需要长达 24 小时才能生效。</span><span class="sxs-lookup"><span data-stu-id="78d38-116">This change is made by the domain sync service, and can take up to 24 hours to take effect.</span></span>

<span data-ttu-id="78d38-117">**多个自定义域**</span><span class="sxs-lookup"><span data-stu-id="78d38-117">**Multiple custom domains**</span></span>

<span data-ttu-id="78d38-118">Yammer 可以拥有与默认租户域不同的主域。</span><span class="sxs-lookup"><span data-stu-id="78d38-118">Yammer can have a primary domain that is different from the default tenant domain.</span></span> <span data-ttu-id="78d38-119">由于存在多个自定义域，因此 Yammer 不会尝试猜测可用域中的正确域。</span><span class="sxs-lookup"><span data-stu-id="78d38-119">Since there are multiple custom domains, Yammer does not attempt to guess the correct domain from those available.</span></span> <span data-ttu-id="78d38-120">需要打开一个支持案例，请求将主域名改为所选的主域。</span><span class="sxs-lookup"><span data-stu-id="78d38-120">You need to open a support case to request that the primary domain name is changed to the primary domain of your choice.</span></span>

<span data-ttu-id="78d38-121">**其他疑难解答信息**</span><span class="sxs-lookup"><span data-stu-id="78d38-121">**Additional troubleshooting information**</span></span>

<span data-ttu-id="78d38-122">在某些情况下，租户之间可能移动了域，而域同步服务无法成功运行。</span><span class="sxs-lookup"><span data-stu-id="78d38-122">In some cases domains may have been moved between tenants and the domain sync service has not been able to run successfully.</span></span> <span data-ttu-id="78d38-123">除了不正确的主域之外，可能还会遇到登录或其他问题。</span><span class="sxs-lookup"><span data-stu-id="78d38-123">You may experience sign-in or other issues, in addition to an incorrect primary domain.</span></span> <span data-ttu-id="78d38-124">若要解决此问题，你可能需要 Microsoft 支持部门的帮助将域移动到正确的网络。</span><span class="sxs-lookup"><span data-stu-id="78d38-124">To resolve this problem, domains may need to be moved to the correct network with help from Microsoft Support.</span></span> <span data-ttu-id="78d38-125">这种情况需要直接协助，可能需要一些时间才能解决，特别是如果有一个很长的域名列表。</span><span class="sxs-lookup"><span data-stu-id="78d38-125">This situation requires direct assistance and can take some time to resolve, especially if there is a very long list of domain names.</span></span> <span data-ttu-id="78d38-126">打开一个支持案例，以获取有关解决这些类型问题的帮助。</span><span class="sxs-lookup"><span data-stu-id="78d38-126">Open a support case to get assistance with resolving these types of issues.</span></span>

<span data-ttu-id="78d38-127">在与支持专员协作时，他们将检查是否已在你的控制之下的租户上验证域。</span><span class="sxs-lookup"><span data-stu-id="78d38-127">When working with a support agent, they will check that domains are verified on a tenant under your control.</span></span> <span data-ttu-id="78d38-128">如果将域添加到你的租户但未通过 DNS 验证，他们可能会询问有关这些域的其他验证问题。</span><span class="sxs-lookup"><span data-stu-id="78d38-128">They may ask additional verification questions about your domains if they are added to your tenant but not verified by DNS.</span></span> <span data-ttu-id="78d38-129">请确保 DNS 已对域进行验证，以便加快进程。</span><span class="sxs-lookup"><span data-stu-id="78d38-129">Please ensure that domains are verified by DNS to speed up the process.</span></span>
