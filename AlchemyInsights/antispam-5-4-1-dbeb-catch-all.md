---
title: 反垃圾邮件 5.4.1 DBEB 捕获全部
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707901"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="f4bc9-102">修复错误代码550的传递问题5.4.1 中继访问被拒绝</span><span class="sxs-lookup"><span data-stu-id="f4bc9-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="f4bc9-103">当您在进入 Microsoft 网络时[检查电子邮件地址是否有效以防止 bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking)时，会出现此问题。</span><span class="sxs-lookup"><span data-stu-id="f4bc9-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="f4bc9-104">请尝试执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="f4bc9-104">Try the following:</span></span>

1. <span data-ttu-id="f4bc9-105">确定问题是否特定于整个域或单个电子邮件地址：</span><span class="sxs-lookup"><span data-stu-id="f4bc9-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="f4bc9-106">整个域：有时域需要同步;尝试[将域设置为 "内部"，然后再设置为 "权威"](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)。</span><span class="sxs-lookup"><span data-stu-id="f4bc9-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="f4bc9-107">单个电子邮件地址：有时需要同步地址;更改 smtp 代理地址，然后将其更改为 "可帮助"。</span><span class="sxs-lookup"><span data-stu-id="f4bc9-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="f4bc9-108">确定问题是否特定于组或公用文件夹。</span><span class="sxs-lookup"><span data-stu-id="f4bc9-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="f4bc9-109">对于某些对象类型，可能需要在 Azure Active Directory 中手动创建对象。</span><span class="sxs-lookup"><span data-stu-id="f4bc9-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="f4bc9-110">如果需要更多帮助，请打开支持票证并指定问题的范围（包括您要发送到的对象的类型），以便我们可以为你提供更好的帮助。</span><span class="sxs-lookup"><span data-stu-id="f4bc9-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>