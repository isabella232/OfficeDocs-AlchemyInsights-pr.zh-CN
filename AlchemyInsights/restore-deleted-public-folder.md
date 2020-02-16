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
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063598"
---
# <a name="restore-a-deleted-public-folder"></a>还原已删除的公用文件夹

**若要从公用文件夹还原已删除的项目，** 请执行以下操作：

- 请参阅[无法从 Outlook 2016 中的非邮件公用文件夹中恢复已删除的项目](https://aka.ms/pfrec)。
 
**若要还原已删除的公用文件夹（属于任何类型），请**执行以下操作： 

- 请使用以下 EXO PowerShell 命令：

    语法：

    >$pf = Set-publicfolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT 递归 |？{$_.Name-eq "\<name_of_deleted_public_Folder"};Set-publicfolder $pf-将在其中还原文件夹\<的路径路径>

    示例：下面的命令将还原 Subfolder1，并将其置于 \Parent1 中：

    >$pf = Set-publicfolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT 递归 |？{$_.Name-eq "Subfolder1"};Set-publicfolder $pf identity-路径 \Parent1

有关详细信息，请参阅[还原已删除的公用文件夹](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)。
