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
- "2574"
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762966"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="913fb-102">登录 Office 应用程序时出现问题</span><span class="sxs-lookup"><span data-stu-id="913fb-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="913fb-103">若要修复 Office 应用的登录问题，请尝试以下操作：</span><span class="sxs-lookup"><span data-stu-id="913fb-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="913fb-104">使用 Windows 设置 >**访问工作或学校**，删除除受影响帐户之外的所有工作帐户。</span><span class="sxs-lookup"><span data-stu-id="913fb-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="913fb-105">使用 Windows 凭据管理器[清除 Office 凭据](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)。</span><span class="sxs-lookup"><span data-stu-id="913fb-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="913fb-106">**注意：** Office 2016 的注册表路径已更改为16.0。</span><span class="sxs-lookup"><span data-stu-id="913fb-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="913fb-107">（Ex： \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="913fb-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="913fb-108">打开 Office 应用程序，选择 "**文件** > **帐户** > **注销**"。然后使用具有有效许可证的用户帐户登录。</span><span class="sxs-lookup"><span data-stu-id="913fb-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="913fb-109">有关详细信息，请参阅[Office 中的账户](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)。</span><span class="sxs-lookup"><span data-stu-id="913fb-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="913fb-110">对于 Mac，参见[无法登录至 Office 2016 for Mac 应用](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)。</span><span class="sxs-lookup"><span data-stu-id="913fb-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="913fb-111">如果使用 Office 2013 连接到 Microsoft 365 时出现错误，请为 Office 客户端启用新式验证。</span><span class="sxs-lookup"><span data-stu-id="913fb-111">If the errors occurs while connecting to Microsoft 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="913fb-112">有关详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="913fb-112">For more information, see:</span></span>
- [<span data-ttu-id="913fb-113">你无法登录到 Microsoft 365、Azure 或 Intune</span><span class="sxs-lookup"><span data-stu-id="913fb-113">You can't sign in to Microsoft 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="913fb-114">在 Windows 10 上更新到 Office 2016 生成16.0.7967 后登录中的连接问题</span><span class="sxs-lookup"><span data-stu-id="913fb-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="913fb-115">"很抱歉，你的组织中的另一个帐户已在此计算机上登录" （Office）</span><span class="sxs-lookup"><span data-stu-id="913fb-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="913fb-116">使用 ADFS 解决 Office 新式身份验证时的登录问题</span><span class="sxs-lookup"><span data-stu-id="913fb-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)