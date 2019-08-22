---
title: 将用户邮箱转换为共享邮箱？
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496389"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a><span data-ttu-id="cb43b-102">将用户邮箱转换为共享邮箱</span><span class="sxs-lookup"><span data-stu-id="cb43b-102">Convert a user mail box into a shared mailbox</span></span>

<span data-ttu-id="cb43b-103">仅当用户拥有 Exchange 许可证时, 才能将用户邮箱转换为共享邮箱。</span><span class="sxs-lookup"><span data-stu-id="cb43b-103">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="cb43b-104">在转换邮箱后, 它将继续显示在活动用户列表中, 因为该列表包含共享邮箱。</span><span class="sxs-lookup"><span data-stu-id="cb43b-104">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="cb43b-105">但是, 已转换的邮箱也会显示在共享邮箱列表中。</span><span class="sxs-lookup"><span data-stu-id="cb43b-105">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="cb43b-106">如果尝试在 Exchange 管理控制台中转换邮箱, 但转换失败, 请清除您的浏览器缓存和 cookie 并重试。</span><span class="sxs-lookup"><span data-stu-id="cb43b-106">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="cb43b-107">如果仍不起作用, 请运行以下命令, 尝试在 Exchange 命令行管理程序中转换邮箱:</span><span class="sxs-lookup"><span data-stu-id="cb43b-107">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="cb43b-108">在 "[将用户邮箱转换为共享邮箱](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox)" 中提供了更多邮箱转换信息。</span><span class="sxs-lookup"><span data-stu-id="cb43b-108">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span></span>
  
