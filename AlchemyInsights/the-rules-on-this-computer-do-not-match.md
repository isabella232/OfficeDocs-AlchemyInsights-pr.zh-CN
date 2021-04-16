---
title: 错误：此计算机上规则不匹配
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782942"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="d2781-102">错误：此计算机上规则不匹配</span><span class="sxs-lookup"><span data-stu-id="d2781-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="d2781-103">To see updated status of this known issue， see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="d2781-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="d2781-104">Outlook 团队已实施内部版本 12928.10000 中的修补程序。</span><span class="sxs-lookup"><span data-stu-id="d2781-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="d2781-105">修复程序已在预览体验成员 - 快，并将于 2020 年 6 月底转到每月频道。</span><span class="sxs-lookup"><span data-stu-id="d2781-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="d2781-106">获得固定版本后，你最后一次可能会收到提示"要保留哪些规则"。</span><span class="sxs-lookup"><span data-stu-id="d2781-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="d2781-107">在系统提示时选择"服务器"，然后在 Outlook 中返回，然后重新启用任何已禁用的规则。</span><span class="sxs-lookup"><span data-stu-id="d2781-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="d2781-108">在修补程序可用之前，请使用以下解决方法：</span><span class="sxs-lookup"><span data-stu-id="d2781-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="d2781-109">**解决方法**：最近的报告中，仅在 Outlook 桌面版中创建客户端规则的人出现了问题。</span><span class="sxs-lookup"><span data-stu-id="d2781-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="d2781-110">如果您继续遇到此问题，请考虑删除规则，然后仅在 OWA (Outlook Web App) 并编辑规则，直到问题得到解决。</span><span class="sxs-lookup"><span data-stu-id="d2781-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="d2781-111">如果无法手动删除规则，可以在通过运行 /cleanrules 命令启动 Outlook 时Outlook.exe Outlook 命令。</span><span class="sxs-lookup"><span data-stu-id="d2781-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="d2781-112">这将同时删除客户端和服务器规则。</span><span class="sxs-lookup"><span data-stu-id="d2781-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="d2781-113">它将删除 Outlook 配置文件中所有帐户的所有规则。</span><span class="sxs-lookup"><span data-stu-id="d2781-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="d2781-114">命令行开关一文进一步记录了此命令。</span><span class="sxs-lookup"><span data-stu-id="d2781-114">This command is further documented in the Command-line switches article.</span></span>

