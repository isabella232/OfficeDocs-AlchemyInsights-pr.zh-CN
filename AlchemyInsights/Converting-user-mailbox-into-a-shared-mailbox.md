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
ms.openlocfilehash: 4da54121763fd33aa111f3bb3c26963cd271dc51
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32374313"
---
仅当用户拥有 Exchange 许可证时, 才能将用户邮箱转换为共享邮箱。 在转换邮箱后, 它将继续显示在活动用户列表中, 因为该列表包含共享邮箱。 但是, 已转换的邮箱也会显示在共享邮箱列表中。 
  
如果尝试在 Exchange 管理控制台中转换邮箱, 但转换失败, 请清除您的浏览器缓存和 cookie 并重试。 如果仍不起作用, 请运行以下命令, 尝试在 Exchange 命令行管理程序中转换邮箱:
  
```
Set-Mailbox -Type Shared
```

在 "[将用户邮箱转换为共享邮箱](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba)" 中提供了更多邮箱转换信息。
  
