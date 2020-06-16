---
title: 所有者无法使用 Outlook 创建子文件夹
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2020
ms.locfileid: "44716537"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>所有者无法使用 Outlook 创建子文件夹

**在公用文件夹所有者使用 Outlook 创建子文件夹时一直都存在问题。该问题将很快得到修复。**

在此期间，请使用以下解决方法中的一个：

1. 使用 Outlook for MAC 创建子文件夹，因为此问题仅影响 Windows 中的 Outlook 桌面版（所有版本）
2. 请管理员使用 EXO Shell 或 EAC 创建子文件夹
3. 将用户上的 DefaultPublicFolderMailbox/EffectivePublicFolderMailbox 更改为导致问题的文件夹的内容邮箱以外的其他邮箱  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. 稍等片刻，然后重新启动 Outlook 客户端