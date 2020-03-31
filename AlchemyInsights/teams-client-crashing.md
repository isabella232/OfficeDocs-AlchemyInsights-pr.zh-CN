---
title: Teams 客户端发生了故障？
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030515"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="c5347-102">Teams 客户端发生了故障？</span><span class="sxs-lookup"><span data-stu-id="c5347-102">Teams client crashing?</span></span>

<span data-ttu-id="c5347-103">如果 Teams 客户端发生了故障，请尝试执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="c5347-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="c5347-104">如果使用的是 Teams 桌面应用，请[确保应用已完全更新](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)。</span><span class="sxs-lookup"><span data-stu-id="c5347-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="c5347-105">确保所有 [Office 365 URL 和地址范围](https://docs.microsoft.com/microsoftteams/connectivity-issues)都可访问。</span><span class="sxs-lookup"><span data-stu-id="c5347-105">Make sure all the [Office 365 URL's and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="c5347-106">使用管理员帐户登录，然后检查[服务运行状况仪表板](https://docs.microsoft.com/office365/enterprise/view-service-health)，以确认是否没有任何故障或服务降级。</span><span class="sxs-lookup"><span data-stu-id="c5347-106">Log in with your admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="c5347-107">最后，可以尝试清除 Teams 客户端缓存：</span><span class="sxs-lookup"><span data-stu-id="c5347-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="c5347-108">完全退出 Microsoft Teams 桌面客户端。</span><span class="sxs-lookup"><span data-stu-id="c5347-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="c5347-109">可以右键单击图标托盘中的“Teams”\*\*\*\*，然后单击“退出”\*\*\*\*，也可以运行“任务管理器”，并完全终止进程。</span><span class="sxs-lookup"><span data-stu-id="c5347-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="c5347-110">转到“文件资源管理器”，然后键入“%appdata%\Microsoft\teams”。</span><span class="sxs-lookup"><span data-stu-id="c5347-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="c5347-111">进入目录后，便会看到以下几个文件夹：</span><span class="sxs-lookup"><span data-stu-id="c5347-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="c5347-112">在“应用程序缓存”\*\*\*\* 中，转到“缓存”，然后删除“缓存”位置 (%appdata%\Microsoft\teams\application cache\cache) 中的任何文件。</span><span class="sxs-lookup"><span data-stu-id="c5347-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="c5347-113">在“Blob_storage”\*\*\*\*(%appdata%\Microsoft\teams\blob_storage) 中，删除所有文件。</span><span class="sxs-lookup"><span data-stu-id="c5347-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="c5347-114">在“缓存”\*\*\*\*(%appdata%\Microsoft\teams\Cache) 中，删除所有文件。</span><span class="sxs-lookup"><span data-stu-id="c5347-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="c5347-115">在“数据库”\*\*\*\*(%appdata%\Microsoft\teams\databases) 中，删除所有文件。</span><span class="sxs-lookup"><span data-stu-id="c5347-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="c5347-116">在“GPUCache”\*\*\*\*(%appdata%\Microsoft\teams\GPUcache) 中，删除所有文件。</span><span class="sxs-lookup"><span data-stu-id="c5347-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="c5347-117">在“IndexedDB”\*\*\*\*(%appdata%\Microsoft\teams\IndexedDB) 中，删除 .db 文件。</span><span class="sxs-lookup"><span data-stu-id="c5347-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="c5347-118">在“本地存储”\*\*\*\*(%appdata%\Microsoft\teams\Local Storage) 中，删除所有文件。</span><span class="sxs-lookup"><span data-stu-id="c5347-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="c5347-119">最后，在“tmp”\*\*\*\*(%appdata%\Microsoft\teams\tmp) 中，删除所有文件。</span><span class="sxs-lookup"><span data-stu-id="c5347-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="c5347-120">重启 Teams 客户端。</span><span class="sxs-lookup"><span data-stu-id="c5347-120">Restart your Teams client.</span></span>
