---
title: 1374解析两个邮箱 howto
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1374"
- "2692"
- "3500014"
ms.assetid: 8bf1a8f2-58ef-4697-b9c0-be340de96bfe
ms.openlocfilehash: 048c527b26d138535550b5bae399d0ce9fbce0a6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720888"
---
# <a name="a-user-has-two-mailboxes"></a><span data-ttu-id="182dd-102">用户有两个邮箱</span><span class="sxs-lookup"><span data-stu-id="182dd-102">A user has two mailboxes</span></span>

<span data-ttu-id="182dd-103">使用 Azure Active Directory Connect (AAD Connect) 或 DirSync 的混合环境可能会意外导致用户拥有两个邮箱：一个本地和一个在云中。</span><span class="sxs-lookup"><span data-stu-id="182dd-103">Hybrid environments that use Azure Active Directory Connect (AAD Connect) or DirSync might accidentally cause a user to have two mailboxes: one on-premises, and one in the cloud.</span></span> <span data-ttu-id="182dd-104">可以在任意位置创建重复的邮箱。</span><span class="sxs-lookup"><span data-stu-id="182dd-104">A duplicate mailbox could be created in either place.</span></span>

<span data-ttu-id="182dd-105">若要解决此问题，请参阅 [如何在 Exchange Online 和内部部署中同时存在邮箱时进行恢复](https://docs.microsoft.com/exchange/troubleshoot/move-mailboxes/mailbox-exists-exo-onpremises)。</span><span class="sxs-lookup"><span data-stu-id="182dd-105">To resolve this issue, see [How to recover when a mailbox exists in both Exchange Online and on-premises](https://docs.microsoft.com/exchange/troubleshoot/move-mailboxes/mailbox-exists-exo-onpremises).</span></span> <span data-ttu-id="182dd-106">如果您想了解有关如何避免在将来发生此问题的详细信息，请参阅 [我的用户在本地和 Exchange Online 中都有邮箱。帮助！](https://techcommunity.microsoft.com/t5/Exchange-Team-Blog/My-user-has-a-mailbox-both-on-premises-and-in-Exchange-Online/ba-p/846809)。</span><span class="sxs-lookup"><span data-stu-id="182dd-106">If you want to learn more about how to avoid this from happening in the future, see [My user has a mailbox both on-premises and in Exchange Online. Help!](https://techcommunity.microsoft.com/t5/Exchange-Team-Blog/My-user-has-a-mailbox-both-on-premises-and-in-Exchange-Online/ba-p/846809).</span></span>
