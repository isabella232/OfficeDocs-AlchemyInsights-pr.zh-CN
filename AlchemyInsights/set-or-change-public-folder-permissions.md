---
title: 设置或更改公用文件夹权限
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: e419c72a890e68fc7b6d40d2b64406e42f9b0769
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51789197"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="bd96b-102">权限和公用文件夹</span><span class="sxs-lookup"><span data-stu-id="bd96b-102">Permissions and Public Folders</span></span>

<span data-ttu-id="bd96b-103">可以使用 Outlook、Exchange 管理中心或 EAC 管理中心或 PowerShell 更改 (文件夹) 权限：</span><span class="sxs-lookup"><span data-stu-id="bd96b-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="bd96b-104">有关 Outlook 说明， [请单击此处](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx)。</span><span class="sxs-lookup"><span data-stu-id="bd96b-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="bd96b-105">有关 EAC 的说明 [，请参阅](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) 本文。</span><span class="sxs-lookup"><span data-stu-id="bd96b-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> 
    
- <span data-ttu-id="bd96b-106">有关使用 Add-PublicFolderClientPermission commandlet 的说明，请参阅本文。 [](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx)</span><span class="sxs-lookup"><span data-stu-id="bd96b-106">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="bd96b-107">如果需要连接到 Exchange Powershell 的说明，[请单击此处。](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx)</span><span class="sxs-lookup"><span data-stu-id="bd96b-107">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="bd96b-108">如果 **外部用户无法** 向启用邮件的公用文件夹发送电子邮件，原因可能是公用文件夹缺少外部电子邮件传递所需的权限。</span><span class="sxs-lookup"><span data-stu-id="bd96b-108">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="bd96b-109">可以使用此处的 Outlook 说明 [或](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)此处的 PowerShell [说明解决此问题](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx)。</span><span class="sxs-lookup"><span data-stu-id="bd96b-109">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

