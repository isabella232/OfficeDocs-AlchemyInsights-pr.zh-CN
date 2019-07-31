---
title: 登录 Office 应用程序时出现问题
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938143"
---
# <a name="blank-sign-in-screen-in-office-apps"></a><span data-ttu-id="1c8a3-102">Office 应用中的空白登录屏幕</span><span class="sxs-lookup"><span data-stu-id="1c8a3-102">Blank sign-in screen in Office apps</span></span>

<span data-ttu-id="1c8a3-103">若要解决此问题, 请尝试以下操作:</span><span class="sxs-lookup"><span data-stu-id="1c8a3-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="1c8a3-104">安装最新的[Windows](https://support.microsoft.com/help/4027667/windows-10-update)和[Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)更新。</span><span class="sxs-lookup"><span data-stu-id="1c8a3-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="1c8a3-105">重置 internet Explorer 选项: 转到 "**工具** > " "**internet 选项** > "**高级** > **重置 internet Explorer 设置**(请注意, 将丢失自定义设置), 然后再次尝试登录到 Office。</span><span class="sxs-lookup"><span data-stu-id="1c8a3-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="1c8a3-106">禁用 Windows Defender 应用程序防护 (WDAG) 或任何类似的防火墙或反病毒程序:</span><span class="sxs-lookup"><span data-stu-id="1c8a3-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="1c8a3-107">在 "控制面板" 中, 转到 "**程序**", 然后选择 **"打开或关闭 Windows 功能"**。</span><span class="sxs-lookup"><span data-stu-id="1c8a3-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="1c8a3-108">如果启用了 Windows Defender 应用程序防护, 请尝试禁用它。</span><span class="sxs-lookup"><span data-stu-id="1c8a3-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="1c8a3-109">**注意:** 您可能需要重新启动计算机。</span><span class="sxs-lookup"><span data-stu-id="1c8a3-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="1c8a3-110">确保任何应用程序或防火墙/反病毒程序都不会阻止 BrokerPlugin [AAD WAM 插件](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1)。</span><span class="sxs-lookup"><span data-stu-id="1c8a3-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="1c8a3-111">使用 Windows 凭据管理器[清除 Office 凭据](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)。</span><span class="sxs-lookup"><span data-stu-id="1c8a3-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="1c8a3-112">**注意:** Office 2016 的注册表路径已更改为16.0。</span><span class="sxs-lookup"><span data-stu-id="1c8a3-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="1c8a3-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="1c8a3-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="1c8a3-114">有关详细信息, 请参阅在[Windows 10 上更新到 Office 2016 生成16.0.7967 后登录中的连接问题](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)。</span><span class="sxs-lookup"><span data-stu-id="1c8a3-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>