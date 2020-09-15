---
title: 将电子邮件传递问题修复为已启用邮件的公用文件夹
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
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677918"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>将电子邮件传递问题修复为已启用邮件的公用文件夹

如果外部发件人无法将邮件发送到已启用邮件的公用文件夹，并且发件人收到错误：找不到 ** (550 5.4.1) **，请验证公用文件夹的电子邮件域是否配置为内部中继域，而不是权威域：

1. 打开 [Exchange 管理中心 (EAC) ](https://docs.microsoft.com/Exchange/exchange-admin-center)。

2. 转到 " **邮件流** \> **接受域**"，选择接受域，然后单击 " **编辑**"。

3. 在打开的 "属性" 页中，如果将 "域类型" 设置为 " **权威**"，请将值更改为 " **内部中继** "，然后单击 " **保存**"。

如果外部发件人收到错误 ** (550 5.7.13) **，请在 [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) 中运行以下命令，以查看对公用文件夹中的匿名用户的权限：

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` 例如， `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` 。

若要允许外部用户向此公用文件夹发送电子邮件，请向用户匿名添加 "CreateItems" 访问权限。 例如，`Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`。
