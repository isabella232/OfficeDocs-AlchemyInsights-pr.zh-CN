---
title: 无法访问公用文件夹
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341393"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook 无法连接到公用文件夹

如果公用文件夹访问不能为某些用户工作，请尝试以下操作：

连接到 EXO PowerShell，并在有问题的用户帐户上配置 DefaultPublicFolderMailbox 参数，使其与工作用户帐户上的参数相匹配。

示例：

Get 邮箱 WorkingUser |ft DefaultPublicFolderMailbox、EffectivePublicFolderMailbox

Set-邮箱 ProblemUser-DefaultPublicFolderMailbox \<value from previous command>

至少等待一个小时，更改才会生效。

如果问题仍然存在，请按照 [以下过程](https://aka.ms/pfcte) 使用 Outlook 解决公用文件夹访问问题。
 
**若要控制哪些用户可以使用 Outlook 访问公用文件夹，** 请执行以下操作：

1.  使用 Set-casmailbox <mailboxname> -PublicFolderClientAccess $true 或 $false  
      
    $true：允许用户访问 Outlook 中的公用文件夹  
      
    $false：阻止用户访问 Outlook 中的公用文件夹。 此值为默认值。  
        
2.  Set-organizationconfig-PublicFolderShowClientControl $true   
      
**注释** 此过程仅可控制适用于 Windows 客户端的 Outlook 桌面的连接。 用户可以继续使用 OWA 或 Outlook for Mac 访问公用文件夹。
 
有关详细信息，请参阅 [宣布支持到 Outlook 中的公用文件夹的受控制连接](https://aka.ms/controlpf)。