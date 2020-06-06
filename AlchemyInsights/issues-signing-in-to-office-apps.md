---
title: 登录到 Microsoft 365 应用程序时出现问题
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
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579927"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="7e647-102">修复 Microsoft 365 应用程序 "抱歉，你的组织中的另一个帐户已登录" 消息</span><span class="sxs-lookup"><span data-stu-id="7e647-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="7e647-103">若要修复此错误，请使用以下步骤：</span><span class="sxs-lookup"><span data-stu-id="7e647-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="7e647-104">使用 Windows 设置 >**访问工作或学校**，删除除受影响帐户之外的所有工作帐户。</span><span class="sxs-lookup"><span data-stu-id="7e647-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="7e647-105">使用 Windows 凭据管理器[清除 Office 凭据](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)。</span><span class="sxs-lookup"><span data-stu-id="7e647-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="7e647-106">**注意：** Office 2016 的注册表路径已更改为16.0。</span><span class="sxs-lookup"><span data-stu-id="7e647-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="7e647-107">（Ex： \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="7e647-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="7e647-108">打开 Office 应用程序，选择 "**文件**  >  **帐户**  >  **注销**"。然后使用具有有效许可证的用户帐户登录。</span><span class="sxs-lookup"><span data-stu-id="7e647-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="7e647-109">有关详细信息，请参阅[Office 中的账户](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)。</span><span class="sxs-lookup"><span data-stu-id="7e647-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="7e647-110">对于 Mac，参见[无法登录至 Office 2016 for Mac 应用](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)。</span><span class="sxs-lookup"><span data-stu-id="7e647-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="7e647-111">有关详细信息，请参阅[Office 中的 "抱歉，你的组织中的另一个帐户已在此计算机上登录"](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)。</span><span class="sxs-lookup"><span data-stu-id="7e647-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>