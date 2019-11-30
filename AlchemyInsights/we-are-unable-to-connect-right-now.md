---
title: 激活问题-我们现在无法连接
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628232"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="0b6eb-102">修复 Office 应用程序 "现在无法连接" 消息</span><span class="sxs-lookup"><span data-stu-id="0b6eb-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="0b6eb-103">如果您收到此消息，请尝试以下操作：</span><span class="sxs-lookup"><span data-stu-id="0b6eb-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="0b6eb-104">检查防火墙、防病毒软件和代理设置以确认他们不会阻止对 Office 应用程序的 Internet 访问。</span><span class="sxs-lookup"><span data-stu-id="0b6eb-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="0b6eb-105">请参阅[Office 365 url 和 IP 地址范围](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。</span><span class="sxs-lookup"><span data-stu-id="0b6eb-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="0b6eb-106">转到 "**开始** > " "**运行**"，然后键入**services.msc**。</span><span class="sxs-lookup"><span data-stu-id="0b6eb-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="0b6eb-107">确保以下服务全部运行：</span><span class="sxs-lookup"><span data-stu-id="0b6eb-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="0b6eb-108">网络连接设备自动设置</span><span class="sxs-lookup"><span data-stu-id="0b6eb-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="0b6eb-109">网络列表服务</span><span class="sxs-lookup"><span data-stu-id="0b6eb-109">Network List Service</span></span>
    - <span data-ttu-id="0b6eb-110">网络位置感知</span><span class="sxs-lookup"><span data-stu-id="0b6eb-110">Network Location Awareness</span></span>
    - <span data-ttu-id="0b6eb-111">Windows 事件日志</span><span class="sxs-lookup"><span data-stu-id="0b6eb-111">Windows Event Log</span></span>

<span data-ttu-id="0b6eb-112">如果其中一项服务未在运行，请尝试启动它。</span><span class="sxs-lookup"><span data-stu-id="0b6eb-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="0b6eb-113">如果您在启动服务时遇到问题，请通过使用提升的权限打开命令提示符来运行以下命令：</span><span class="sxs-lookup"><span data-stu-id="0b6eb-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="0b6eb-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="0b6eb-114">**sfc /scannow**</span></span>

<span data-ttu-id="0b6eb-115">此命令完成后，重新启动计算机。</span><span class="sxs-lookup"><span data-stu-id="0b6eb-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="0b6eb-116">有关详细信息，请参阅["很抱歉，我们无法连接到你的帐户。在从 Office 365 激活 Office 时，请稍后重试 "错误"](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)。</span><span class="sxs-lookup"><span data-stu-id="0b6eb-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>