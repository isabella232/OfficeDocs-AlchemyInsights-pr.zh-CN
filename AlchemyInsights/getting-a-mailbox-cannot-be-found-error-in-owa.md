---
title: 126在 OWA 中找不到获取邮箱的错误？
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 9a8897767ebfebac5807116251634c615ef6767d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47706740"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>在 web 上的 Outlook 中获取 "找不到邮箱" 错误？

如果您使用的是 web 上的 Outlook，但 **无法找到错误的邮箱** ，则用于连接到 web 上的 outlook 的帐户没有 Exchange Online 许可证，因此没有邮箱与该帐户相关联。 您的管理员可以通过执行以下步骤，将许可证分配给您的帐户：

1. 打开[Microsoft 365 管理中心](https://portal.office.com/adminportal/home#/homepage)并转到 "**用户**" 部分下的 "**活动用户**"，然后选择查看错误的用户。

2. 在打开的用户页中，转到 " **许可证和应用** " 部分，选择适当的 " **位置** " 值，然后分配包含 Exchange Online (的许可证。展开许可证以查看其详细信息) 。 完成后，单击“**保存更改**”。
