---
title: 将电子邮件传递问题修复为已启用邮件的公用文件夹
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 900b6cc2765937ee005c7e7dce5d33bbdf582601
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752658"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>将电子邮件传递问题修复为已启用邮件的公用文件夹

如果外部发件人无法将邮件发送到已启用邮件的公用文件夹, 并且发件人收到错误:**无法找到 (550 5.4.1)**, 请验证公用文件夹的电子邮件域是否配置为内部中继域, 而不是权威域:

1. 打开[Exchange 管理中心 (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center)。

2. 转到 "**邮件流** \> **接受域**", 选择接受域, 然后单击 "**编辑**"。

3. 在打开的 "属性" 页中, 如果将 "域类型" 设置为 "**权威**", 请将值更改为 "**内部中继**", 然后单击 "**保存**"。

如果外部发件人收到错误 **(550 5.7.13)**, 请在[Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)中运行以下命令, 以查看对公用文件夹中的匿名用户的权限:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`例如, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`。

若要允许外部用户向此公用文件夹发送电子邮件, 请向用户匿名添加 "CreateItems" 访问权限。 例如，`Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`。
