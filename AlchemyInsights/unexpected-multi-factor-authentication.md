---
title: 意外的多重身份验证
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ''
ms.custom:
- "1300007"
- "4372"
ms.openlocfilehash: 48303d5b408cbdb243ec45dc4c80ac9a83f273a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689512"
---
# <a name="unexpected-multi-factor-authentication"></a><span data-ttu-id="5774f-102">意外的多重身份验证</span><span class="sxs-lookup"><span data-stu-id="5774f-102">Unexpected multi-factor authentication</span></span>

<span data-ttu-id="5774f-103">如果你的租户在 2019 年 10 月 21 日后创建，并且意外收到了有关 MFA 的提示，则你的租户中可能启用了[安全性默认值](https://aka.ms/securitydefaults)。</span><span class="sxs-lookup"><span data-stu-id="5774f-103">If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span> 

<span data-ttu-id="5774f-104">要管理安全性默认值：</span><span class="sxs-lookup"><span data-stu-id="5774f-104">To Manage security defaults:</span></span>

1. <span data-ttu-id="5774f-105">使用全局管理员凭据登录[管理中心](https://go.microsoft.com/fwlink/p/?linkid=834822)。</span><span class="sxs-lookup"><span data-stu-id="5774f-105">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="5774f-106">转到 [Azure Active Directory 属性](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties)。</span><span class="sxs-lookup"><span data-stu-id="5774f-106">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="5774f-107">在页面底部，单击“**管理安全性默认值**”。</span><span class="sxs-lookup"><span data-stu-id="5774f-107">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="5774f-108">单击“**是**”启用安全性默认值，或单击“**否**”禁用安全性默认值。</span><span class="sxs-lookup"><span data-stu-id="5774f-108">Click **Yes** to enable security defaults and **No** to disable security defaults.</span></span>
