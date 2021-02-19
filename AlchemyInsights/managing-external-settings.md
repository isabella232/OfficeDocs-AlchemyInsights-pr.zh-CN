---
title: 管理外部设置
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50282806"
---
# <a name="managing-external-settings"></a><span data-ttu-id="5721d-102">管理外部设置</span><span class="sxs-lookup"><span data-stu-id="5721d-102">Managing External Settings</span></span>

<span data-ttu-id="5721d-103">**公告**</span><span class="sxs-lookup"><span data-stu-id="5721d-103">**Announcement**</span></span>

- <span data-ttu-id="5721d-104">[从 2021 年 1 月 4 日起，Google 弃用 WebView 登录支持](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support)。</span><span class="sxs-lookup"><span data-stu-id="5721d-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span></span> <span data-ttu-id="5721d-105">按照 Google 关于测试兼容性的指南，测试你的应用是否受到了影响</span><span class="sxs-lookup"><span data-stu-id="5721d-105">Test whether your apps are affected by following Google’s guidance on testing compatibility</span></span>
- <span data-ttu-id="5721d-106">让用户使用消费者 Google 帐户登录时，请确保使用系统 Web 视图或系统浏览器。</span><span class="sxs-lookup"><span data-stu-id="5721d-106">Make sure to use the system webview or the system browser when signing in your users with consumer Google accounts</span></span>

<span data-ttu-id="5721d-107">**管理邀请设置**</span><span class="sxs-lookup"><span data-stu-id="5721d-107">**Manage Invitation Settings**</span></span>

<span data-ttu-id="5721d-108">请确认你[配置了外部协作设置](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)以允许相应人员发送邀请。</span><span class="sxs-lookup"><span data-stu-id="5721d-108">Confirm that you have [configured the external collaboration settings](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) to allow the appropriate people to send invitations.</span></span>

<span data-ttu-id="5721d-109">**管理来宾用户访问权限**</span><span class="sxs-lookup"><span data-stu-id="5721d-109">**Manage Guest User Access Permissions**</span></span>

1. <span data-ttu-id="5721d-110">通过在“外部协作设置”页面上配置来宾访问权限，全局管理员就可以在目录中通过 Azure 门户管理来宾访问权限。</span><span class="sxs-lookup"><span data-stu-id="5721d-110">Global admins can manage guest access permissions in the directory through the Azure portal by configuring the guest access permissions on the External Collaboration Settings page.</span></span> <span data-ttu-id="5721d-111">[了解有关此设置的详细信息](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="5721d-111">[Learn more about this setting](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
2. <span data-ttu-id="5721d-112">如果希望来宾访问 Teams 或 SharePoint 等应用，请确认已配置这些应用以允许来宾访问。</span><span class="sxs-lookup"><span data-stu-id="5721d-112">If you would like your guests to access apps such as Teams or SharePoint, confirm that you've configured those apps to allow guest access.</span></span> <span data-ttu-id="5721d-113">了解更多关于 [Teams 设置](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support)和 [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support) 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5721d-113">Learn more about the [Teams settings](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) and [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="5721d-114">**配置邀请：**</span><span class="sxs-lookup"><span data-stu-id="5721d-114">**Configuring invitations:**</span></span>

- [<span data-ttu-id="5721d-115">启用 B2B 外部协作以及管理谁可邀请来宾</span><span class="sxs-lookup"><span data-stu-id="5721d-115">Enable B2B external collaboration and manage who can invite guests</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- <span data-ttu-id="5721d-116">[允许或阻止邀请来自特定组织的用户](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="5721d-116">[Allow or block invitations to users from specific organizations](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="5721d-117">**配置允许的身份提供程序：**</span><span class="sxs-lookup"><span data-stu-id="5721d-117">**Configuring allowed identity providers:**</span></span>

- [<span data-ttu-id="5721d-118">Google 联合身份验证</span><span class="sxs-lookup"><span data-stu-id="5721d-118">Google Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="5721d-119">直接联合身份验证</span><span class="sxs-lookup"><span data-stu-id="5721d-119">Direct Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="5721d-120">发送一次性密码身份验证的电子邮件</span><span class="sxs-lookup"><span data-stu-id="5721d-120">Email one-time Passcode Authentication</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
