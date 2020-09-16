---
title: 以 Microsoft 365 组的身份发送
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 51bd8a10c3da23941cc16d7ba860406f8477044a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740141"
---
# <a name="send-as-microsoft-365-group"></a><span data-ttu-id="ec1ae-102">以 Microsoft 365 组的身份发送</span><span class="sxs-lookup"><span data-stu-id="ec1ae-102">Send As Microsoft 365 group</span></span>

<span data-ttu-id="ec1ae-103">可以分配“发送方式”权限，允许特定用户以 Microsoft 365 组的身份发送邮件：</span><span class="sxs-lookup"><span data-stu-id="ec1ae-103">You can assign Send As permissions to allow specific users to send messages as a Microsoft 365 group:</span></span>  

1. <span data-ttu-id="ec1ae-104">连接到 Exchange Online PowerShell。</span><span class="sxs-lookup"><span data-stu-id="ec1ae-104">Connect to Exchange Online PowerShell.</span></span>  

2. <span data-ttu-id="ec1ae-105">运行以下命令：</span><span class="sxs-lookup"><span data-stu-id="ec1ae-105">Run the following command:</span></span>  

    <span data-ttu-id="ec1ae-106">Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs</span><span class="sxs-lookup"><span data-stu-id="ec1ae-106">Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs</span></span>

<span data-ttu-id="ec1ae-107">有关详细信息，请参阅[允许成员以组的身份或代表组发送](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide)。</span><span class="sxs-lookup"><span data-stu-id="ec1ae-107">For more information, see [Allow members to send as or send on behalf of a group](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span></span>