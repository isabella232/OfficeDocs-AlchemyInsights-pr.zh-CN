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
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28277932"
---
如果用户具有的 Exchange 许可证，您仅可以将用户邮箱转换为共享邮箱。转换邮箱后，它将继续显示的活动用户列表中，因为该列表包含共享的邮箱。但是，转换后的邮箱将还显示共享的邮箱列表中。 
  
如果您尝试将转换 Exchange 管理控制台中的邮箱，并在转换失败，则清除您的浏览器缓存和 cookie 并重试。如果仍无法工作，请尝试将 Exchange 命令行管理程序中的邮箱转换通过运行以下命令：
  
```
Set-Mailbox -Type Shared
```

[转换共享邮箱的用户邮箱](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba)中提供邮箱转换的详细信息。
  
