---
title: 0x8004de40 OneDrive 时出现错误
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
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813642"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="6ce5f-102">0x8004de40 OneDrive 时出现错误</span><span class="sxs-lookup"><span data-stu-id="6ce5f-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="6ce5f-103">如果在登录 OneDrive **0x8004de40** 收到错误消息，请重启计算机，同时连接到工作或学校域。</span><span class="sxs-lookup"><span data-stu-id="6ce5f-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="6ce5f-104">如果在重新启动后收到此错误，请在连接到工作或学校域时尝试以下操作：</span><span class="sxs-lookup"><span data-stu-id="6ce5f-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="6ce5f-105">单击"开始"，在搜索框中键入 **cmd** 或命令提示符，右键单击命令提示符应用，然后选择"以 **管理员角色运行"。**</span><span class="sxs-lookup"><span data-stu-id="6ce5f-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="6ce5f-106">如果系统提示你输入管理员密码或进行确认，请键入密码，或单击"允许 **"。**</span><span class="sxs-lookup"><span data-stu-id="6ce5f-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="6ce5f-107">在命令提示符窗口中，键入 **dsregcmd /leave**  并等待命令完成。</span><span class="sxs-lookup"><span data-stu-id="6ce5f-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="6ce5f-108">然后键入 **dsregcmd /join** 并等待命令完成。</span><span class="sxs-lookup"><span data-stu-id="6ce5f-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="6ce5f-109">重新启动计算机。</span><span class="sxs-lookup"><span data-stu-id="6ce5f-109">Reboot your computer.</span></span>
