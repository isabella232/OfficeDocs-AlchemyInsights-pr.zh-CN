---
title: 修复 Microsoft 365 应用 抱歉，我们收到临时服务器问题消息
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
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835261"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="80e32-102">修复 Microsoft 365 应用"抱歉，我们遇到临时服务器问题"消息</span><span class="sxs-lookup"><span data-stu-id="80e32-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="80e32-103">如果收到此消息，请尝试执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="80e32-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="80e32-104">请检查防火墙、防病毒软件和代理设置，确认它们不会阻止 Internet 访问 Microsoft 365 应用。</span><span class="sxs-lookup"><span data-stu-id="80e32-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="80e32-105">请参阅 [URL 和 IP 地址范围](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。</span><span class="sxs-lookup"><span data-stu-id="80e32-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="80e32-106">转到"**开始**  >  **运行**"，然后键入 **services.msc。**</span><span class="sxs-lookup"><span data-stu-id="80e32-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="80e32-107">确保以下服务均在运行：</span><span class="sxs-lookup"><span data-stu-id="80e32-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="80e32-108">网络连接设备自动设置</span><span class="sxs-lookup"><span data-stu-id="80e32-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="80e32-109">网络列表服务</span><span class="sxs-lookup"><span data-stu-id="80e32-109">Network List Service</span></span>
    - <span data-ttu-id="80e32-110">网络位置感知</span><span class="sxs-lookup"><span data-stu-id="80e32-110">Network Location Awareness</span></span>
    - <span data-ttu-id="80e32-111">Windows 事件日志</span><span class="sxs-lookup"><span data-stu-id="80e32-111">Windows Event Log</span></span>

<span data-ttu-id="80e32-112">如果其中一个服务未运行，请尝试启动它。</span><span class="sxs-lookup"><span data-stu-id="80e32-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="80e32-113">如果在启动服务时遇到问题，请通过打开具有提升的权限的命令提示符来运行以下命令：</span><span class="sxs-lookup"><span data-stu-id="80e32-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="80e32-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="80e32-114">**sfc /scannow**</span></span>

<span data-ttu-id="80e32-115">此命令完成后，重新启动计算机。</span><span class="sxs-lookup"><span data-stu-id="80e32-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="80e32-116">有关详细信息，请参阅["抱歉，无法连接到您的帐户。请在激活 时重试"错误"。](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="80e32-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>