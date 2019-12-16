---
title: 修复 OneDrive 中的0x8004de40 错误
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052027"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="a0e01-102">修复 OneDrive 中的0x8004de40 错误</span><span class="sxs-lookup"><span data-stu-id="a0e01-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="a0e01-103">如果您收到 OneDrive 的0x8004de40 错误：</span><span class="sxs-lookup"><span data-stu-id="a0e01-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="a0e01-104">在连接到您的 Acitve Directory 域时，重新启动受影响的计算机。</span><span class="sxs-lookup"><span data-stu-id="a0e01-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="a0e01-105">如果重新启动不能解决问题，请从 Azure AD 中脱离并重新加入设备。</span><span class="sxs-lookup"><span data-stu-id="a0e01-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="a0e01-106">**注意**：在执行这些步骤时，您应在公司网络上。</span><span class="sxs-lookup"><span data-stu-id="a0e01-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="a0e01-107">如果无法连接到公司基础结构（例如出差时），请不要执行这些步骤。</span><span class="sxs-lookup"><span data-stu-id="a0e01-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="a0e01-108">打开提升的命令提示符。</span><span class="sxs-lookup"><span data-stu-id="a0e01-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="a0e01-109">若要打开提升的命令提示符，请单击 "**开始**"，右键单击 "**命令提示符**"，然后单击 "**以管理员身份运行**"。</span><span class="sxs-lookup"><span data-stu-id="a0e01-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="a0e01-110">键入*dsregcmd/leave* ，然后按**enter**。</span><span class="sxs-lookup"><span data-stu-id="a0e01-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="a0e01-111">完成后，键入*dsregcmd/join* ，然后按**enter**。</span><span class="sxs-lookup"><span data-stu-id="a0e01-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="a0e01-112">完成后，关闭命令提示符。</span><span class="sxs-lookup"><span data-stu-id="a0e01-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="a0e01-113">重新启动计算机，然后登录到 OneDrive。</span><span class="sxs-lookup"><span data-stu-id="a0e01-113">Reboot the computer, and log into OneDrive.</span></span>