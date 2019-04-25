---
title: 流身份验证错误疑难解答
ms.author: kaarins
author: kaarins
ms.date: 6/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c15fed9f-65c6-422e-9d32-87e889a44b51
ms.openlocfilehash: e578149e37c86178b98cf6073f6ed6325f42c455
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32393603"
---
# <a name="troubleshoot-flow-authentication-errors"></a><span data-ttu-id="91b69-102">流身份验证错误疑难解答</span><span class="sxs-lookup"><span data-stu-id="91b69-102">Troubleshoot Flow authentication errors</span></span>

<span data-ttu-id="91b69-103">在许多情况下, 流会因身份验证错误而失败。</span><span class="sxs-lookup"><span data-stu-id="91b69-103">In many cases, flows fail because of an authentication error.</span></span> <span data-ttu-id="91b69-104">如果您具有此类错误, 则错误消息将包含 "未授权", 或者出现错误代码401或403。</span><span class="sxs-lookup"><span data-stu-id="91b69-104">If you have this type of error, the error message contains "Unauthorized," or an error code of 401 or 403 appears.</span></span> <span data-ttu-id="91b69-105">您通常可以通过更新连接来修复身份验证错误:</span><span class="sxs-lookup"><span data-stu-id="91b69-105">You can usually fix an authentication error by updating the connection:</span></span>
  
1. <span data-ttu-id="91b69-106">在 web 门户顶部, 单击或点击齿轮图标以打开 "设置" 菜单, 然后单击或点击 "**连接**"。</span><span class="sxs-lookup"><span data-stu-id="91b69-106">At the top of the web portal, click or tap the gear icon to open the Settings menu, and then click or tap **Connections**.</span></span>
    
2. <span data-ttu-id="91b69-107">滚动到您看到了未经授权的错误消息的连接。</span><span class="sxs-lookup"><span data-stu-id="91b69-107">Scroll to the connection for which you saw the Unauthorized error message.</span></span>
    
3. <span data-ttu-id="91b69-108">在 "连接" 旁边, 单击或点击 "**确认密码**" 链接, 以了解有关未通过身份验证的连接的消息。</span><span class="sxs-lookup"><span data-stu-id="91b69-108">Next to the connection, click or tap the **Verify password** link in the message about the connection not being authenticated.</span></span> 
    
4. <span data-ttu-id="91b69-109">按照出现的说明验证您的凭据, 返回到流运行失败, 然后单击或点击 "**重新提交**"。</span><span class="sxs-lookup"><span data-stu-id="91b69-109">Verify your credentials by following the instructions that appear, return to your flow-run failure, and then click or tap **Resubmit**.</span></span>
    
<span data-ttu-id="91b69-110">有关更多帮助, 请参阅[排除流故障](https://go.microsoft.com/fwlink/?linkid=872110)。</span><span class="sxs-lookup"><span data-stu-id="91b69-110">For more help, see [Troubleshooting a flow](https://go.microsoft.com/fwlink/?linkid=872110).</span></span>
  

