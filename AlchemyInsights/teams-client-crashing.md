---
title: Teams 客户端发生了故障？
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826261"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="29da6-102">Teams 客户端发生了故障？</span><span class="sxs-lookup"><span data-stu-id="29da6-102">Teams client crashing?</span></span>

<span data-ttu-id="29da6-103">如果 Teams 客户端发生了故障，请尝试执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="29da6-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="29da6-104">如果使用的是 Teams 桌面应用，请[确保应用已完全更新](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)。</span><span class="sxs-lookup"><span data-stu-id="29da6-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="29da6-105">确保所有 [Microsoft 365 URL 和地址范围](https://docs.microsoft.com/microsoftteams/connectivity-issues)均可访问。</span><span class="sxs-lookup"><span data-stu-id="29da6-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="29da6-106">使用租户管理员帐户登录，然后检查[服务运行状况仪表板](https://docs.microsoft.com/office365/enterprise/view-service-health)，以确认没有任何故障或服务降级。</span><span class="sxs-lookup"><span data-stu-id="29da6-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="29da6-107">卸载并重新安装 Teams 应用程序（链接）</span><span class="sxs-lookup"><span data-stu-id="29da6-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="29da6-108">浏览到计算机上的 %appdata%\Microsoft\teams\ 文件夹，然后删除该目录中的所有文件。</span><span class="sxs-lookup"><span data-stu-id="29da6-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="29da6-109">[下载并安装 Teams 应用](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)，如有可能，请以管理员身份安装 Teams（右键单击 Teams 安装程序，然后选择“以管理员身份运行”(如果有)）。</span><span class="sxs-lookup"><span data-stu-id="29da6-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="29da6-110">如果 Teams 客户端仍出现崩溃，是否可以重现问题？</span><span class="sxs-lookup"><span data-stu-id="29da6-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="29da6-111">如果是这样：</span><span class="sxs-lookup"><span data-stu-id="29da6-111">If so:</span></span>

1. <span data-ttu-id="29da6-112">请使用步骤记录器捕获步骤。</span><span class="sxs-lookup"><span data-stu-id="29da6-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="29da6-113">关闭所有不必要的或机密的应用程序。</span><span class="sxs-lookup"><span data-stu-id="29da6-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="29da6-114">启动步骤记录器并在使用受影响的用户帐户登录时重现该问题。</span><span class="sxs-lookup"><span data-stu-id="29da6-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="29da6-115">[收集捕获记录的重现步骤的 Teams 日志](https://docs.microsoft.com/microsoftteams/log-files)。</span><span class="sxs-lookup"><span data-stu-id="29da6-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="29da6-116">**注意**：请确保捕获受影响用户的登录地址。</span><span class="sxs-lookup"><span data-stu-id="29da6-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="29da6-117">收集转储和/或故障存储桶信息(Windows)。</span><span class="sxs-lookup"><span data-stu-id="29da6-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="29da6-118">在发生崩溃的计算机上启动 Windows Powershell，然后运行以下命令：</span><span class="sxs-lookup"><span data-stu-id="29da6-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="29da6-119">将文件附加到你的支持用例。</span><span class="sxs-lookup"><span data-stu-id="29da6-119">Attach the file to your support case.</span></span>
