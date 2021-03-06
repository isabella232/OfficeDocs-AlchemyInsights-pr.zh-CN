---
title: 使用 Exchange Online PowerShell 为特定域启用 DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500669"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>使用 Exchange Online PowerShell 为特定域启用 DKIM

如果无法在管理中心创建 DKIM DNS 记录，请尝试使用 Exchange Online PowerShell。 

若要使用 Exchange Online PowerShell 创建 DKIM DNS 记录，请执行以下步骤：

1. 以Windows PowerShell打开命令，并按所述顺序运行以下命令：

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
如果在连接到 Exchange Online PowerShell 时遇到问题，请参阅["连接到 Exchange Online PowerShell"。](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. 连接到 Exchange Online PowerShell 后，运行以下命令：

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. 成功执行上述命令后，运行以下命令以终止 Exchange Online PowerShell 会话：

    `Remove-PSSession $Session` 



