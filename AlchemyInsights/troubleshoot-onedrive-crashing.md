---
title: OneDrive 崩溃疑难解答
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664988"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="2c7f4-102">OneDrive 崩溃疑难解答</span><span class="sxs-lookup"><span data-stu-id="2c7f4-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="2c7f4-103">如果 OneDrive 反复崩溃，请尝试以下故障排除步骤：</span><span class="sxs-lookup"><span data-stu-id="2c7f4-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="2c7f4-104">**确保未设置注册表项：**</span><span class="sxs-lookup"><span data-stu-id="2c7f4-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="2c7f4-105">打开注册表编辑器，导航至 HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="2c7f4-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="2c7f4-106">如果 DisableFileSyncNGSC 存在，并且设置为 1，请打开该项，将值更改为 0。</span><span class="sxs-lookup"><span data-stu-id="2c7f4-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="2c7f4-107">通过转到“开始”，手动启动 OneDrive，</span><span class="sxs-lookup"><span data-stu-id="2c7f4-107">Manually launch OneDrive by going to Start</span></span> ![按 Windows 徽标键](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="2c7f4-109">在搜索框中键入 OneDrive，然后单击 OneDrive 桌面应用程序。</span><span class="sxs-lookup"><span data-stu-id="2c7f4-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="2c7f4-110">**重置 OneDrive：**</span><span class="sxs-lookup"><span data-stu-id="2c7f4-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="2c7f4-111">注意：</span><span class="sxs-lookup"><span data-stu-id="2c7f4-111">Notes:</span></span>

- <span data-ttu-id="2c7f4-112">重置 OneDrive 将断开所有现有同步连接（如果设置了个人 OneDrive 也会断开其连接）。</span><span class="sxs-lookup"><span data-stu-id="2c7f4-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="2c7f4-113">在计算机上重置 OneDrive 不会丢失文件或数据。</span><span class="sxs-lookup"><span data-stu-id="2c7f4-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="2c7f4-114">**重置 OneDrive：**</span><span class="sxs-lookup"><span data-stu-id="2c7f4-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="2c7f4-115">按 Windows 徽标键和 “R”打开“运行”对话框。</span><span class="sxs-lookup"><span data-stu-id="2c7f4-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="2c7f4-116">键入 %localappdata%\Microsoft\OneDrive\onedrive.exe /reset 并按“确定”。</span><span class="sxs-lookup"><span data-stu-id="2c7f4-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="2c7f4-117">“命令”窗口可能会一闪而过。</span><span class="sxs-lookup"><span data-stu-id="2c7f4-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="2c7f4-118">通过转到“开始”，手动启动 OneDrive，</span><span class="sxs-lookup"><span data-stu-id="2c7f4-118">Manually launch OneDrive by going to Start</span></span> ![按 Windows 徽标键](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="2c7f4-120">在搜索框中键入 OneDrive，然后单击 OneDrive 桌面应用程序。</span><span class="sxs-lookup"><span data-stu-id="2c7f4-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="2c7f4-121">注意：</span><span class="sxs-lookup"><span data-stu-id="2c7f4-121">Notes:</span></span>

- <span data-ttu-id="2c7f4-122">如果在重置之前选择了仅同步部分文件夹，则同步完成之后将需要再次执行该操作。</span><span class="sxs-lookup"><span data-stu-id="2c7f4-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="2c7f4-123">有关详细信息，请参阅 [选择要同步到计算机的 OneDrive 文件夹](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) 。</span><span class="sxs-lookup"><span data-stu-id="2c7f4-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="2c7f4-124">您需要为您的个人 OneDrive 和 OneDrive for Business 完成此操作。</span><span class="sxs-lookup"><span data-stu-id="2c7f4-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>