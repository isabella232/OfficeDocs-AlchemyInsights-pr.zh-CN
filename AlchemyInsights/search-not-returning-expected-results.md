---
title: 1491-搜索-不返回-预期结果
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709217"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="8b76e-102">内容搜索未返回预期结果</span><span class="sxs-lookup"><span data-stu-id="8b76e-102">Content Search not returning expected results</span></span>

<span data-ttu-id="8b76e-103">在从 Microsoft 365 安全 & 合规中心运行内容搜索时，您可能会收到意外的搜索结果。</span><span class="sxs-lookup"><span data-stu-id="8b76e-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="8b76e-104">请考虑可能影响您的搜索结果的以下内容：</span><span class="sxs-lookup"><span data-stu-id="8b76e-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="8b76e-105">**内容位置和搜索条件**：请确保已选择正确的内容位置和搜索条件。</span><span class="sxs-lookup"><span data-stu-id="8b76e-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="8b76e-106">如果您运行的是大型搜索（包含多个位置），请考虑将其拆分为多个搜索。</span><span class="sxs-lookup"><span data-stu-id="8b76e-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="8b76e-107">**部分索引项目**：估计的搜索结果中包含来自邮箱的[部分索引项目](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search)。</span><span class="sxs-lookup"><span data-stu-id="8b76e-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="8b76e-108">但是，搜索估计中不包含来自 SharePoint 和 OneDrive 中的网站的部分索引项。</span><span class="sxs-lookup"><span data-stu-id="8b76e-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="8b76e-109">**搜索失败**：搜索大量邮箱（超过100000个邮箱）时，您可能会收到搜索错误，其中包含错误代码，如 CS008-009 和 CS012-002）。</span><span class="sxs-lookup"><span data-stu-id="8b76e-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="8b76e-110">在这种情况下，请仅对发生故障的内容位置重试搜索。</span><span class="sxs-lookup"><span data-stu-id="8b76e-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="8b76e-111">有关详细信息，请参阅[本文](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search)。</span><span class="sxs-lookup"><span data-stu-id="8b76e-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
