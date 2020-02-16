---
title: 修复 Office 应用你的帐户处于错误状态消息
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969253"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="722a6-102">修复 Office 应用程序 "你的帐户处于错误状态" 错误</span><span class="sxs-lookup"><span data-stu-id="722a6-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="722a6-103">若要修复此错误，请在受影响的计算机上尝试以下选项：</span><span class="sxs-lookup"><span data-stu-id="722a6-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="722a6-104">打开 Office 应用程序，选择 "**文件** > **帐户** > 注销**所有帐户**"。</span><span class="sxs-lookup"><span data-stu-id="722a6-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="722a6-105">使用具有有效许可证的用户帐户重新登录。</span><span class="sxs-lookup"><span data-stu-id="722a6-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="722a6-106">有关详细信息，请参阅[Office 中的帐户](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)。</span><span class="sxs-lookup"><span data-stu-id="722a6-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="722a6-107">使用 Windows 凭据管理器[清除 Office 凭据](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)。</span><span class="sxs-lookup"><span data-stu-id="722a6-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="722a6-108">**注意：** Office 2016 的注册表路径已更改为16.0。</span><span class="sxs-lookup"><span data-stu-id="722a6-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="722a6-109">例如，\Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="722a6-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="722a6-110">在受影响的计算机上，使用以下步骤设置 EnableADAL = 0：</span><span class="sxs-lookup"><span data-stu-id="722a6-110">On the affected computer, set the EnableADAL = 0 using the following steps:</span></span>  
     1. <span data-ttu-id="722a6-111">右键单击 "Windows" 按钮，然后选择 "**运行**"。</span><span class="sxs-lookup"><span data-stu-id="722a6-111">Right-click the Windows button and select **Run**.</span></span> <span data-ttu-id="722a6-112">在 "**打开**" 框中，键入 " **regedit**"，然后选择 **"确定"**。</span><span class="sxs-lookup"><span data-stu-id="722a6-112">In the **Open** box, type **regedit**, and then select **OK**.</span></span>
     2. <span data-ttu-id="722a6-113">当系统提示允许注册表编辑器对设备进行更改时，选择 **"是"** 。</span><span class="sxs-lookup"><span data-stu-id="722a6-113">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="722a6-114">在注册表编辑器中，将 EnableADAL 的 DWORD 值添加到 HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity. 下的设置为0。</span><span class="sxs-lookup"><span data-stu-id="722a6-114">In the Registry Editor, add a DWORD value of EnableADAL with a setting of 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>
- <span data-ttu-id="722a6-115">如果使用 Office 2013 连接到 Office 365 时出现错误，请为 Office 客户端[启用新式验证](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)。</span><span class="sxs-lookup"><span data-stu-id="722a6-115">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="722a6-116">有关详细信息，请参阅[如何排查无法登录到 Office 365、Azure 或 Intune 的非浏览器应用程序的问题](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)。</span><span class="sxs-lookup"><span data-stu-id="722a6-116">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

