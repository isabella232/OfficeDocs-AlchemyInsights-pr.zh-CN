---
title: 修复 Microsoft 365 应用你的帐户处于错误状态消息
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
- "2558"
- "9000571"
ms.openlocfilehash: ec529291ec9406eba9dc2b0f2cc7a93c77fa3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744535"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="e3ff7-102">修复 Microsoft 365 应用程序 "你的帐户处于错误状态" 错误</span><span class="sxs-lookup"><span data-stu-id="e3ff7-102">Fixing the Microsoft 365 apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="e3ff7-103">若要修复此错误，请在受影响的计算机上尝试以下选项：</span><span class="sxs-lookup"><span data-stu-id="e3ff7-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="e3ff7-104">打开 Office 应用程序，选择 "**文件**  >  **帐户**注销  >  **所有帐户**"。</span><span class="sxs-lookup"><span data-stu-id="e3ff7-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="e3ff7-105">使用具有有效许可证的用户帐户再次登录。</span><span class="sxs-lookup"><span data-stu-id="e3ff7-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="e3ff7-106">有关详细信息，请参阅 [Office 中的帐户](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)。</span><span class="sxs-lookup"><span data-stu-id="e3ff7-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="e3ff7-107">使用 Windows 凭据管理器[清除 Office 凭据](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)。</span><span class="sxs-lookup"><span data-stu-id="e3ff7-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="e3ff7-108">**注意：** Office 2016 的注册表路径已更改为16.0。</span><span class="sxs-lookup"><span data-stu-id="e3ff7-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="e3ff7-109">例如，\Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="e3ff7-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="e3ff7-110">如果使用 Office 2013 连接到 Office 365 时出现错误，请为 Office 客户端 [启用新式验证](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) 。</span><span class="sxs-lookup"><span data-stu-id="e3ff7-110">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="e3ff7-111">有关详细信息，请参阅 [如何排查无法登录到 Microsoft 365、Azure 或 Intune 的非浏览器应用程序的问题](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)。</span><span class="sxs-lookup"><span data-stu-id="e3ff7-111">For more information, see [How to troubleshoot non-browser apps that can't sign in to Microsoft  365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

