---
title: 关于Exchange Server安全更新
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005482"
- "9005483"
- "9413"
- "9412"
ms.openlocfilehash: 87a5cf1ac4dfb96a5406f6b1431adb6ead074fd6
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449045"
---
# <a name="about-exchange-server-security-updates"></a><span data-ttu-id="c6a4a-102">关于Exchange Server安全更新</span><span class="sxs-lookup"><span data-stu-id="c6a4a-102">About Exchange Server Security updates</span></span>

<span data-ttu-id="c6a4a-103">Microsoft 发布了一系列针对本地Exchange Server关键安全更新。</span><span class="sxs-lookup"><span data-stu-id="c6a4a-103">Microsoft has released a series of critical security updates for Exchange Server on-premises.</span></span> <span data-ttu-id="c6a4a-104">受影响的服务器版本是 Exchange Server 2010、2013、2016 和 2019 的任何更新级别。</span><span class="sxs-lookup"><span data-stu-id="c6a4a-104">The affected server versions are any update levels of Exchange Server 2010, 2013, 2016 and 2019.</span></span> <span data-ttu-id="c6a4a-105">Exchange Online 不会受到影响，但如果由于混合配置而具有一些本地 Exchange 服务器，则它们可能会易受攻击。</span><span class="sxs-lookup"><span data-stu-id="c6a4a-105">Exchange Online is NOT impacted, but if you have some on-premises Exchange servers due to Hybrid configuration, they are potentially vulnerable.</span></span>

<span data-ttu-id="c6a4a-106">若要更新内部部署服务器，必须至少运行以下 Exchange 版本：</span><span class="sxs-lookup"><span data-stu-id="c6a4a-106">To update your on-premises servers will have to be running at least the following versions of Exchange:</span></span>

- <span data-ttu-id="c6a4a-107">Exchange 2010 Service Pack 3</span><span class="sxs-lookup"><span data-stu-id="c6a4a-107">Exchange 2010 Service Pack 3</span></span>
- <span data-ttu-id="c6a4a-108">Exchange Server 2013 CU 23</span><span class="sxs-lookup"><span data-stu-id="c6a4a-108">Exchange Server 2013 CU 23</span></span>
- <span data-ttu-id="c6a4a-109">Exchange Server 2016 CU 19 或 CU 18</span><span class="sxs-lookup"><span data-stu-id="c6a4a-109">Exchange Server 2016 CU 19 or CU 18</span></span>
- <span data-ttu-id="c6a4a-110">Exchange Server 2019 CU 8 或 CU 7</span><span class="sxs-lookup"><span data-stu-id="c6a4a-110">Exchange Server 2019 CU 8 or CU 7</span></span>

<span data-ttu-id="c6a4a-111">有关修复位置，请参阅以下公告：已发布[：2021](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)年 3 月Exchange Server安全更新</span><span class="sxs-lookup"><span data-stu-id="c6a4a-111">Please see the following announcement for location of fixes: [Released: March 2021 Exchange Server Security Updates](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span></span>

<span data-ttu-id="c6a4a-112">**重要说明**：</span><span class="sxs-lookup"><span data-stu-id="c6a4a-112">**Important notes:**</span></span>

<span data-ttu-id="c6a4a-113">如果您的本地服务器未按上述列表运行所需的 Exchange 版本，则更新安装将不起作用。</span><span class="sxs-lookup"><span data-stu-id="c6a4a-113">Installation of updates will not work if your on-premises servers are not running required Exchange versions, as per the above list.</span></span>

<span data-ttu-id="c6a4a-114">如果手动安装更新，请阅读更新知识库文章的"已知问题"部分，了解重要信息。</span><span class="sxs-lookup"><span data-stu-id="c6a4a-114">If installing updates manually, please read the "Known issues" section of update KB articles for important information.</span></span> <span data-ttu-id="c6a4a-115">安全更新必须从提升的 CMD/PowerShell 提示符运行！</span><span class="sxs-lookup"><span data-stu-id="c6a4a-115">Security updates MUST be run from elevated CMD/PowerShell prompt!</span></span>
