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
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959485"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook 无法连接到公用文件夹

如果公用文件夹访问不能为少数用户工作，请尝试以下操作：

连接到 EXO PowerShell，并在有问题的用户帐户上配置 DefaultPublicFolderMailbox，使其与工作用户帐户上的相匹配。

示例：

Get 邮箱 WorkingUser |ft DefaultPublicFolderMailbox、EffectivePublicFolderMailbox

Set-邮箱 ProblemUser-DefaultPublicFolderMailbox \<来自上一个命令的值>

至少等待一个小时，更改才会生效。