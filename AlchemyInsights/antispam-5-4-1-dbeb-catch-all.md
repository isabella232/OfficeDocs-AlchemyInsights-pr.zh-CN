---
title: AntiSpam 5.4.1 DBEB catch-all
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
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821437"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="170ec-102">修复错误代码为 550 5.4.1 中继访问被拒绝的传递问题</span><span class="sxs-lookup"><span data-stu-id="170ec-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="170ec-103">在 [检查电子邮件地址是否](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) 有效以防止在进入 Microsoft 网络时发生回弹时，会出现此问题。</span><span class="sxs-lookup"><span data-stu-id="170ec-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="170ec-104">请尝试执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="170ec-104">Try the following:</span></span>

1. <span data-ttu-id="170ec-105">确定问题是特定于整个域还是单个电子邮件地址：</span><span class="sxs-lookup"><span data-stu-id="170ec-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="170ec-106">整个域：有时需要同步域;尝试[将域设置为"内部"，然后返回到"权威"。](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)</span><span class="sxs-lookup"><span data-stu-id="170ec-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="170ec-107">单个电子邮件地址：有时需要同步地址;更改 smtp 代理地址，然后再更改回地址可能会有所帮助。</span><span class="sxs-lookup"><span data-stu-id="170ec-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="170ec-108">确定问题是特定于组还是公用文件夹。</span><span class="sxs-lookup"><span data-stu-id="170ec-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="170ec-109">对于一些对象类型，可能需要在 Azure Active Directory 中手动创建对象。</span><span class="sxs-lookup"><span data-stu-id="170ec-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="170ec-110">如果需要其他帮助，请打开支持票证并指定问题范围 (包括你发送到项目的对象类型) 以便我们可以更好地协助你。</span><span class="sxs-lookup"><span data-stu-id="170ec-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>