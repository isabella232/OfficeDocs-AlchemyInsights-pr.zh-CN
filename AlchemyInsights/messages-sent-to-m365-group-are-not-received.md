---
title: 并非所有成员都会收到发送到 Microsoft 365 组的邮件
ms.author: pebaum
author: pebaum
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 73c0fd3eb2f022b1c5917849bae676b748025fb69a3a15ba1389b42a6854db9c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53976495"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>并非所有成员都会收到发送到 Microsoft 365 组的邮件

确保所有组成员均已订阅以接收电子邮件。 请参阅 [关注 Outlook 中的组](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36)。  

若要查看已订阅组电子邮件的成员的消息状态，请在 [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true) 上运行以下命令：

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

使用以下 EXO PowerShell 命令配置所有团队成员以接收发送到其收件箱中 Microsoft 365 组的电子邮件：

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

例如：

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`