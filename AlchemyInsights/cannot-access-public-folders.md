---
title: 无法访问公用文件夹
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819502"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook 无法连接到公用文件夹

如果公用文件夹访问对一些用户没有用，请尝试以下操作：

连接到 EXO PowerShell，并针对问题用户帐户配置 DefaultPublicFolderMailbox 参数，以匹配工作用户帐户上的参数。

示例：

Get-Mailbox WorkingUser |ft DefaultPublicFolderMailbox，EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

等待至少一小时，更改生效。

如果问题仍然存在， [请按照此过程使用](https://aka.ms/pfcte) Outlook 解决公用文件夹访问问题。
 
**若要控制哪些用户可以使用 Outlook 访问公用文件夹**：

1.  使用 Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true 或 $false  
      
    $true：允许用户在 Outlook 中访问公用文件夹  
      
    $false：防止用户在Outlook 中访问公用文件夹。 此值为默认值。  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**注意** 此过程只能控制与适用于 Windows 客户端的 Outlook 桌面的连接。 用户可以继续使用 OWA 或 Outlook for Mac 访问公用文件夹。
 
有关详细信息，请参阅 [宣布支持受控连接到 Outlook 中的公用文件夹](https://aka.ms/controlpf)。