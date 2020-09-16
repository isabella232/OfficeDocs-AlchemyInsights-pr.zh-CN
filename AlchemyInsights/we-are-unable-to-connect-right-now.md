---
title: 激活问题-我们现在无法连接
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
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725973"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="0f7b2-102">修复 Microsoft 365 应用程序 "当前无法连接" 消息</span><span class="sxs-lookup"><span data-stu-id="0f7b2-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="0f7b2-103">如果您收到此消息，请尝试以下操作：</span><span class="sxs-lookup"><span data-stu-id="0f7b2-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="0f7b2-104">检查你的防火墙、防病毒软件和代理设置以确认他们没有阻止对 Microsoft 365 应用的 Internet 访问。</span><span class="sxs-lookup"><span data-stu-id="0f7b2-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="0f7b2-105">请参阅 [Microsoft url 和 IP 地址范围](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。</span><span class="sxs-lookup"><span data-stu-id="0f7b2-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="0f7b2-106">转到 "**开始**  >  " "**运行**"，然后键入**services.msc**。</span><span class="sxs-lookup"><span data-stu-id="0f7b2-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="0f7b2-107">确保以下服务全部运行：</span><span class="sxs-lookup"><span data-stu-id="0f7b2-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="0f7b2-108">网络连接设备自动设置</span><span class="sxs-lookup"><span data-stu-id="0f7b2-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="0f7b2-109">网络列表服务</span><span class="sxs-lookup"><span data-stu-id="0f7b2-109">Network List Service</span></span>
    - <span data-ttu-id="0f7b2-110">网络位置感知</span><span class="sxs-lookup"><span data-stu-id="0f7b2-110">Network Location Awareness</span></span>
    - <span data-ttu-id="0f7b2-111">Windows 事件日志</span><span class="sxs-lookup"><span data-stu-id="0f7b2-111">Windows Event Log</span></span>

<span data-ttu-id="0f7b2-112">如果其中一项服务未在运行，请尝试启动它。</span><span class="sxs-lookup"><span data-stu-id="0f7b2-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="0f7b2-113">如果您在启动服务时遇到问题，请通过使用提升的权限打开命令提示符来运行以下命令：</span><span class="sxs-lookup"><span data-stu-id="0f7b2-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="0f7b2-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="0f7b2-114">**sfc /scannow**</span></span>

<span data-ttu-id="0f7b2-115">此命令完成后，重新启动计算机。</span><span class="sxs-lookup"><span data-stu-id="0f7b2-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="0f7b2-116">有关详细信息，请参阅 ["很抱歉，我们无法连接到你的帐户。在从 Microsoft 365 激活 Office 时，请稍后重试 "错误"](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)。</span><span class="sxs-lookup"><span data-stu-id="0f7b2-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>