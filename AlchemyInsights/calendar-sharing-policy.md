---
title: 618日历共享策略
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2020
ms.locfileid: "44372989"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="72775-102">共享日历时出现策略错误</span><span class="sxs-lookup"><span data-stu-id="72775-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="72775-103">根据您的具体情况执行下列操作之一：</span><span class="sxs-lookup"><span data-stu-id="72775-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="72775-104">使用远程 PowerShell 连接到 Exchange Online。</span><span class="sxs-lookup"><span data-stu-id="72775-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="72775-105">有关详细信息，请参阅[使用远程 PowerShell 连接到 Exchange Online](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)。</span><span class="sxs-lookup"><span data-stu-id="72775-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="72775-106">在本地服务器上，打开 Exchange 命令行管理程序。</span><span class="sxs-lookup"><span data-stu-id="72775-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="72775-107">确定分配给用户的共享策略。</span><span class="sxs-lookup"><span data-stu-id="72775-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="72775-108">为此，请运行以下命令并记下返回的策略：</span><span class="sxs-lookup"><span data-stu-id="72775-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="72775-109">为用户更新共享策略。</span><span class="sxs-lookup"><span data-stu-id="72775-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="72775-110">要实现这一点，请执行下列步骤：</span><span class="sxs-lookup"><span data-stu-id="72775-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="72775-111">打开“Exchange 管理中心”。</span><span class="sxs-lookup"><span data-stu-id="72775-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="72775-112">单击 "**组织**"，然后双击在**单独共享**中分配给用户的策略。</span><span class="sxs-lookup"><span data-stu-id="72775-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="72775-113">这是在步骤2中返回的策略。</span><span class="sxs-lookup"><span data-stu-id="72775-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="72775-114">在 "共享规则" 页上的 "**指定要共享的信息**" 下，选择要允许的日历共享级别;单击 "**保存**"。</span><span class="sxs-lookup"><span data-stu-id="72775-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="72775-115">有关详细信息，请参阅[当用户尝试共享日历时，"策略不允许将此级别的权限授予一个或多个收件人" 错误](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)。</span><span class="sxs-lookup"><span data-stu-id="72775-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
