---
title: 登录 Microsoft 365 应用时的问题
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
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833021"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="62c03-102">Microsoft 365 应用中的空白登录屏幕</span><span class="sxs-lookup"><span data-stu-id="62c03-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="62c03-103">若要解决此问题，请尝试执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="62c03-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="62c03-104">安装 Windows [和](https://support.microsoft.com/help/4027667/windows-10-update) Office 的最新 [更新](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)。</span><span class="sxs-lookup"><span data-stu-id="62c03-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="62c03-105">重置Internet Explorer选项： 转到工具Internet 选项 高级重置 Internet Explorer 设置 (请注意，你将丢失自定义设置  >    >    >  ) ，然后再次尝试登录 Office。</span><span class="sxs-lookup"><span data-stu-id="62c03-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="62c03-106">禁用 WINDOWS DEFENDER 应用程序防护 (WDAG) 或类似防火墙或防病毒程序：</span><span class="sxs-lookup"><span data-stu-id="62c03-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="62c03-107">在"控制面板"中，转到"**程序**"，然后选择"**打开或关闭 Windows 功能"。**</span><span class="sxs-lookup"><span data-stu-id="62c03-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="62c03-108">如果Windows Defender应用程序防护，请尝试禁用它。</span><span class="sxs-lookup"><span data-stu-id="62c03-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="62c03-109">**注意：** 您可能需要重新启动计算机。</span><span class="sxs-lookup"><span data-stu-id="62c03-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="62c03-110">确保 Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) 插件未被任何应用程序或防火墙/防病毒程序阻止。</span><span class="sxs-lookup"><span data-stu-id="62c03-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="62c03-111">[使用 Windows 凭据管理器](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) 清除 Office 凭据。</span><span class="sxs-lookup"><span data-stu-id="62c03-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="62c03-112">**注意：** Office 2016 的注册表路径已更改为 16.0。</span><span class="sxs-lookup"><span data-stu-id="62c03-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="62c03-113"> (：\Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="62c03-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="62c03-114">有关详细信息，请参阅 [Windows 10 上的 Office 2016 内部版本 16.0.7967](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)更新后登录的连接问题。</span><span class="sxs-lookup"><span data-stu-id="62c03-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>