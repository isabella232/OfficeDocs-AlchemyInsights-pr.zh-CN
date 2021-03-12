---
title: 副本集
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50716266"
---
# <a name="replica-set"></a><span data-ttu-id="ec8cc-102">副本集</span><span class="sxs-lookup"><span data-stu-id="ec8cc-102">Replica set</span></span>

<span data-ttu-id="ec8cc-103">AADDS 也称为托管域。</span><span class="sxs-lookup"><span data-stu-id="ec8cc-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="ec8cc-104">它实际上是由后端运行和维护的两个域控制器。</span><span class="sxs-lookup"><span data-stu-id="ec8cc-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="ec8cc-105">这两个 DC 包括一个主 DC 和一个复制 DC。</span><span class="sxs-lookup"><span data-stu-id="ec8cc-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="ec8cc-106">AADDS 中的 (托管) 是 Azure 平台管理的自动化过程。</span><span class="sxs-lookup"><span data-stu-id="ec8cc-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="ec8cc-107">如果托管域出现问题，Azure 支持可帮助你从备份中还原。</span><span class="sxs-lookup"><span data-stu-id="ec8cc-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="ec8cc-108">在虚拟网络中创建每个副本集。</span><span class="sxs-lookup"><span data-stu-id="ec8cc-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="ec8cc-109">每个虚拟网络都必须与托管托管域的副本集的所有其他虚拟网络对等。</span><span class="sxs-lookup"><span data-stu-id="ec8cc-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="ec8cc-110">此配置创建支持目录复制的网格网络拓扑。</span><span class="sxs-lookup"><span data-stu-id="ec8cc-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="ec8cc-111">如果每个副本集位于不同的虚拟子网中，虚拟网络可以支持多个副本集。</span><span class="sxs-lookup"><span data-stu-id="ec8cc-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="ec8cc-112">有关副本集的更多详细信息，请参阅 [概念副本集](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)。</span><span class="sxs-lookup"><span data-stu-id="ec8cc-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
