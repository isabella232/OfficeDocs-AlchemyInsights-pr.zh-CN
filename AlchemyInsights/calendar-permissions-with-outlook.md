---
title: 日历权限
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44853980"
---
# <a name="calendar-permissions"></a><span data-ttu-id="22e87-102">日历权限</span><span class="sxs-lookup"><span data-stu-id="22e87-102">Calendar Permissions</span></span>

<span data-ttu-id="22e87-103">用户可以使用 Web 上的 Outlook 或其他客户端更改自己的日历权限，但作为管理员，您可能还需要调查。</span><span class="sxs-lookup"><span data-stu-id="22e87-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="22e87-104">使用 Exchange PowerShell cmdlet 将向你显示对用户日历的权限：</span><span class="sxs-lookup"><span data-stu-id="22e87-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="22e87-105">若要查看详细信息，请参阅以下内容：</span><span class="sxs-lookup"><span data-stu-id="22e87-105">To see more information see the following:</span></span>

- [<span data-ttu-id="22e87-106">Add-mailboxfolderpermission</span><span class="sxs-lookup"><span data-stu-id="22e87-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="22e87-107">Add-mailboxfolderpermission</span><span class="sxs-lookup"><span data-stu-id="22e87-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="22e87-108">外接 Add-mailboxfolderpermission</span><span class="sxs-lookup"><span data-stu-id="22e87-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="22e87-109">日历权限用于共享日历，若要查看有关共享 Outlook 日历的详细信息，请参阅以下文章：</span><span class="sxs-lookup"><span data-stu-id="22e87-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="22e87-110">与其他人共享 Outlook 日历</span><span class="sxs-lookup"><span data-stu-id="22e87-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="22e87-111">在适用于企业的 Outlook 网页版中共享日历</span><span class="sxs-lookup"><span data-stu-id="22e87-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="22e87-112">若要解决日历权限问题，您可以使用 "[支持和恢复助手](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)" 工具。</span><span class="sxs-lookup"><span data-stu-id="22e87-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>