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
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="c0c3f-102">Outlook 无法连接到公用文件夹</span><span class="sxs-lookup"><span data-stu-id="c0c3f-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="c0c3f-103">如果公用文件夹访问不能为某些用户工作，请尝试以下操作：</span><span class="sxs-lookup"><span data-stu-id="c0c3f-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="c0c3f-104">连接到 EXO PowerShell，并在有问题的用户帐户上配置 DefaultPublicFolderMailbox 参数，使其与工作用户帐户上的参数相匹配。</span><span class="sxs-lookup"><span data-stu-id="c0c3f-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="c0c3f-105">示例：</span><span class="sxs-lookup"><span data-stu-id="c0c3f-105">Example:</span></span>

<span data-ttu-id="c0c3f-106">Get 邮箱 WorkingUser |ft DefaultPublicFolderMailbox、EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="c0c3f-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="c0c3f-107">Set-邮箱 ProblemUser-DefaultPublicFolderMailbox \<来自上一个命令的值></span><span class="sxs-lookup"><span data-stu-id="c0c3f-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="c0c3f-108">至少等待一个小时，更改才会生效。</span><span class="sxs-lookup"><span data-stu-id="c0c3f-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="c0c3f-109">如果问题仍然存在，请按照[以下过程](https://aka.ms/pfcte)使用 Outlook 解决公用文件夹访问问题。</span><span class="sxs-lookup"><span data-stu-id="c0c3f-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>