---
title: Teams 客户端崩溃
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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187711"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="e504d-102">Teams 客户端崩溃</span><span class="sxs-lookup"><span data-stu-id="e504d-102">Teams client crashing</span></span>

<span data-ttu-id="e504d-103">如果 Teams 客户端发生了故障，请尝试执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="e504d-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="e504d-104">如果使用的是 Teams 桌面应用，请[确保应用已完全更新](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)。</span><span class="sxs-lookup"><span data-stu-id="e504d-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="e504d-105">确保所有 [Microsoft 365 URL 和地址范围](/microsoftteams/connectivity-issues)均可访问。</span><span class="sxs-lookup"><span data-stu-id="e504d-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="e504d-106">使用租户管理员帐户登录，然后检查[服务运行状况仪表板](/office365/enterprise/view-service-health)，以确认没有任何故障或服务降级。</span><span class="sxs-lookup"><span data-stu-id="e504d-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="e504d-107">卸载并重新安装 Teams 应用程序</span><span class="sxs-lookup"><span data-stu-id="e504d-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="e504d-108">浏览到计算机上的 %appdata%\Microsoft\Teams\ 文件夹，然后删除该目录中的所有文件。</span><span class="sxs-lookup"><span data-stu-id="e504d-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="e504d-109">[下载并安装 Teams 应用](https://www.microsoft.com/microsoft-teams/download-app)，如有可能，请以管理员身份安装 Teams（右键单击 Teams 安装程序，然后选择“**以管理员身份运行**”(如果有)）。</span><span class="sxs-lookup"><span data-stu-id="e504d-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="e504d-110">如果 Teams 客户端仍出现崩溃，请尝试重现问题。</span><span class="sxs-lookup"><span data-stu-id="e504d-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="e504d-111">如果可以：</span><span class="sxs-lookup"><span data-stu-id="e504d-111">If you can:</span></span>

1. <span data-ttu-id="e504d-112">请使用步骤记录器捕获步骤。</span><span class="sxs-lookup"><span data-stu-id="e504d-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="e504d-113">关闭所有不必要的或机密的应用程序。</span><span class="sxs-lookup"><span data-stu-id="e504d-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="e504d-114">启动步骤记录器并在使用受影响的用户帐户登录时重现该问题。</span><span class="sxs-lookup"><span data-stu-id="e504d-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="e504d-115">[收集捕获记录的重现步骤的 Teams 日志](/microsoftteams/log-files)。</span><span class="sxs-lookup"><span data-stu-id="e504d-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="e504d-116">**注意**：请确保捕获受影响用户的登录地址。</span><span class="sxs-lookup"><span data-stu-id="e504d-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="e504d-117">收集转储和/或故障存储桶信息(Windows)。</span><span class="sxs-lookup"><span data-stu-id="e504d-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="e504d-118">在发生崩溃的计算机上启动 Windows Powershell，然后运行以下命令（在每个命令之后按 Enter）：</span><span class="sxs-lookup"><span data-stu-id="e504d-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="e504d-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="e504d-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="e504d-120">生成文本文件并显示在屏幕上后，保存该文件并将其附加到服务请求。</span><span class="sxs-lookup"><span data-stu-id="e504d-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
