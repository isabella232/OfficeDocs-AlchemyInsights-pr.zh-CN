---
title: 软件清单缺失或不准确
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52658046"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="f92a2-102">软件清单缺失或不准确</span><span class="sxs-lookup"><span data-stu-id="f92a2-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="f92a2-103">威胁和漏洞管理 （TVM） 中的软件清单是组织中具有官方公共平台枚举 （CPE） 的已知软件列表。</span><span class="sxs-lookup"><span data-stu-id="f92a2-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="f92a2-104">没有官方 CPE 的软件产品不发布漏洞。</span><span class="sxs-lookup"><span data-stu-id="f92a2-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="f92a2-105">库存还包括供应商名称、弱点数、威胁和公开设备数量等详细信息。</span><span class="sxs-lookup"><span data-stu-id="f92a2-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="f92a2-106">设备上的软件更改通常在两小时内反映到安全门户中。</span><span class="sxs-lookup"><span data-stu-id="f92a2-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="f92a2-107">但是，有时可能需要更长时间。</span><span class="sxs-lookup"><span data-stu-id="f92a2-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="f92a2-108">当前无法强制进行同步;这是持续持续评估。</span><span class="sxs-lookup"><span data-stu-id="f92a2-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="f92a2-109">如果 5 小时后进行了软件更改，并且更改未准确反映到 TVM 中，请按照下列步骤操作：</span><span class="sxs-lookup"><span data-stu-id="f92a2-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="f92a2-110">检查软件证据部分，了解系统是如何检测到软件的。</span><span class="sxs-lookup"><span data-stu-id="f92a2-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="f92a2-111">确保软件受支持。</span><span class="sxs-lookup"><span data-stu-id="f92a2-111">Make sure that the software is supported.</span></span> <span data-ttu-id="f92a2-112">软件可能仅在设备级别可见，即使威胁和漏洞管理当前也不支持该软件。</span><span class="sxs-lookup"><span data-stu-id="f92a2-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="f92a2-113">但是，只有有限的数据可用。</span><span class="sxs-lookup"><span data-stu-id="f92a2-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="f92a2-114">有关从门户网站报告不准确度的步骤，请参阅[报告不准确度](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)。</span><span class="sxs-lookup"><span data-stu-id="f92a2-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="f92a2-115">**注意**：从 MDE 门户报告不精确性是工程的一个单向通道。</span><span class="sxs-lookup"><span data-stu-id="f92a2-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="f92a2-116">如果问题紧急，请打开支持票证。</span><span class="sxs-lookup"><span data-stu-id="f92a2-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="f92a2-117">有关详细信息，请参阅[软件清单 - 威胁和漏洞管理](/microsoft-365/security/defender-endpoint/tvm-software-inventory)。</span><span class="sxs-lookup"><span data-stu-id="f92a2-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>