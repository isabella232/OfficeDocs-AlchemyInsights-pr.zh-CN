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
ms.custom: Adm_O365
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: e4e98ba3e7dff2bd86be4667d7262c9544f9c9cb
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29899198"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="bb1ab-102">权限和公用文件夹</span><span class="sxs-lookup"><span data-stu-id="bb1ab-102">Permissions and Public Folders</span></span>

<span data-ttu-id="bb1ab-103">您可以更改上使用 Outlook，Exchange 管理员中心 (EAC) 中，您的公用文件夹的权限或 PowerShell:</span><span class="sxs-lookup"><span data-stu-id="bb1ab-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="bb1ab-104">有关 Outlook 的说明，[请单击此处](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx)。</span><span class="sxs-lookup"><span data-stu-id="bb1ab-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="bb1ab-p101">EAC 中，请参阅[这篇文章](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1)的说明。您可以单击[此处](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx)以导航到 EAC。</span><span class="sxs-lookup"><span data-stu-id="bb1ab-p101">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions. You can click [here](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx) to navigate to EAC.</span></span> 
    
- <span data-ttu-id="bb1ab-p102">有关 Powershell 中，请参阅[本文](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx)以使用 Add-publicfolderclientpermission commandlet 的说明。如果需要连接到 Exchange Powershell 中的说明，请单击[此处](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx)。</span><span class="sxs-lookup"><span data-stu-id="bb1ab-p102">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet. If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="bb1ab-p103">如果**外部用户无法发送电子邮件发送给已启用邮件的公用文件夹**，原因可能是公用文件夹缺少权限所需的外部电子邮件传递。您可以解决此问题使用 Outlook 说明[此处](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)或的 PowerShell 说明[此处](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx)。</span><span class="sxs-lookup"><span data-stu-id="bb1ab-p103">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery. You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

