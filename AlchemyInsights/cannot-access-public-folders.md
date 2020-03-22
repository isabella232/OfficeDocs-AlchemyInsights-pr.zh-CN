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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891739"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook 无法连接到公用文件夹

如果公用文件夹访问不能为某些用户工作，请尝试以下操作：

连接到 EXO PowerShell，并在有问题的用户帐户上配置 DefaultPublicFolderMailbox 参数，使其与工作用户帐户上的参数相匹配。

示例：

Get 邮箱 WorkingUser |ft DefaultPublicFolderMailbox、EffectivePublicFolderMailbox

Set-邮箱 ProblemUser-DefaultPublicFolderMailbox \<来自上一个命令的值>

至少等待一个小时，更改才会生效。

如果问题仍然存在，请按照[以下过程](https://aka.ms/pfcte)使用 Outlook 解决公用文件夹访问问题。