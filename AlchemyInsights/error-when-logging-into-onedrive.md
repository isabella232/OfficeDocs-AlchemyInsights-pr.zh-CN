---
title: 启动 OneDrive 时出现0x8004de40 错误
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/30/2020
ms.locfileid: "48815967"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="d7f23-102">启动 OneDrive 时出现0x8004de40 错误</span><span class="sxs-lookup"><span data-stu-id="d7f23-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="d7f23-103">如果你在登录 OneDrive 时收到错误 **0x8004de40** ，请在连接到你的工作或学校域时重新启动计算机。</span><span class="sxs-lookup"><span data-stu-id="d7f23-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="d7f23-104">如果重新启动后收到此错误，请在连接到工作或学校域时尝试以下操作：</span><span class="sxs-lookup"><span data-stu-id="d7f23-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="d7f23-105">单击 "开始"，在 "搜索" 框中键入 **cmd** 或 **命令提示符**  ，右键单击 "命令提示符" 应用，然后选择 "  **以管理员身份运行** "。</span><span class="sxs-lookup"><span data-stu-id="d7f23-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="d7f23-106">如果系统提示您输入管理员密码或进行确认，请键入密码或单击 " **允许** "。</span><span class="sxs-lookup"><span data-stu-id="d7f23-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="d7f23-107">在命令提示符窗口中，键入 **dsregcmd/leave**  并等待该命令完成。</span><span class="sxs-lookup"><span data-stu-id="d7f23-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="d7f23-108">然后键入 **dsregcmd/join** 并等待该命令完成。</span><span class="sxs-lookup"><span data-stu-id="d7f23-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="d7f23-109">重新启动计算机。</span><span class="sxs-lookup"><span data-stu-id="d7f23-109">Reboot your computer.</span></span>
