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
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938144"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="466a2-102">修复 Office 应用程序 "计算机的受信任的平台模块未正常运行" 消息</span><span class="sxs-lookup"><span data-stu-id="466a2-102">Fixing the Office apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="466a2-103">若要修复此错误, 请尝试以下操作:</span><span class="sxs-lookup"><span data-stu-id="466a2-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="466a2-104">安装最新的[Windows](https://support.microsoft.com/help/4027667/windows-10-update)和[Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)更新。</span><span class="sxs-lookup"><span data-stu-id="466a2-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="466a2-105">使用 Windows 凭据管理器[清除 Office 凭据](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)。</span><span class="sxs-lookup"><span data-stu-id="466a2-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="466a2-106">**注意:** Office 2016 的注册表路径已更改为16.0。</span><span class="sxs-lookup"><span data-stu-id="466a2-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="466a2-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="466a2-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="466a2-108">尝试[用户恢复过程](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2)以修复受信任的平台模块 (TPM) 故障。</span><span class="sxs-lookup"><span data-stu-id="466a2-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="466a2-109">使用以下步骤设置 EnableADAL = 0:</span><span class="sxs-lookup"><span data-stu-id="466a2-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="466a2-110">右键单击 Windows "开始" 按钮, 选择 "**运行**", 键入 " **regedit**", 然后选择 **"确定"**。</span><span class="sxs-lookup"><span data-stu-id="466a2-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="466a2-111">选择 **"是"** 以允许注册表编辑器对你的设备进行更改。</span><span class="sxs-lookup"><span data-stu-id="466a2-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="466a2-112">在注册表编辑器中, 将**EnableADAL**的 DWORD 值添加到 HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity. 下的设置为**0** 。</span><span class="sxs-lookup"><span data-stu-id="466a2-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="466a2-113">有关详细信息, 请参阅在[Windows 10 上更新到 Office 2016 生成16.0.7967 后登录中的连接问题](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)。</span><span class="sxs-lookup"><span data-stu-id="466a2-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>