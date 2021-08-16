---
title: 修复启用邮件的公用文件夹的电子邮件传递问题
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
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068802"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>修复启用邮件的公用文件夹的电子邮件传递问题

如果外部发件人无法向已启用邮件的公用文件夹发送邮件，并且发件人收到错误："找不到 **(550 5.4.1) "，** 请验证公用文件夹的电子邮件域是否配置为 内部中继域 而不是权威域：

1. 在[EAC Exchange中 (管理) 。 ](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. 转到"**邮件流** \> **""接受** 域"，选择接受域，然后单击"编辑 **"。**

3. 在打开的属性页中，如果域类型设置为 **"** 权威"，将值更改为"**内部** 中继"，然后单击"保存 **"。**

如果外部发件人收到您没有权限 **(550 5.7.13)** 的错误，请运行 Exchange Online [PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)中的以下命令以查看公用文件夹中匿名用户的权限：

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` 例如， `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` 。

若要允许外部用户向此公用文件夹发送电子邮件，请将 CreateItems 访问权限添加到匿名用户。 例如，`Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`。
