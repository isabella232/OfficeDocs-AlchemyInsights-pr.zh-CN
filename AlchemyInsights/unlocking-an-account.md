---
title: 解除帐户锁定
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002449"
- "4748"
ms.openlocfilehash: cf2431cb49902b3f7625ab96bc6d4e2121e51fdd
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544134"
---
# <a name="unlocking-an-account"></a><span data-ttu-id="53b06-102">解除帐户锁定</span><span class="sxs-lookup"><span data-stu-id="53b06-102">Unlocking an account</span></span>

<span data-ttu-id="53b06-103">用户可能会因密码尝试不当或其他威胁而被锁定，无法再使用 Microsoft 365。</span><span class="sxs-lookup"><span data-stu-id="53b06-103">It's possible users are locked out of Microsoft 365 due to bad password attempts or other compromises.</span></span> <span data-ttu-id="53b06-104">若要帮助用户重新登录到 Microsoft 365，**可在考虑开启支持请求之前先尝试执行以下步骤**。</span><span class="sxs-lookup"><span data-stu-id="53b06-104">To help users sign back in to Microsoft 365, **you can attempt the following steps before opening a Support Request**.</span></span> 

<span data-ttu-id="53b06-105">**电子邮件发送受限**</span><span class="sxs-lookup"><span data-stu-id="53b06-105">**Email Restricted**</span></span>

<span data-ttu-id="53b06-106">作为管理员，如果你的一个用户被限制发送电子邮件，可以[自行为其解除帐户锁定](/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)。</span><span class="sxs-lookup"><span data-stu-id="53b06-106">As an admin, if one of your users is restricted from sending email, you can [unblock the account yourself](/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam).</span></span> <span data-ttu-id="53b06-107">解除限制后，该用户在一小时之内便可发送电子邮件。</span><span class="sxs-lookup"><span data-stu-id="53b06-107">The user will be able to send email within an hour after removing the restriction.</span></span>

<span data-ttu-id="53b06-108">**重置用户密码**</span><span class="sxs-lookup"><span data-stu-id="53b06-108">**Reset the User Password**</span></span>

1. <span data-ttu-id="53b06-109">在管理中心中，转到“**用户”>“[活动用户](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)**”。</span><span class="sxs-lookup"><span data-stu-id="53b06-109">In the admin center, go to **Users > [Active Users](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)**.</span></span>

2. <span data-ttu-id="53b06-110">选择用户，随后选择“**重置密码**”。</span><span class="sxs-lookup"><span data-stu-id="53b06-110">Select the user and click **Reset Password**.</span></span>

<span data-ttu-id="53b06-111">**确保允许用户登录**</span><span class="sxs-lookup"><span data-stu-id="53b06-111">**Make sure the user is allowed to sign in**</span></span>

1. <span data-ttu-id="53b06-112">在管理中心中，转到“**用户”>“[活动用户](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)**”。</span><span class="sxs-lookup"><span data-stu-id="53b06-112">In the admin center, go to **Users > [Active Users](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)**.</span></span>

2. <span data-ttu-id="53b06-113">选择用户，然后单击三个点（更多操作）以及 **“编辑登录状态”**。</span><span class="sxs-lookup"><span data-stu-id="53b06-113">Select the user and click the three dots (more actions), then click **Edit sign-in status**.</span></span>

<span data-ttu-id="53b06-114">有关更多密码重置方案（包括自助式密码重置），请参阅[重置 Microsoft 365 multiple-attempts-to-charge-online-payment-instrumentsbusiness 密码](/microsoft-365/admin/add-users/reset-passwords)。</span><span class="sxs-lookup"><span data-stu-id="53b06-114">For more password reset scenarios, including Self-Service Password Reset, see [Reset Microsoft 365 for multiple-attempts-to-charge-online-payment-instrumentsbusiness passwords](/microsoft-365/admin/add-users/reset-passwords).</span></span>

<span data-ttu-id="53b06-115">此服务在检测到帐户被盗用和/或出站垃圾邮件的证据后，阻止用户发送电子邮件。</span><span class="sxs-lookup"><span data-stu-id="53b06-115">The service prevents a user from sending email after detecting evidence of a compromised account and/or outbound spam.</span></span> <span data-ttu-id="53b06-116">为预防起见，按照[响应 Microsoft 365 中遭到入侵的电子邮件帐户](/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)的用户步骤执行操作。</span><span class="sxs-lookup"><span data-stu-id="53b06-116">As a precaution, follow the steps in [Responding to a Compromised Email Account in Microsoft 365](/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account) for the user.</span></span>
