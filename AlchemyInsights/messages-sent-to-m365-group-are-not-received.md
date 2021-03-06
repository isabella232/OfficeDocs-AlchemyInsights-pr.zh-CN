---
title: 并非所有成员都会收到发送到 Microsoft 365 组的邮件
ms.author: pebaum
author: pebaum
manager: mnirkhe
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: d222eb92d806bad52264139a8ddba72f323b3783
ms.sourcegitcommit: 10cfd9d552b0d8a096bcef34e82c04a4c166a13a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50479443"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>并非所有成员都会收到发送到 Microsoft 365 组的邮件

确保所有组成员均已订阅以接收电子邮件。 请参阅 [关注 Outlook 中的组](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36)。  

若要查看已订阅组电子邮件的成员的消息状态，请在 [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true) 上运行以下命令：

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

使用以下 EXO PowerShell 命令配置所有团队成员以接收发送到其收件箱中 Microsoft 365 组的电子邮件：

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

例如：

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`