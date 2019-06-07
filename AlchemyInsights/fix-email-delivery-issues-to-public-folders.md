---
title: 将电子邮件传递问题修复为已启用邮件的公用文件夹
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 900b6cc2765937ee005c7e7dce5d33bbdf582601
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752658"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="d94dd-102">将电子邮件传递问题修复为已启用邮件的公用文件夹</span><span class="sxs-lookup"><span data-stu-id="d94dd-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="d94dd-103">如果外部发件人无法将邮件发送到已启用邮件的公用文件夹, 并且发件人收到错误:**无法找到 (550 5.4.1)**, 请验证公用文件夹的电子邮件域是否配置为内部中继域, 而不是权威域:</span><span class="sxs-lookup"><span data-stu-id="d94dd-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="d94dd-104">打开[Exchange 管理中心 (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center)。</span><span class="sxs-lookup"><span data-stu-id="d94dd-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="d94dd-105">转到 "**邮件流** \> **接受域**", 选择接受域, 然后单击 "**编辑**"。</span><span class="sxs-lookup"><span data-stu-id="d94dd-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="d94dd-106">在打开的 "属性" 页中, 如果将 "域类型" 设置为 "**权威**", 请将值更改为 "**内部中继**", 然后单击 "**保存**"。</span><span class="sxs-lookup"><span data-stu-id="d94dd-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="d94dd-107">如果外部发件人收到错误 **(550 5.7.13)**, 请在[Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)中运行以下命令, 以查看对公用文件夹中的匿名用户的权限:</span><span class="sxs-lookup"><span data-stu-id="d94dd-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="d94dd-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`例如, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`。</span><span class="sxs-lookup"><span data-stu-id="d94dd-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="d94dd-109">若要允许外部用户向此公用文件夹发送电子邮件, 请向用户匿名添加 "CreateItems" 访问权限。</span><span class="sxs-lookup"><span data-stu-id="d94dd-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="d94dd-110">例如，`Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`。</span><span class="sxs-lookup"><span data-stu-id="d94dd-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
