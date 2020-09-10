---
title: 使用Outlook控制对公共文件夹的访问
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: b04e09f5110266d59db82e25cfda1835779fd4b7
ms.sourcegitcommit: b7bbe4c5419668ce8e84196db382032ca09cd176
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/08/2020
ms.locfileid: "47406541"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="8ecb0-102">使用Outlook控制对公共文件夹的访问</span><span class="sxs-lookup"><span data-stu-id="8ecb0-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="8ecb0-103">使用 Outlook 控制哪些用户可以访问公用文件夹，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="8ecb0-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="8ecb0-104">使用 `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="8ecb0-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="8ecb0-105">$true：允许用户在 Outlook 中访问公用文件夹</span><span class="sxs-lookup"><span data-stu-id="8ecb0-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="8ecb0-106">$false：防止用户在Outlook 中访问公用文件夹。</span><span class="sxs-lookup"><span data-stu-id="8ecb0-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="8ecb0-107">此值为默认值。</span><span class="sxs-lookup"><span data-stu-id="8ecb0-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="8ecb0-108">注意：此过程仅可控制与 Windows 客户端的 Outlook 桌面版的连接。</span><span class="sxs-lookup"><span data-stu-id="8ecb0-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="8ecb0-109">用户可以使用 OWA 或 Outlook for Mac 继续访问公用文件夹。</span><span class="sxs-lookup"><span data-stu-id="8ecb0-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="8ecb0-110">如需了解更多信息，请参阅 [ Outlook 中对公用文件夹的受控连接](https://aka.ms/controlpf)。</span><span class="sxs-lookup"><span data-stu-id="8ecb0-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
