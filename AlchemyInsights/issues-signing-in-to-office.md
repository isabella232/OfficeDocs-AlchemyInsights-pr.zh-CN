---
title: 登录到 Microsoft 365 应用程序时出现问题
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
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695277"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="d29ab-102">Microsoft 365 应用中的空白登录屏幕</span><span class="sxs-lookup"><span data-stu-id="d29ab-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="d29ab-103">若要解决此问题，请尝试以下操作：</span><span class="sxs-lookup"><span data-stu-id="d29ab-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="d29ab-104">安装最新的 [Windows](https://support.microsoft.com/help/4027667/windows-10-update) 和 [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)更新。</span><span class="sxs-lookup"><span data-stu-id="d29ab-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="d29ab-105">重置 internet Explorer 选项：转到 "**工具**" "  >  **internet 选项**"  >  **高级**  >  **重置 internet Explorer 设置** (请注意，您将丢失自定义设置) ，然后再次尝试登录 Office。</span><span class="sxs-lookup"><span data-stu-id="d29ab-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="d29ab-106">禁用 Windows Defender 应用程序防护 (WDAG) 或任何类似的防火墙或反病毒程序：</span><span class="sxs-lookup"><span data-stu-id="d29ab-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="d29ab-107">在 "控制面板" 中，转到 " **程序**"，然后选择 **"打开或关闭 Windows 功能"**。</span><span class="sxs-lookup"><span data-stu-id="d29ab-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="d29ab-108">如果启用了 Windows Defender 应用程序防护，请尝试禁用它。</span><span class="sxs-lookup"><span data-stu-id="d29ab-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="d29ab-109">**注意：** 您可能需要重新启动计算机。</span><span class="sxs-lookup"><span data-stu-id="d29ab-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="d29ab-110">确保任何应用程序或防火墙/反病毒程序都不会阻止 BrokerPlugin [AAD WAM 插件](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) 。</span><span class="sxs-lookup"><span data-stu-id="d29ab-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="d29ab-111">使用 Windows 凭据管理器[清除 Office 凭据](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)。</span><span class="sxs-lookup"><span data-stu-id="d29ab-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="d29ab-112">**注意：** Office 2016 的注册表路径已更改为16.0。</span><span class="sxs-lookup"><span data-stu-id="d29ab-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="d29ab-113"> (Ex： \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="d29ab-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="d29ab-114">有关详细信息，请参阅在 [Windows 10 上更新到 Office 2016 生成16.0.7967 后登录中的连接问题](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)。</span><span class="sxs-lookup"><span data-stu-id="d29ab-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>