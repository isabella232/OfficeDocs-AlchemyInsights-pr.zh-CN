---
title: 隔离中缺少电子邮件
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
- "5668"
- "9002625"
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539814"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="e1f20-102">隔离中缺少电子邮件"</span><span class="sxs-lookup"><span data-stu-id="e1f20-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="e1f20-103">管理员可以查看 [、释放或删除这些邮件。](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span><span class="sxs-lookup"><span data-stu-id="e1f20-103">Administrators can [view, release, or delete these messages.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span></span>

<span data-ttu-id="e1f20-104">若要打开安全&合规中心，请转到 [https://protection.office.com](https://protection.office.com/) 。</span><span class="sxs-lookup"><span data-stu-id="e1f20-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="e1f20-105">若要直接打开"隔离"页面，请转到 [https://protection.office.com/quarantine](https://protection.office.com/quarantine) 。</span><span class="sxs-lookup"><span data-stu-id="e1f20-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="e1f20-106">可以按下面的值搜索：</span><span class="sxs-lookup"><span data-stu-id="e1f20-106">You can search by the following values:</span></span>  

- <span data-ttu-id="e1f20-107">**邮件 ID**：邮件的全局唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e1f20-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="e1f20-108">如果在列表中选择邮件，则"邮件 **ID"** 值将显示在出现的"详细信息"飞出窗格中。</span><span class="sxs-lookup"><span data-stu-id="e1f20-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="e1f20-109">管理员可以使用[邮件跟踪](/microsoft-365/security/office-365-security/message-trace-scc)来查找邮件及其相应“邮件 ID”值。</span><span class="sxs-lookup"><span data-stu-id="e1f20-109">Admins can use [message trace](/microsoft-365/security/office-365-security/message-trace-scc) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="e1f20-110">**发件人电子邮件地址**：单个发件人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="e1f20-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="e1f20-111">**收件人电子邮件地址**：单个收件人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="e1f20-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="e1f20-112">**主题**：使用邮件的整个主题。</span><span class="sxs-lookup"><span data-stu-id="e1f20-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="e1f20-113">搜索不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="e1f20-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="e1f20-114">输入搜索条件后，单击“刷新” ![“刷新”按钮](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) 来筛选结果。</span><span class="sxs-lookup"><span data-stu-id="e1f20-114">After you've entered the search criteria, click ![Refresh button](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** to filter the results.</span></span>

<span data-ttu-id="e1f20-115">用于查看和管理隔离邮件和文件的 cmdlet 包括：</span><span class="sxs-lookup"><span data-stu-id="e1f20-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="e1f20-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="e1f20-116">Delete-QuarantineMessage</span></span>](/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="e1f20-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="e1f20-117">Export-QuarantineMessage</span></span>](/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="e1f20-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="e1f20-118">Get-QuarantineMessage</span></span>](/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="e1f20-119">[Preview-QuarantineMessage：](/powershell/module/exchange/preview-quarantinemessage)请注意，此 cmdlet 仅适用于来自 Office 365 for SharePoint Online、OneDrive for Business 或 Teams 的 Microsoft Defender 恶意软件文件。</span><span class="sxs-lookup"><span data-stu-id="e1f20-119">[Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from Microsoft Defender for Office 365 for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="e1f20-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="e1f20-120">Release-QuarantineMessage</span></span>](/powershell/module/exchange/release-quarantinemessage)