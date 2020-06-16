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
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="4c81f-102">所有者无法使用 Outlook 创建子文件夹</span><span class="sxs-lookup"><span data-stu-id="4c81f-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="4c81f-103">**在公用文件夹所有者使用 Outlook 创建子文件夹时一直都存在问题。该问题将很快得到修复。**</span><span class="sxs-lookup"><span data-stu-id="4c81f-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="4c81f-104">在此期间，请使用以下解决方法中的一个：</span><span class="sxs-lookup"><span data-stu-id="4c81f-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="4c81f-105">使用 Outlook for MAC 创建子文件夹，因为此问题仅影响 Windows 中的 Outlook 桌面版（所有版本）</span><span class="sxs-lookup"><span data-stu-id="4c81f-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="4c81f-106">请管理员使用 EXO Shell 或 EAC 创建子文件夹</span><span class="sxs-lookup"><span data-stu-id="4c81f-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="4c81f-107">将用户上的 DefaultPublicFolderMailbox/EffectivePublicFolderMailbox 更改为导致问题的文件夹的内容邮箱以外的其他邮箱</span><span class="sxs-lookup"><span data-stu-id="4c81f-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="4c81f-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="4c81f-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="4c81f-109">稍等片刻，然后重新启动 Outlook 客户端</span><span class="sxs-lookup"><span data-stu-id="4c81f-109">Wait for an hour, restart outlook client</span></span>