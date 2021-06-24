---
title: 启用 SMTP 身份验证和故障排除
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
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077641"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="eeb08-102">启用 SMTP 身份验证和故障排除</span><span class="sxs-lookup"><span data-stu-id="eeb08-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="eeb08-103">如果要为邮箱启用 SMTP 身份验证，或者在尝试通过使用 Microsoft 365 对设备或应用程序进行身份验证来中继电子邮件时收到“客户端未通过身份验证”、“身份验证失败”或“SmtpClientAuthentication”错误消息（代码分别为“5.7.57”、“5.7.3”和“5.7.139”），请执行以下三项操作来解决此问题：</span><span class="sxs-lookup"><span data-stu-id="eeb08-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="eeb08-104">通过将“**启用安全性默认设置**”切换为“**否**”，禁用 [Azure 安全性默认设置](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)。</span><span class="sxs-lookup"><span data-stu-id="eeb08-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="eeb08-105">a.</span><span class="sxs-lookup"><span data-stu-id="eeb08-105">a.</span></span> <span data-ttu-id="eeb08-106">以安全管理员、条件访问管理员或全局管理员的身份登录到 Azure 门户。</span><span class="sxs-lookup"><span data-stu-id="eeb08-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="eeb08-107">b.</span><span class="sxs-lookup"><span data-stu-id="eeb08-107">b.</span></span> <span data-ttu-id="eeb08-108">浏览到 Azure Active Directory > **属性**。</span><span class="sxs-lookup"><span data-stu-id="eeb08-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="eeb08-109">c.</span><span class="sxs-lookup"><span data-stu-id="eeb08-109">c.</span></span> <span data-ttu-id="eeb08-110">选择 **管理安全性默认设置**。</span><span class="sxs-lookup"><span data-stu-id="eeb08-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="eeb08-111">d.</span><span class="sxs-lookup"><span data-stu-id="eeb08-111">d.</span></span> <span data-ttu-id="eeb08-112">将“**启用安全性默认设置**”设置为“**否**”。</span><span class="sxs-lookup"><span data-stu-id="eeb08-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="eeb08-113">e.</span><span class="sxs-lookup"><span data-stu-id="eeb08-113">e.</span></span> <span data-ttu-id="eeb08-114">选择“**保存**”。</span><span class="sxs-lookup"><span data-stu-id="eeb08-114">Select **Save**.</span></span>

2. <span data-ttu-id="eeb08-115">在许可邮箱上[启用客户端 SMTP 提交](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes)。</span><span class="sxs-lookup"><span data-stu-id="eeb08-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="eeb08-116">a.</span><span class="sxs-lookup"><span data-stu-id="eeb08-116">a.</span></span> <span data-ttu-id="eeb08-117">从 Microsoft 365 管理中心，转到“**活动用户**”并选择用户。</span><span class="sxs-lookup"><span data-stu-id="eeb08-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="eeb08-118">b.</span><span class="sxs-lookup"><span data-stu-id="eeb08-118">b.</span></span> <span data-ttu-id="eeb08-119">转到“邮件”选项卡，然后在“**电子邮件应用**”下，选择“**管理电子邮件应用**”。</span><span class="sxs-lookup"><span data-stu-id="eeb08-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="eeb08-120">d.</span><span class="sxs-lookup"><span data-stu-id="eeb08-120">d.</span></span> <span data-ttu-id="eeb08-121">确保已选中“**已验证的 SMTP**”（已启用）。</span><span class="sxs-lookup"><span data-stu-id="eeb08-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="eeb08-122">e.</span><span class="sxs-lookup"><span data-stu-id="eeb08-122">e.</span></span> <span data-ttu-id="eeb08-123">选择“**保存更改**”。</span><span class="sxs-lookup"><span data-stu-id="eeb08-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="eeb08-124">在许可邮箱上[禁用多重身份验证 (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa)。</span><span class="sxs-lookup"><span data-stu-id="eeb08-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="eeb08-125">a.</span><span class="sxs-lookup"><span data-stu-id="eeb08-125">a.</span></span> <span data-ttu-id="eeb08-126">转到 Microsoft 365 管理中心，在左侧导航菜单窗格中选择“**用户** > **活动用户**”。</span><span class="sxs-lookup"><span data-stu-id="eeb08-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="eeb08-127">b.</span><span class="sxs-lookup"><span data-stu-id="eeb08-127">b.</span></span> <span data-ttu-id="eeb08-128">选择“**多重身份验证**”。</span><span class="sxs-lookup"><span data-stu-id="eeb08-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="eeb08-129">c.</span><span class="sxs-lookup"><span data-stu-id="eeb08-129">c.</span></span> <span data-ttu-id="eeb08-130">选择用户并禁用“**多重身份验证**”。</span><span class="sxs-lookup"><span data-stu-id="eeb08-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
