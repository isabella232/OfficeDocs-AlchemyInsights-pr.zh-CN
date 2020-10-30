---
title: 为 SharePoint、OneDrive 和 Microsoft 团队启用 Office 365 ATP
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801037"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="da112-102">为 SharePoint Online、OneDrive 和 Microsoft 团队启用 Microsoft Defender for Office 365</span><span class="sxs-lookup"><span data-stu-id="da112-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="da112-103">转到 https://protection.office.com 并登录。</span><span class="sxs-lookup"><span data-stu-id="da112-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="da112-104">选择 **威胁管理**  >  **策略**  >  **安全附件** 。</span><span class="sxs-lookup"><span data-stu-id="da112-104">Choose **Threat management** > **Policy** > **Safe Attachments** .</span></span>
3. <span data-ttu-id="da112-105">选择 " **启用 SharePoint、OneDrive 和 Microsoft 团队的 ATP** "，然后单击 " **保存** "。</span><span class="sxs-lookup"><span data-stu-id="da112-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams** , and then click **Save** .</span></span>
4. <span data-ttu-id="da112-106"> (推荐) 为全局管理员或 SharePoint Online 管理员，请运行 [set-spotenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet，并将 **DisallowInfectedFileDownload** 参数设置为 *true* 。</span><span class="sxs-lookup"><span data-stu-id="da112-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true* .</span></span>
5. <span data-ttu-id="da112-107"> (建议的) 为检测到的文件 [设置通知](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) 。</span><span class="sxs-lookup"><span data-stu-id="da112-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="da112-108">ATP 将在 SharePoint Online、OneDrive 或 Microsoft 团队中扫描每个单个文件。</span><span class="sxs-lookup"><span data-stu-id="da112-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="da112-109">文件通过使用共享和来宾活动事件的进程进行异步扫描，同时还通过智能启发和威胁信号来识别恶意文件。</span><span class="sxs-lookup"><span data-stu-id="da112-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="da112-110">请参阅 [适用于 SharePoint、OneDrive 和 Microsoft 团队的 ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)。</span><span class="sxs-lookup"><span data-stu-id="da112-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>