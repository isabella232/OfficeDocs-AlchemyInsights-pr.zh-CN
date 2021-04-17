---
title: 日历权限
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
- "3800009"
- "611"
ms.openlocfilehash: bbd49134bd4a4451649b76bb5f60b19065910cae
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819898"
---
# <a name="calendar-permissions"></a><span data-ttu-id="4be02-102">日历权限</span><span class="sxs-lookup"><span data-stu-id="4be02-102">Calendar Permissions</span></span>

<span data-ttu-id="4be02-103">用户可以使用 Web 上的 Outlook 或其他客户端更改其自己的日历权限，但作为管理员，你可能需要进行调查。</span><span class="sxs-lookup"><span data-stu-id="4be02-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="4be02-104">使用 Exchange PowerShell cmdlet 将显示用户日历上的权限：</span><span class="sxs-lookup"><span data-stu-id="4be02-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="4be02-105">有关详细信息，请参阅以下内容：</span><span class="sxs-lookup"><span data-stu-id="4be02-105">To see more information see the following:</span></span>

- [<span data-ttu-id="4be02-106">Get-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="4be02-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="4be02-107">Set-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="4be02-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="4be02-108">Add-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="4be02-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="4be02-109">日历权限用于共享日历，若要详细了解如何共享 Outlook 日历，请参阅以下文章：</span><span class="sxs-lookup"><span data-stu-id="4be02-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="4be02-110">与其他人共享 Outlook 日历</span><span class="sxs-lookup"><span data-stu-id="4be02-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="4be02-111">在适用于企业 Web 的 Outlook 中共享日历</span><span class="sxs-lookup"><span data-stu-id="4be02-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="4be02-112">若要解决日历权限问题，可以使用 [支持和恢复助手](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) 工具。</span><span class="sxs-lookup"><span data-stu-id="4be02-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>