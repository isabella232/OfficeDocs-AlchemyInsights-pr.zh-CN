---
title: 还原已删除的公用文件夹
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
- "3488"
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809429"
---
# <a name="restore-a-deleted-public-folder"></a>还原已删除的公用文件夹

**若要从公用文件夹还原已删除的项目：**

- 请参阅 [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec)。
 
**若要还原已删除的公用文件夹 (类型，) ：** 

- 请使用以下 EXO PowerShell 命令：

    语法：

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    示例：以下命令将还原 Subfolder1，并放在 \Parent1 下：

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

有关 [更多详细信息，请参阅还原已删除](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) 的公用文件夹。
