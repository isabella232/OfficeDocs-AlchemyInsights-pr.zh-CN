---
title: 1490-故障排除-电子数据展示-故障
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277828"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="576db-102">内容搜索错误疑难解答</span><span class="sxs-lookup"><span data-stu-id="576db-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="576db-103">在您导出搜索结果时，您是否遇到内容搜索问题或获取故障？</span><span class="sxs-lookup"><span data-stu-id="576db-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="576db-104">例如，运行搜索时是否收到以下信息？</span><span class="sxs-lookup"><span data-stu-id="576db-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="576db-105">CS008 或 CS012 错误</span><span class="sxs-lookup"><span data-stu-id="576db-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="576db-106">服务器忙/timeout 错误</span><span class="sxs-lookup"><span data-stu-id="576db-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="576db-107">出现应用程序错误</span><span class="sxs-lookup"><span data-stu-id="576db-107">Application error occurred</span></span>

<span data-ttu-id="576db-108">或者从大量邮箱中搜索或导出结果时 (超过100000个邮箱) ，您是否收到导出错误？</span><span class="sxs-lookup"><span data-stu-id="576db-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="576db-109">对于这些类型的错误，请重试对失败的内容位置的搜索。</span><span class="sxs-lookup"><span data-stu-id="576db-109">For these types of errors, retry the search for the content locations that have failed.</span></span> <span data-ttu-id="576db-110">有关详细信息，请参阅  [本文](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) 。</span><span class="sxs-lookup"><span data-stu-id="576db-110">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="576db-111">如果要导出超过10万个以上的邮箱，则需要使用以下 Powershell 下载导出结果：  [导出超过10个邮箱的结果](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)。</span><span class="sxs-lookup"><span data-stu-id="576db-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
