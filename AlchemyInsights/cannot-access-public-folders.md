---
title: 无法访问公用文件夹
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
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819502"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="fcf1b-102">Outlook 无法连接到公用文件夹</span><span class="sxs-lookup"><span data-stu-id="fcf1b-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="fcf1b-103">如果公用文件夹访问对一些用户没有用，请尝试以下操作：</span><span class="sxs-lookup"><span data-stu-id="fcf1b-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="fcf1b-104">连接到 EXO PowerShell，并针对问题用户帐户配置 DefaultPublicFolderMailbox 参数，以匹配工作用户帐户上的参数。</span><span class="sxs-lookup"><span data-stu-id="fcf1b-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="fcf1b-105">示例：</span><span class="sxs-lookup"><span data-stu-id="fcf1b-105">Example:</span></span>

<span data-ttu-id="fcf1b-106">Get-Mailbox WorkingUser |ft DefaultPublicFolderMailbox，EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="fcf1b-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="fcf1b-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="fcf1b-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="fcf1b-108">等待至少一小时，更改生效。</span><span class="sxs-lookup"><span data-stu-id="fcf1b-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="fcf1b-109">如果问题仍然存在， [请按照此过程使用](https://aka.ms/pfcte) Outlook 解决公用文件夹访问问题。</span><span class="sxs-lookup"><span data-stu-id="fcf1b-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="fcf1b-110">**若要控制哪些用户可以使用 Outlook 访问公用文件夹**：</span><span class="sxs-lookup"><span data-stu-id="fcf1b-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="fcf1b-111">使用 Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true 或 $false</span><span class="sxs-lookup"><span data-stu-id="fcf1b-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="fcf1b-112">$true：允许用户在 Outlook 中访问公用文件夹</span><span class="sxs-lookup"><span data-stu-id="fcf1b-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="fcf1b-113">$false：防止用户在Outlook 中访问公用文件夹。</span><span class="sxs-lookup"><span data-stu-id="fcf1b-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="fcf1b-114">此值为默认值。</span><span class="sxs-lookup"><span data-stu-id="fcf1b-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="fcf1b-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="fcf1b-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="fcf1b-116">**注意** 此过程只能控制与适用于 Windows 客户端的 Outlook 桌面的连接。</span><span class="sxs-lookup"><span data-stu-id="fcf1b-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="fcf1b-117">用户可以继续使用 OWA 或 Outlook for Mac 访问公用文件夹。</span><span class="sxs-lookup"><span data-stu-id="fcf1b-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="fcf1b-118">有关详细信息，请参阅 [宣布支持受控连接到 Outlook 中的公用文件夹](https://aka.ms/controlpf)。</span><span class="sxs-lookup"><span data-stu-id="fcf1b-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>