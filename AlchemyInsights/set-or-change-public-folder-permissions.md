---
title: 设置或更改公用文件夹权限
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: 1015c2203406e15d6b418c387b6632a182d6d2ff
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36734659"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="b634d-102">权限和公用文件夹</span><span class="sxs-lookup"><span data-stu-id="b634d-102">Permissions and Public Folders</span></span>

<span data-ttu-id="b634d-103">您可以使用 Outlook、Exchange 管理中心（EAC）或 PowerShell 更改对公用文件夹的权限：</span><span class="sxs-lookup"><span data-stu-id="b634d-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="b634d-104">有关 Outlook 说明，请[单击此处](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx)。</span><span class="sxs-lookup"><span data-stu-id="b634d-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="b634d-105">对于 EAC，请参阅[本文](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1)获取相关说明。</span><span class="sxs-lookup"><span data-stu-id="b634d-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> 
    
- <span data-ttu-id="b634d-106">对于 Powershell，请参阅[本文](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx)，了解有关使用外接程序 add-publicfolderclientpermission commandlet 的说明。</span><span class="sxs-lookup"><span data-stu-id="b634d-106">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="b634d-107">如果你需要有关连接到 Exchange Powershell 的说明，请单击[此处](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx)。</span><span class="sxs-lookup"><span data-stu-id="b634d-107">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="b634d-108">如果**外部用户无法将电子邮件发送到已启用邮件的公用文件夹**，则原因可能是公用文件夹缺少外部电子邮件传递所需的权限。</span><span class="sxs-lookup"><span data-stu-id="b634d-108">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="b634d-109">您可以使用 Outlook 中[的说明或 PowerShell 说明来](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)解决此问题[。](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx)</span><span class="sxs-lookup"><span data-stu-id="b634d-109">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

