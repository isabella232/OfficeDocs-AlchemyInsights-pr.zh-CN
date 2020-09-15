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
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695169"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="7ad4e-102">解决 Microsoft 365 应用程序 "计算机的受信任的平台模块无法正常运行" 消息</span><span class="sxs-lookup"><span data-stu-id="7ad4e-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="7ad4e-103">若要修复此错误，请使用以下步骤：</span><span class="sxs-lookup"><span data-stu-id="7ad4e-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="7ad4e-104">安装最新的 [Windows](https://support.microsoft.com/help/4027667/windows-10-update) 和 [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)更新。</span><span class="sxs-lookup"><span data-stu-id="7ad4e-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="7ad4e-105">使用 Windows 凭据管理器[清除 Office 凭据](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)。</span><span class="sxs-lookup"><span data-stu-id="7ad4e-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="7ad4e-106">**注意：** Office 2016 的注册表路径已更改为16.0。</span><span class="sxs-lookup"><span data-stu-id="7ad4e-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="7ad4e-107"> (Ex： \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="7ad4e-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="7ad4e-108">尝试 [用户恢复过程](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) 以修复受信任的平台模块 (TPM) 故障。</span><span class="sxs-lookup"><span data-stu-id="7ad4e-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="7ad4e-109">使用以下步骤设置 EnableADAL = 0：</span><span class="sxs-lookup"><span data-stu-id="7ad4e-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="7ad4e-110">右键单击 Windows "开始" 按钮，选择 " **运行**"，键入 " **regedit**"，然后选择 **"确定"**。</span><span class="sxs-lookup"><span data-stu-id="7ad4e-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="7ad4e-111">选择 **"是"** 以允许注册表编辑器对你的设备进行更改。</span><span class="sxs-lookup"><span data-stu-id="7ad4e-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="7ad4e-112">在注册表编辑器中，将 **EnableADAL** 的 DWORD 值添加到 HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity. 下的设置为 **0** 。</span><span class="sxs-lookup"><span data-stu-id="7ad4e-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="7ad4e-113">有关详细信息，请参阅在 [Windows 10 上更新到 Office 2016 生成16.0.7967 后登录中的连接问题](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)。</span><span class="sxs-lookup"><span data-stu-id="7ad4e-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>