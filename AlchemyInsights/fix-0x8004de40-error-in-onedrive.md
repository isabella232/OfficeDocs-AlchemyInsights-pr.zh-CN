---
title: 修复0x8004de40 OneDrive 中的错误
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649738"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="3566b-102">修复0x8004de40 OneDrive 中的错误</span><span class="sxs-lookup"><span data-stu-id="3566b-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="3566b-103">如果你运行的是 Windows 7 并收到此错误，请更新以在 Windows 的 WinHTTP 中启用 [TLS 1.1 和 TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)作为默认安全协议。</span><span class="sxs-lookup"><span data-stu-id="3566b-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="3566b-104">如果运行的是 Windows 10，并且收到 OneDrive 0x8004de40错误：</span><span class="sxs-lookup"><span data-stu-id="3566b-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="3566b-105">连接到 Acitve 目录域时重新启动受影响的计算机。</span><span class="sxs-lookup"><span data-stu-id="3566b-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="3566b-106">如果重启无法解决问题，请从 Azure AD 中取消加入设备并重新加入设备。</span><span class="sxs-lookup"><span data-stu-id="3566b-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="3566b-107">**注意**：执行这些步骤时，你应该位于企业网络上。</span><span class="sxs-lookup"><span data-stu-id="3566b-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="3566b-108">例如，未连接到公司基础结构或 (，请不要执行这些步骤) 。</span><span class="sxs-lookup"><span data-stu-id="3566b-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="3566b-109">通过选择"开始"打开提升的命令提示符，右键单击"**命令提示符**"，然后选择"以 **管理员角色运行"。**</span><span class="sxs-lookup"><span data-stu-id="3566b-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="3566b-110">键入 *dsregcmd /leave，* 然后按 **Enter。**</span><span class="sxs-lookup"><span data-stu-id="3566b-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="3566b-111">完成后，键入 *dsregcmd /join* 并按 **Enter。**</span><span class="sxs-lookup"><span data-stu-id="3566b-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="3566b-112">完成后，关闭命令提示符。</span><span class="sxs-lookup"><span data-stu-id="3566b-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="3566b-113">重新启动计算机，并登录到 OneDrive。</span><span class="sxs-lookup"><span data-stu-id="3566b-113">Reboot the computer, and log into OneDrive.</span></span>