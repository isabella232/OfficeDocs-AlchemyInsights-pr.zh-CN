---
title: 授予用户对 SharePoint 和 OneDrive 的访问权限
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
ms.openlocfilehash: ae4d2c00be6387744bdc84e1d8a021530f80f8fa
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2019
ms.locfileid: "34715202"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="afc33-102">授予用户对 SharePoint 和 OneDrive 的访问权限</span><span class="sxs-lookup"><span data-stu-id="afc33-102">Give users access to SharePoint and OneDrive</span></span>

<p><span data-ttu-id="afc33-103"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">在使用相同的用户主体名称 (UPN) 对用户进行删除和重新创建时, 通常会出现此问题。使用不同的 PUID (Passport 唯一 ID) 值创建新帐户。当用户尝试访问网站集或其 OneDrive 时, 用户的 PUID 不正确。第二个方案涉及与 Active Directory 组织单位 (OU) 的目录同步。如果用户已登录到 SharePoint, 然后将移动到不同的 OU 并 resynced 使用 SharePoint, 他们可能会遇到此问题。</span></span><span class="sxs-lookup"><span data-stu-id="afc33-103"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN). The new account is created by using a different PUID (Passport Unique ID) value. When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID. A second scenario involves directory synchronization with an Active Directory organizational unit (OU). If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span></span></p> <p><span data-ttu-id="afc33-104"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">若要解决此问题, 您应使用本文中的步骤还原原始 UPN, 在<a href="https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide">Office 365 中还原用户。</a></span></span><span class="sxs-lookup"><span data-stu-id="afc33-104"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">To resolve this issue you should restore the original UPN with the steps in the article, <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide">Restore a user in Office 365.</a></span></span></span></p> <p><span data-ttu-id="afc33-105"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">完成此操作后, 您可以按照为<a href="https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive">用户的 Onedrive 添加管理员的</a>步骤来验证用户是否具有对 onedrive 网站的管理员权限。</span></span><span class="sxs-lookup"><span data-stu-id="afc33-105"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to <a href="https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive">Add admin's for a user's OneDrive.</a></span></span></span></p> <p><span data-ttu-id="afc33-106"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">有关权限级别的详细信息, 请参阅<a href="https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels">了解 SharePoint 中的权限级别</a>一文。&nbsp;</span></span><span class="sxs-lookup"><span data-stu-id="afc33-106"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">For more information on permission levels, see the article, <a href="https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels">Understanding permission levels in SharePoint.</a>&nbsp;</span></span></span></p>
