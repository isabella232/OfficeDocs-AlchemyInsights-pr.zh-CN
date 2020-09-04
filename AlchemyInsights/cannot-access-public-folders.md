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
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="3659a-102">Outlook 无法连接到公用文件夹</span><span class="sxs-lookup"><span data-stu-id="3659a-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="3659a-103">如果公用文件夹访问不能为某些用户工作，请尝试以下操作：</span><span class="sxs-lookup"><span data-stu-id="3659a-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="3659a-104">连接到 EXO PowerShell，并在有问题的用户帐户上配置 DefaultPublicFolderMailbox 参数，使其与工作用户帐户上的参数相匹配。</span><span class="sxs-lookup"><span data-stu-id="3659a-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="3659a-105">示例：</span><span class="sxs-lookup"><span data-stu-id="3659a-105">Example:</span></span>

<span data-ttu-id="3659a-106">Get 邮箱 WorkingUser |ft DefaultPublicFolderMailbox、EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="3659a-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="3659a-107">Set-邮箱 ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="3659a-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="3659a-108">至少等待一个小时，更改才会生效。</span><span class="sxs-lookup"><span data-stu-id="3659a-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="3659a-109">如果问题仍然存在，请按照 [以下过程](https://aka.ms/pfcte) 使用 Outlook 解决公用文件夹访问问题。</span><span class="sxs-lookup"><span data-stu-id="3659a-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="3659a-110">**若要控制哪些用户可以使用 Outlook 访问公用文件夹，** 请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="3659a-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="3659a-111">使用 Set-casmailbox <mailboxname> -PublicFolderClientAccess $true 或 $false</span><span class="sxs-lookup"><span data-stu-id="3659a-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="3659a-112">$true：允许用户访问 Outlook 中的公用文件夹</span><span class="sxs-lookup"><span data-stu-id="3659a-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="3659a-113">$false：阻止用户访问 Outlook 中的公用文件夹。</span><span class="sxs-lookup"><span data-stu-id="3659a-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="3659a-114">此值为默认值。</span><span class="sxs-lookup"><span data-stu-id="3659a-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="3659a-115">Set-organizationconfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="3659a-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="3659a-116">**注释** 此过程仅可控制适用于 Windows 客户端的 Outlook 桌面的连接。</span><span class="sxs-lookup"><span data-stu-id="3659a-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="3659a-117">用户可以继续使用 OWA 或 Outlook for Mac 访问公用文件夹。</span><span class="sxs-lookup"><span data-stu-id="3659a-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="3659a-118">有关详细信息，请参阅 [宣布支持到 Outlook 中的公用文件夹的受控制连接](https://aka.ms/controlpf)。</span><span class="sxs-lookup"><span data-stu-id="3659a-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>