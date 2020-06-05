---
title: 隔离中缺少电子邮件
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2020
ms.locfileid: "44542087"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="f8432-102">隔离中缺少电子邮件 "</span><span class="sxs-lookup"><span data-stu-id="f8432-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="f8432-103">管理员可以[查看、释放或删除这些邮件。](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="f8432-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="f8432-104">若要打开安全 & 合规中心，请转到 [https://protection.office.com](https://protection.office.com/) 。</span><span class="sxs-lookup"><span data-stu-id="f8432-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="f8432-105">若要直接打开隔离页面，请转到 [https://protection.office.com/quarantine](https://protection.office.com/quarantine) 。</span><span class="sxs-lookup"><span data-stu-id="f8432-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="f8432-106">可以按下面的值搜索：</span><span class="sxs-lookup"><span data-stu-id="f8432-106">You can search by the following values:</span></span>  

- <span data-ttu-id="f8432-107">**邮件 ID**：邮件的全局唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f8432-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="f8432-108">如果选择列表中的邮件，则会在显示的 "**详细信息**" 弹出窗口中显示**邮件 ID**值。</span><span class="sxs-lookup"><span data-stu-id="f8432-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="f8432-109">管理员可以使用[邮件跟踪](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide)来查找邮件及其相应“邮件 ID”值。</span><span class="sxs-lookup"><span data-stu-id="f8432-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="f8432-110">**发件人电子邮件地址**：单个发件人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="f8432-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="f8432-111">**收件人电子邮件地址**：单个收件人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="f8432-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="f8432-112">**主题**：使用邮件的整个主题。</span><span class="sxs-lookup"><span data-stu-id="f8432-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="f8432-113">搜索不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="f8432-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="f8432-114">输入搜索条件后，单击 " ![ 刷新按钮 ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **刷新**" 以筛选结果。  </span><span class="sxs-lookup"><span data-stu-id="f8432-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="f8432-115">用于查看和管理隔离区中的邮件和文件的 cmdlet 为：</span><span class="sxs-lookup"><span data-stu-id="f8432-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="f8432-116">删除-Get-quarantinemessage</span><span class="sxs-lookup"><span data-stu-id="f8432-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="f8432-117">Export-Get-quarantinemessage</span><span class="sxs-lookup"><span data-stu-id="f8432-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="f8432-118">Get-quarantinemessage</span><span class="sxs-lookup"><span data-stu-id="f8432-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="f8432-119">[Preview-get-quarantinemessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)：请注意，此 cmdlet 仅适用于邮件，而不适用于 SharePoint Online、OneDrive for Business 或团队的 ATP 中的恶意软件文件。</span><span class="sxs-lookup"><span data-stu-id="f8432-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="f8432-120">发布-Get-quarantinemessage</span><span class="sxs-lookup"><span data-stu-id="f8432-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)