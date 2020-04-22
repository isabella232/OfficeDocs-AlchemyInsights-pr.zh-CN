---
title: 修复 Office 应用程序抱歉，我们暂时出现服务器问题
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764107"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="2249a-102">修复 Office 应用程序 "很抱歉，出现临时服务器问题" 消息</span><span class="sxs-lookup"><span data-stu-id="2249a-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="2249a-103">如果您收到此消息，请尝试以下操作：</span><span class="sxs-lookup"><span data-stu-id="2249a-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="2249a-104">检查防火墙、防病毒软件和代理设置以确认他们不会阻止对 Office 应用程序的 Internet 访问。</span><span class="sxs-lookup"><span data-stu-id="2249a-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="2249a-105">请参阅[url 和 IP 地址范围](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。</span><span class="sxs-lookup"><span data-stu-id="2249a-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="2249a-106">转到 "**开始** > " "**运行**"，然后键入**services.msc**。</span><span class="sxs-lookup"><span data-stu-id="2249a-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="2249a-107">确保以下服务全部运行：</span><span class="sxs-lookup"><span data-stu-id="2249a-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="2249a-108">网络连接设备自动设置</span><span class="sxs-lookup"><span data-stu-id="2249a-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="2249a-109">网络列表服务</span><span class="sxs-lookup"><span data-stu-id="2249a-109">Network List Service</span></span>
    - <span data-ttu-id="2249a-110">网络位置感知</span><span class="sxs-lookup"><span data-stu-id="2249a-110">Network Location Awareness</span></span>
    - <span data-ttu-id="2249a-111">Windows 事件日志</span><span class="sxs-lookup"><span data-stu-id="2249a-111">Windows Event Log</span></span>

<span data-ttu-id="2249a-112">如果其中一项服务未在运行，请尝试启动它。</span><span class="sxs-lookup"><span data-stu-id="2249a-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="2249a-113">如果您在启动服务时遇到问题，请通过使用提升的权限打开命令提示符来运行以下命令：</span><span class="sxs-lookup"><span data-stu-id="2249a-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="2249a-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="2249a-114">**sfc /scannow**</span></span>

<span data-ttu-id="2249a-115">此命令完成后，重新启动计算机。</span><span class="sxs-lookup"><span data-stu-id="2249a-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="2249a-116">有关详细信息，请参阅["很抱歉，我们无法连接到你的帐户。请稍后在激活时重试 "错误"](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)。</span><span class="sxs-lookup"><span data-stu-id="2249a-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>