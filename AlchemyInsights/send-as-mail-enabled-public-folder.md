---
title: 在 EXO 中以启用邮件的形式发送公用文件夹
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
- "1956"
- "3500007"
ms.openlocfilehash: 0765262c04571e7df139de993611fd6e67068c54
ms.sourcegitcommit: 45635cc7a6c36d6c7b5f78215ad32f2aa7e3aed0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/08/2020
ms.locfileid: "48394685"
---
# <a name="sendas-mail-enabled-public-folder"></a><span data-ttu-id="c6f67-102">SendAs 启用邮件的公用文件夹</span><span class="sxs-lookup"><span data-stu-id="c6f67-102">SendAs Mail Enabled Public Folder</span></span>

<span data-ttu-id="c6f67-103">下面的示例将已启用邮件的公用文件夹 NewPF1 的 "代理发送" 权限分配给用户 Jason。</span><span class="sxs-lookup"><span data-stu-id="c6f67-103">The following example assigns "Send As" permissions for the mail-enabled public folder NewPF1 to the user Jason.</span></span>

<span data-ttu-id="c6f67-104">Add-RecipientPermission-Identity "NewPF1"-受信者 "Jason"-AccessRights "SendAs"</span><span class="sxs-lookup"><span data-stu-id="c6f67-104">Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'</span></span>

<span data-ttu-id="c6f67-105">有关详细的语法和参数信息，请参阅为 [已启用邮件的公用文件夹分配 "代理发送" 或 "代表发送" 权限](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs)。</span><span class="sxs-lookup"><span data-stu-id="c6f67-105">For detailed syntax and parameter information see [Assign "Send As" or "Send on Behalf" permissions for mail-enabled public folders](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span></span>
