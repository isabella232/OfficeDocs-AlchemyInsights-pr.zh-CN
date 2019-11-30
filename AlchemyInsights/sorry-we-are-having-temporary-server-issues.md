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
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627980"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="e356a-102">修复 Office 应用程序 "很抱歉，出现临时服务器问题" 消息</span><span class="sxs-lookup"><span data-stu-id="e356a-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="e356a-103">如果您收到此消息，请尝试以下操作：</span><span class="sxs-lookup"><span data-stu-id="e356a-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="e356a-104">检查防火墙、防病毒软件和代理设置以确认他们不会阻止对 Office 应用程序的 Internet 访问。</span><span class="sxs-lookup"><span data-stu-id="e356a-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="e356a-105">请参阅[Office 365 url 和 IP 地址范围](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。</span><span class="sxs-lookup"><span data-stu-id="e356a-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="e356a-106">转到 "**开始** > " "**运行**"，然后键入**services.msc**。</span><span class="sxs-lookup"><span data-stu-id="e356a-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="e356a-107">确保以下服务全部运行：</span><span class="sxs-lookup"><span data-stu-id="e356a-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="e356a-108">网络连接设备自动设置</span><span class="sxs-lookup"><span data-stu-id="e356a-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="e356a-109">网络列表服务</span><span class="sxs-lookup"><span data-stu-id="e356a-109">Network List Service</span></span>
    - <span data-ttu-id="e356a-110">网络位置感知</span><span class="sxs-lookup"><span data-stu-id="e356a-110">Network Location Awareness</span></span>
    - <span data-ttu-id="e356a-111">Windows 事件日志</span><span class="sxs-lookup"><span data-stu-id="e356a-111">Windows Event Log</span></span>

<span data-ttu-id="e356a-112">如果其中一项服务未在运行，请尝试启动它。</span><span class="sxs-lookup"><span data-stu-id="e356a-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="e356a-113">如果您在启动服务时遇到问题，请通过使用提升的权限打开命令提示符来运行以下命令：</span><span class="sxs-lookup"><span data-stu-id="e356a-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="e356a-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="e356a-114">**sfc /scannow**</span></span>

<span data-ttu-id="e356a-115">此命令完成后，重新启动计算机。</span><span class="sxs-lookup"><span data-stu-id="e356a-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="e356a-116">有关详细信息，请参阅["很抱歉，我们无法连接到你的帐户。在从 Office 365 激活 Office 时，请稍后重试 "错误"](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)。</span><span class="sxs-lookup"><span data-stu-id="e356a-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>