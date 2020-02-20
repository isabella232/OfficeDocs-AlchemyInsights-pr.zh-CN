---
title: 旧电子数据展示工具的退休
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: c4632b52dde579b7d5b2e6e15f1583300a0bd136
ms.sourcegitcommit: a7c17217c170ead24571421baaf5a14f1525b1a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42157516"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="20976-102">旧电子数据展示工具的退休</span><span class="sxs-lookup"><span data-stu-id="20976-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="20976-103">由于 Microsoft 365 合规性中心中新增和改进的电子数据展示功能的结果，以下旧的电子数据展示工具和 commandlet 将在接下来的几个月内退出：</span><span class="sxs-lookup"><span data-stu-id="20976-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="20976-104">Exchange 管理中心内的[就地电子数据展示](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery)和[就地保留](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)。</span><span class="sxs-lookup"><span data-stu-id="20976-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="20976-105">支持就地电子数据展示和就地保留的 Exchange Online PowerShell cmdlet。</span><span class="sxs-lookup"><span data-stu-id="20976-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="20976-106">（这些 cmdlet 共同标识为 \*-New-mailboxsearch cmdlet。）这包括以下 cmdlet：</span><span class="sxs-lookup"><span data-stu-id="20976-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="20976-107">新 New-mailboxsearch</span><span class="sxs-lookup"><span data-stu-id="20976-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="20976-108">启动-New-mailboxsearch</span><span class="sxs-lookup"><span data-stu-id="20976-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="20976-109">New-mailboxsearch</span><span class="sxs-lookup"><span data-stu-id="20976-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="20976-110">New-mailboxsearch</span><span class="sxs-lookup"><span data-stu-id="20976-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="20976-111">Exchange Online PowerShell 中的[搜索邮箱](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps)cmdlet。</span><span class="sxs-lookup"><span data-stu-id="20976-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="20976-112">Exchange Web Services API 中的以下操作：</span><span class="sxs-lookup"><span data-stu-id="20976-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="20976-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="20976-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="20976-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="20976-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="20976-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="20976-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="20976-116">Office 365 高级电子数据展示1。0</span><span class="sxs-lookup"><span data-stu-id="20976-116">Office 365 Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="20976-117">**停用的时间线**：</span><span class="sxs-lookup"><span data-stu-id="20976-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="20976-118">2020年4月1日：您将无法创建新的搜索和保留，但您仍可以自行承担运行、编辑和删除现有搜索。</span><span class="sxs-lookup"><span data-stu-id="20976-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="20976-119">Microsoft 支持将不再支持 EAC 中的就地电子数据展示 & 保留。</span><span class="sxs-lookup"><span data-stu-id="20976-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="20976-120">2020年7月1日：就地电子数据展示 & 保留 EAC 中的功能将被置于只读模式下。</span><span class="sxs-lookup"><span data-stu-id="20976-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="20976-121">这意味着您将只能删除现有的搜索和保留。</span><span class="sxs-lookup"><span data-stu-id="20976-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="20976-122">**有关详细信息，请参阅**：</span><span class="sxs-lookup"><span data-stu-id="20976-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="20976-123">将旧式电子数据展示搜索和保留迁移到 Microsoft 365 合规性中心</span><span class="sxs-lookup"><span data-stu-id="20976-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="20976-124">旧电子数据展示工具的退休</span><span class="sxs-lookup"><span data-stu-id="20976-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="20976-125">有关就地电子数据展示和就地保留的常见问题解答</span><span class="sxs-lookup"><span data-stu-id="20976-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



