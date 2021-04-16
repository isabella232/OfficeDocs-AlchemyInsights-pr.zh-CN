---
title: 停用旧版电子数据展示工具
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798539"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="97e2f-102">停用旧版电子数据展示工具</span><span class="sxs-lookup"><span data-stu-id="97e2f-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="97e2f-103">作为 Microsoft 365 合规中心中新增和改进电子数据展示功能的结果，以下旧版电子数据展示工具和命令let 将在几个月后停用：</span><span class="sxs-lookup"><span data-stu-id="97e2f-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="97e2f-104">[Exchange 管理中心中的](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) 就 [地](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) 电子数据展示和就地保留。</span><span class="sxs-lookup"><span data-stu-id="97e2f-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="97e2f-105">支持电子数据展示和保留In-Place Exchange Online PowerShell In-Place cmdlet。</span><span class="sxs-lookup"><span data-stu-id="97e2f-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="97e2f-106"> (这些 cmdlet 统称为\ *-MailboxSearch cmdlet。) 包括以下 cmdlet：</span><span class="sxs-lookup"><span data-stu-id="97e2f-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="97e2f-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="97e2f-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="97e2f-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="97e2f-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="97e2f-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="97e2f-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="97e2f-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="97e2f-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="97e2f-111">Exchange Online PowerShell 中的 [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet。</span><span class="sxs-lookup"><span data-stu-id="97e2f-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="97e2f-112">Exchange Web 服务 API 中的以下操作：</span><span class="sxs-lookup"><span data-stu-id="97e2f-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="97e2f-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="97e2f-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="97e2f-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="97e2f-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="97e2f-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="97e2f-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="97e2f-116">高级电子数据展示 v1.0</span><span class="sxs-lookup"><span data-stu-id="97e2f-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="97e2f-117">**停用时间线**：</span><span class="sxs-lookup"><span data-stu-id="97e2f-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="97e2f-118">**2020 年 7 月 1 日** 你无法再创建新的搜索和保留，但可以自行承担运行、编辑和删除现有搜索的风险。</span><span class="sxs-lookup"><span data-stu-id="97e2f-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="97e2f-119">Microsoft 支持不再支持In-Place EAC &电子数据展示保留。</span><span class="sxs-lookup"><span data-stu-id="97e2f-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="97e2f-120">**2020 年 10** 月 1 In-Place EAC 中的电子数据展示 & 保留功能将置于只读模式，因此只能删除现有搜索和保留。</span><span class="sxs-lookup"><span data-stu-id="97e2f-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="97e2f-121">**有关详细信息，请参阅**：</span><span class="sxs-lookup"><span data-stu-id="97e2f-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="97e2f-122">将旧版电子数据展示搜索和保留迁移到 Microsoft 365 合规中心</span><span class="sxs-lookup"><span data-stu-id="97e2f-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="97e2f-123">旧版电子数据展示工具的停用</span><span class="sxs-lookup"><span data-stu-id="97e2f-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="97e2f-124">有关电子数据展示In-Place保留的常见问题In-Place常见问题</span><span class="sxs-lookup"><span data-stu-id="97e2f-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



