---
title: 日历权限
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748783"
---
# <a name="calendar-permissions"></a>日历权限

用户可以使用 Web 上的 Outlook 或其他客户端更改自己的日历权限，但作为管理员，您可能还需要调查。  
使用 Exchange PowerShell cmdlet 将向你显示对用户日历的权限：

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

若要查看详细信息，请参阅以下内容：

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Add-mailboxfolderpermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [外接 Add-mailboxfolderpermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

日历权限用于共享日历，若要查看有关共享 Outlook 日历的详细信息，请参阅以下文章：

- [与其他人共享 Outlook 日历](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [在适用于企业的 Outlook 网页版中共享日历](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

若要解决日历权限问题，您可以使用 " [支持和恢复助手](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) " 工具。