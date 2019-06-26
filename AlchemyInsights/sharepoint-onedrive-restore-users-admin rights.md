---
title: 对 OneDrive for Business 网站的 "拒绝访问" 消息进行故障排除
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: b394cc1441187133d8829cfc5fb0c1edbd71fd96
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223414"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="4f7b2-102">对 OneDrive for Business 网站的 "拒绝访问" 消息进行故障排除</span><span class="sxs-lookup"><span data-stu-id="4f7b2-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="4f7b2-103">在使用相同的用户主体名称 (UPN) 对用户进行删除和重新创建时, 通常会出现此问题。</span><span class="sxs-lookup"><span data-stu-id="4f7b2-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="4f7b2-104">使用不同的 PUID (Passport 唯一 ID) 值创建新帐户。</span><span class="sxs-lookup"><span data-stu-id="4f7b2-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="4f7b2-105">当用户尝试访问网站集或其 OneDrive 时, 用户的 PUID 不正确。</span><span class="sxs-lookup"><span data-stu-id="4f7b2-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="4f7b2-106">第二个方案涉及与 Active Directory 组织单位 (OU) 的目录同步。</span><span class="sxs-lookup"><span data-stu-id="4f7b2-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="4f7b2-107">如果用户已登录到 SharePoint, 然后将移动到不同的 OU 并 resynced 使用 SharePoint, 他们可能会遇到此问题。</span><span class="sxs-lookup"><span data-stu-id="4f7b2-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="4f7b2-108">若要解决此问题, 您应使用本文中的步骤还原原始 UPN, 在[Office 365 中还原用户](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)。</span><span class="sxs-lookup"><span data-stu-id="4f7b2-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="4f7b2-109">完成此操作后, 您可以通过按照为[用户的 Onedrive 添加管理员的](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)步骤来验证用户是否具有对 onedrive 网站的管理员权限。</span><span class="sxs-lookup"><span data-stu-id="4f7b2-109">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="4f7b2-110">有关权限级别的详细信息, 请参阅[了解 SharePoint 中的权限级别](https://docs.microsoft.com/sharepoint/understanding-permission-levels)一文。</span><span class="sxs-lookup"><span data-stu-id="4f7b2-110">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
