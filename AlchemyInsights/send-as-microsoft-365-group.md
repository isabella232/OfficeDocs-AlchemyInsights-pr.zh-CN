---
title: 以 Microsoft 365 组的身份发送
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 51bd8a10c3da23941cc16d7ba860406f8477044a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740141"
---
# <a name="send-as-microsoft-365-group"></a>以 Microsoft 365 组的身份发送

可以分配“发送方式”权限，允许特定用户以 Microsoft 365 组的身份发送邮件：  

1. 连接到 Exchange Online PowerShell。  

2. 运行以下命令：  

    Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs

有关详细信息，请参阅[允许成员以组的身份或代表组发送](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide)。