---
title: 为Office 365、SharePoint和OneDrive启用 ATP Microsoft Teams
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
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543918"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="fcbf2-102">为 Office 365 Online SharePoint、OneDrive 和 Microsoft Teams 启用 Microsoft Defender for Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="fcbf2-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="fcbf2-103">转到 https://protection.office.com 并登录。</span><span class="sxs-lookup"><span data-stu-id="fcbf2-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="fcbf2-104">选择 **"威胁管理**  >  **策略**  >  **保险箱附件"。**</span><span class="sxs-lookup"><span data-stu-id="fcbf2-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="fcbf2-105">选择 **打开 Defender for Office 365 for SharePoint、OneDrive 和 Microsoft Teams，\*\*\*\*然后单击保存。**</span><span class="sxs-lookup"><span data-stu-id="fcbf2-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="fcbf2-106"> (建议) 全局管理员或 SharePoint Online 管理员，运行 [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet，将 **DisallowInfectedFileDownload** 参数设置为 *true。*</span><span class="sxs-lookup"><span data-stu-id="fcbf2-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="fcbf2-107"> (推荐) [设置检测到的文件](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) 的警报。</span><span class="sxs-lookup"><span data-stu-id="fcbf2-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="fcbf2-108">Microsoft Defender for Office 365不会扫描 SharePoint Online、OneDrive 或 Microsoft Teams。</span><span class="sxs-lookup"><span data-stu-id="fcbf2-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="fcbf2-109">通过使用共享和来宾活动事件以及智能启发和威胁信号识别恶意文件的过程，以异步方式扫描文件。</span><span class="sxs-lookup"><span data-stu-id="fcbf2-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="fcbf2-110">请参阅[Microsoft Defender for Office 365 for SharePoint、OneDrive 和 Microsoft Teams。](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="fcbf2-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>