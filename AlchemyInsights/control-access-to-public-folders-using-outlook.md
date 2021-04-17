---
title: 使用Outlook控制对公共文件夹的访问
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816730"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="5fb8b-102">使用Outlook控制对公共文件夹的访问</span><span class="sxs-lookup"><span data-stu-id="5fb8b-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="5fb8b-103">使用 Outlook 控制哪些用户可以访问公用文件夹，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="5fb8b-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="5fb8b-104">使用 `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="5fb8b-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="5fb8b-105">$true：允许用户在 Outlook 中访问公用文件夹</span><span class="sxs-lookup"><span data-stu-id="5fb8b-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="5fb8b-106">$false：防止用户在Outlook 中访问公用文件夹。</span><span class="sxs-lookup"><span data-stu-id="5fb8b-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="5fb8b-107">此值为默认值。</span><span class="sxs-lookup"><span data-stu-id="5fb8b-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="5fb8b-108">注意：此过程仅可控制与 Windows 客户端的 Outlook 桌面版的连接。</span><span class="sxs-lookup"><span data-stu-id="5fb8b-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="5fb8b-109">用户可以使用 OWA 或 Outlook for Mac 继续访问公用文件夹。</span><span class="sxs-lookup"><span data-stu-id="5fb8b-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="5fb8b-110">如需了解更多信息，请参阅 [ Outlook 中对公用文件夹的受控连接](https://aka.ms/controlpf)。</span><span class="sxs-lookup"><span data-stu-id="5fb8b-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
