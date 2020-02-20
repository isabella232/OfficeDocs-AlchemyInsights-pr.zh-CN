---
title: 还原已删除的公用文件夹
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
- "3488"
ms.openlocfilehash: cd85dd3c0eb14f6e02ac4f912e733468403387aa
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158482"
---
# <a name="restore-a-deleted-public-folder"></a>还原已删除的公用文件夹

**若要从公用文件夹还原已删除的项目，** 请执行以下操作：

- 请参阅[无法从 Outlook 2016 中的非邮件公用文件夹中恢复已删除的项目](https://aka.ms/pfrec)。
 
**若要还原已删除的公用文件夹（属于任何类型），请**执行以下操作： 

- 请使用以下 EXO PowerShell 命令：

    语法：

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    示例：下面的命令将还原 Subfolder1，并将其置于 \Parent1 中：

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

有关详细信息，请参阅[还原已删除的公用文件夹](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)。
