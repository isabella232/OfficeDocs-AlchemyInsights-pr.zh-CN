---
title: 登录 Microsoft 365 应用时的问题
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
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709096"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="94fc2-102">修复 Microsoft 365 应用"计算机的受信任平台模块无法正常工作"消息</span><span class="sxs-lookup"><span data-stu-id="94fc2-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="94fc2-103">若要修复此错误，请使用以下步骤：</span><span class="sxs-lookup"><span data-stu-id="94fc2-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="94fc2-104">安装 Windows [和](https://support.microsoft.com/help/4027667/windows-10-update) Office 的最新 [更新](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)。</span><span class="sxs-lookup"><span data-stu-id="94fc2-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="94fc2-105">[使用 Windows 凭据管理器](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) 清除 Office 凭据。</span><span class="sxs-lookup"><span data-stu-id="94fc2-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="94fc2-106">**注意：** Office 2016 的注册表路径已更改为 16.0。</span><span class="sxs-lookup"><span data-stu-id="94fc2-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="94fc2-107"> (：\Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="94fc2-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="94fc2-108">尝试 [用户恢复过程以](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) 修复 TPM 故障 (受信任的) 模块。</span><span class="sxs-lookup"><span data-stu-id="94fc2-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="94fc2-109">使用以下步骤设置 EnableADAL = 0：</span><span class="sxs-lookup"><span data-stu-id="94fc2-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="94fc2-110">右键单击 Windows"开始"按钮，选择"**运行**"，键入 **regedit，** 然后选择 **"确定"。**</span><span class="sxs-lookup"><span data-stu-id="94fc2-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="94fc2-111">选择 **"** 是"以允许注册表编辑器对设备进行更改。</span><span class="sxs-lookup"><span data-stu-id="94fc2-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="94fc2-112">在注册表编辑器中，添加 **EnableADAL** 的 DWORD 值，在"注册表编辑器"下将设置为 **0** HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity。</span><span class="sxs-lookup"><span data-stu-id="94fc2-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="94fc2-113">有关详细信息，请参阅 [Windows 10 上的 Office 2016 内部版本 16.0.7967](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)更新后登录的连接问题。</span><span class="sxs-lookup"><span data-stu-id="94fc2-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>