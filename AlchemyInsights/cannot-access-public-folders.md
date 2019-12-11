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
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="c538a-102">Outlook 无法连接到公用文件夹</span><span class="sxs-lookup"><span data-stu-id="c538a-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="c538a-103">如果公用文件夹访问不能为少数用户工作，请尝试以下操作：</span><span class="sxs-lookup"><span data-stu-id="c538a-103">If public folder access isn't working for few users, try the following:</span></span>

<span data-ttu-id="c538a-104">连接到 EXO PowerShell，并在有问题的用户帐户上配置 DefaultPublicFolderMailbox，使其与工作用户帐户上的相匹配。</span><span class="sxs-lookup"><span data-stu-id="c538a-104">Connect to EXO PowerShell, and configure the DefaultPublicFolderMailbox on the problem user account to match one on a working user account.</span></span>

<span data-ttu-id="c538a-105">示例：</span><span class="sxs-lookup"><span data-stu-id="c538a-105">Example:</span></span>

<span data-ttu-id="c538a-106">Get 邮箱 WorkingUser |ft DefaultPublicFolderMailbox、EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="c538a-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="c538a-107">Set-邮箱 ProblemUser-DefaultPublicFolderMailbox \<来自上一个命令的值></span><span class="sxs-lookup"><span data-stu-id="c538a-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="c538a-108">至少等待一个小时，更改才会生效。</span><span class="sxs-lookup"><span data-stu-id="c538a-108">Wait at least one hour for the change to take effect.</span></span>