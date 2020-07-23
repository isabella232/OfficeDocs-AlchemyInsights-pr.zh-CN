---
title: 密码同步疑难解答
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387867"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="e610e-102">密码同步疑难解答</span><span class="sxs-lookup"><span data-stu-id="e610e-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="e610e-103">若要解决密码同步问题，请使用此 AAD Connect 故障排除任务开始，以确定密码未同步的原因。</span><span class="sxs-lookup"><span data-stu-id="e610e-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="e610e-104">若要开始，请转到[管理直接同步](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)。</span><span class="sxs-lookup"><span data-stu-id="e610e-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="e610e-105">在 Azure AD Connect 服务器上打开一个新的 Windows PowerShell 会话，然后选择 "**以管理员身份运行**" 选项。</span><span class="sxs-lookup"><span data-stu-id="e610e-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="e610e-106">运行 ExecutionPolicy RemoteSigned 或 ExecutionPolicy 不受限制的设置。</span><span class="sxs-lookup"><span data-stu-id="e610e-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="e610e-107">启动 Azure AD Connect 向导。</span><span class="sxs-lookup"><span data-stu-id="e610e-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="e610e-108">转到 "其他任务" 页**Troubleshoot**>  >  **下一步**解决问题。</span><span class="sxs-lookup"><span data-stu-id="e610e-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="e610e-109">选择 "**启动**" 以打开 PowerShell 故障排除菜单。</span><span class="sxs-lookup"><span data-stu-id="e610e-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="e610e-110">选择 "**密码同步疑难解答**"。</span><span class="sxs-lookup"><span data-stu-id="e610e-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="e610e-111">问题通常是不会为特定用户帐户同步密码。</span><span class="sxs-lookup"><span data-stu-id="e610e-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="e610e-112">**备注**如果上一次成功的密码同步曾经过一次，则密码同步将失败。</span><span class="sxs-lookup"><span data-stu-id="e610e-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="e610e-113">有关疑难解答密码同步的更多帮助，请参阅[密码哈希同步与 AZURE AD Connect Sync 疑难解答](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)。</span><span class="sxs-lookup"><span data-stu-id="e610e-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>