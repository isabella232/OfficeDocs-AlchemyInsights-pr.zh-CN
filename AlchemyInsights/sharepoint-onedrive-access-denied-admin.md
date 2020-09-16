---
title: 访问被拒绝邮件疑难解答
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767643"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="4c749-102">Sharepoint/OneDrive 管理中心中的拒绝访问邮件疑难解答</span><span class="sxs-lookup"><span data-stu-id="4c749-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="4c749-103">如果在尝试浏览到 Sharepoint/OneDrive 管理中心时收到 "拒绝访问" 消息，请确保 [将许可证分配](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)给该用户。</span><span class="sxs-lookup"><span data-stu-id="4c749-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="4c749-104">如果用户具有许可证，还应确保为其分配可访问管理中心的 [管理员角色](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) 。</span><span class="sxs-lookup"><span data-stu-id="4c749-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="4c749-105">在使用相同的用户主体名称 (UPN) 中删除并重新创建用户时，也会发生此问题。</span><span class="sxs-lookup"><span data-stu-id="4c749-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="4c749-106">新帐户是使用其他 PUID (Passport 唯一 ID) 值创建的。</span><span class="sxs-lookup"><span data-stu-id="4c749-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="4c749-107">当用户尝试访问网站集或其 OneDrive 时，用户的 PUID 不正确。</span><span class="sxs-lookup"><span data-stu-id="4c749-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="4c749-108">第二个方案涉及目录与 Active Directory 组织单位 (OU) 的同步。</span><span class="sxs-lookup"><span data-stu-id="4c749-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="4c749-109">如果用户已登录到 SharePoint，然后将移动到不同的 OU 并 resynced 使用 SharePoint，他们可能会遇到此问题。</span><span class="sxs-lookup"><span data-stu-id="4c749-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="4c749-110">若要解决此问题，您应使用本文中的步骤还原原始 UPN，在 [Microsoft 365 中还原用户](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)。</span><span class="sxs-lookup"><span data-stu-id="4c749-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="4c749-111">注意：如果 OneDrive 或 SharePoint 管理中心对之前有权访问的多个用户不可用，则可能存在暂时性的服务问题。</span><span class="sxs-lookup"><span data-stu-id="4c749-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="4c749-112">[检查服务运行状况仪表板](https://portal.office.com/adminportal/home#/servicehealth)。</span><span class="sxs-lookup"><span data-stu-id="4c749-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


