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
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996620"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook无法连接到公用文件夹

如果公用文件夹访问对一些用户没有用，请尝试以下操作：

连接 EXO PowerShell，并针对问题用户帐户配置 DefaultPublicFolderMailbox 参数，以匹配工作用户帐户上的参数。

示例：

Get-Mailbox WorkingUser |ft DefaultPublicFolderMailbox，EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

等待至少一小时，更改生效。

如果问题仍然存在，请按照此过程[使用](https://aka.ms/pfcte)Outlook 解决公用文件夹访问Outlook。
 
**若要控制哪些用户可以使用 Outlook：**

1.  使用 Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true 或 $false  
      
    $true：允许用户在 Outlook 中访问公用文件夹  
      
    $false：防止用户在Outlook 中访问公用文件夹。 此值为默认值。  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**注意** 此过程只能控制与客户端Outlook桌面Windows连接。 用户可以继续使用 OWA 或 Outlook for Mac。
 
有关详细信息，请参阅宣布支持受控连接到公用文件夹[Outlook。](https://aka.ms/controlpf)