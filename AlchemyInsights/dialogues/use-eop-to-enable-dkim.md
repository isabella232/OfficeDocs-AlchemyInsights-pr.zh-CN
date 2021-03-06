---
title: 使用 Exchange Online PowerShell 为特定域启用 DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500669"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a><span data-ttu-id="6201f-102">使用 Exchange Online PowerShell 为特定域启用 DKIM</span><span class="sxs-lookup"><span data-stu-id="6201f-102">Use Exchange Online PowerShell to enable DKIM for a specific domain</span></span>

<span data-ttu-id="6201f-103">如果无法在管理中心创建 DKIM DNS 记录，请尝试使用 Exchange Online PowerShell。</span><span class="sxs-lookup"><span data-stu-id="6201f-103">If you can't create the DKIM DNS records in the admin center, try using Exchange Online PowerShell.</span></span> 

<span data-ttu-id="6201f-104">若要使用 Exchange Online PowerShell 创建 DKIM DNS 记录，请执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="6201f-104">To create a DKIM DNS record using Exchange Online PowerShell, perform the following steps:</span></span>

1. <span data-ttu-id="6201f-105">以Windows PowerShell打开命令，并按所述顺序运行以下命令：</span><span class="sxs-lookup"><span data-stu-id="6201f-105">Open Windows PowerShell as an administrator and run the following commands in the described sequence:</span></span>

    <span data-ttu-id="6201f-106">a.</span><span class="sxs-lookup"><span data-stu-id="6201f-106">a.</span></span> `$UserCredential = Get-Credential`

    <span data-ttu-id="6201f-107">b.</span><span class="sxs-lookup"><span data-stu-id="6201f-107">b.</span></span> `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="6201f-108">c.</span><span class="sxs-lookup"><span data-stu-id="6201f-108">c.</span></span> `Import-PSSession $Session -DisableNameChecking`
    
<span data-ttu-id="6201f-109">如果在连接到 Exchange Online PowerShell 时遇到问题，请参阅["连接到 Exchange Online PowerShell"。](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="6201f-109">If you have trouble connecting to Exchange Online PowerShell, see [Connect to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="6201f-110">连接到 Exchange Online PowerShell 后，运行以下命令：</span><span class="sxs-lookup"><span data-stu-id="6201f-110">Once you're connected to Exchange Online PowerShell, run the following command:</span></span>

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. <span data-ttu-id="6201f-111">成功执行上述命令后，运行以下命令以终止 Exchange Online PowerShell 会话：</span><span class="sxs-lookup"><span data-stu-id="6201f-111">Once the above command has been successfully executed, run the following command to terminate the Exchange Online PowerShell session:</span></span>

    `Remove-PSSession $Session` 



