---
title: 转换共享邮箱的用户邮箱？
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Priority
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 22ad1b3fb818b40bcd77974031735f931e986968
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29459216"
---
<span data-ttu-id="ca647-p101">如果用户具有的 Exchange 许可证，您仅可以将用户邮箱转换为共享邮箱。转换邮箱后，它将继续显示的活动用户列表中，因为该列表包含共享的邮箱。但是，转换后的邮箱将还显示共享的邮箱列表中。</span><span class="sxs-lookup"><span data-stu-id="ca647-p101">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license. After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes. However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="ca647-p102">如果您尝试将转换 Exchange 管理控制台中的邮箱，并在转换失败，则清除您的浏览器缓存和 cookie 并重试。如果仍无法工作，请尝试将 Exchange 命令行管理程序中的邮箱转换通过运行以下命令：</span><span class="sxs-lookup"><span data-stu-id="ca647-p102">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again. If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="ca647-107">[转换共享邮箱的用户邮箱](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba)中提供邮箱转换的详细信息。</span><span class="sxs-lookup"><span data-stu-id="ca647-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
