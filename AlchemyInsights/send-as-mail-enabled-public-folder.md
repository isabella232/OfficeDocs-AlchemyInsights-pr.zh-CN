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
ms.openlocfilehash: ed62c6d7db0ae532f806ce4fdc48f42623bcd545
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451379"
---
# <a name="sendas-mail-enabled-public-folder"></a><span data-ttu-id="ad626-102">SendAs 启用邮件的公用文件夹</span><span class="sxs-lookup"><span data-stu-id="ad626-102">SendAs Mail Enabled Public Folder</span></span>

<span data-ttu-id="ad626-103">下面的示例将已启用邮件的公用文件夹 NewPF1 的 "代理发送" 权限分配给用户 Jason。</span><span class="sxs-lookup"><span data-stu-id="ad626-103">The following example assigns "Send As" permissions for the mail-enabled public folder NewPF1 to the user Jason.</span></span>

<span data-ttu-id="ad626-104">Add-RecipientPermission-Identity "NewPF1"-受信者 "Jason"-AccessRights "SendAs"</span><span class="sxs-lookup"><span data-stu-id="ad626-104">Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'</span></span>

<span data-ttu-id="ad626-105">有关详细的语法和参数信息，请参阅为 [已启用邮件的公用文件夹分配 "代理发送" 或 "代表发送" 权限](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs)。</span><span class="sxs-lookup"><span data-stu-id="ad626-105">For detailed syntax and parameter information see [Assign "Send As" or "Send on Behalf" permissions for mail-enabled public folders](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span></span>

