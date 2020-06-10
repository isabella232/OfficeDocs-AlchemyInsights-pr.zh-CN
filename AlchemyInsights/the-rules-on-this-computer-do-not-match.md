---
title: 错误：此计算机上的规则不匹配
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c0982da82826d1644f437b19e0d343a59d7ac473
ms.sourcegitcommit: e09af4285c6b81ca0a5320fdb811713ac25748c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/09/2020
ms.locfileid: "44664236"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="002c7-102">错误：此计算机上的规则不匹配</span><span class="sxs-lookup"><span data-stu-id="002c7-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="002c7-103">若要查看此已知问题的更新状态，请参阅[此计算机上的规则与 Microsoft Exchange 上的规则不匹配](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="002c7-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="002c7-104">Outlook 团队已在内部版本12928.10000 中实施了修补程序。</span><span class="sxs-lookup"><span data-stu-id="002c7-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="002c7-105">该修补程序已在有问必答内快速进行，并将于 6 2020 月6日后期进入每月频道。</span><span class="sxs-lookup"><span data-stu-id="002c7-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="002c7-106">获得固定生成后，您可能会收到提示 "您想要保留哪条规则" 一次。</span><span class="sxs-lookup"><span data-stu-id="002c7-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="002c7-107">出现提示时选择 "服务器"，然后返回到 Outlook 并重新启用已禁用的任何规则。</span><span class="sxs-lookup"><span data-stu-id="002c7-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="002c7-108">在修补程序可用之前，请使用以下解决方法：</span><span class="sxs-lookup"><span data-stu-id="002c7-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="002c7-109">**解决方法**：在最近的报告中，只有在 Outlook desktop 中创建了客户端规则的客户端才会出现此问题。</span><span class="sxs-lookup"><span data-stu-id="002c7-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="002c7-110">如果仍遇到问题，请考虑删除这些规则，然后仅在 OWA （Outlook Web App）中创建和编辑规则，直到问题得到解决。</span><span class="sxs-lookup"><span data-stu-id="002c7-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="002c7-111">如果您无法手动删除规则，则可以在通过运行/cleanrules. 启动 outlook 时运行 Outlook 命令。</span><span class="sxs-lookup"><span data-stu-id="002c7-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="002c7-112">这将同时删除客户端和服务器规则。</span><span class="sxs-lookup"><span data-stu-id="002c7-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="002c7-113">它将删除 Outlook 配置文件中所有帐户的所有规则。</span><span class="sxs-lookup"><span data-stu-id="002c7-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="002c7-114">命令行开关一文中会进一步介绍此命令。</span><span class="sxs-lookup"><span data-stu-id="002c7-114">This command is further documented in the Command-line switches article.</span></span>

