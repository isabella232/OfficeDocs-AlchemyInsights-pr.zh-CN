---
title: 无法访问 SharePoint 或 OneDrive 管理中心
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
- "9001459"
- "5638"
ms.openlocfilehash: afb28ccae2c9f087f1e1417cb6594cedc908e1cf759a5d1e6d92c4ee9a75527d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020434"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a>无法访问 SharePoint 或 OneDrive 管理中心

- 如果你的 SharePoint 或 OneDrive 管理中心网站无法访问或不可用，则可能存在暂时性服务问题，具体表现为用户在访问 SharePoint 网站或 OneDrive 内容时遇到间歇性延迟或导航错误。 请查看[服务运行状况仪表板](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)，了解你的组织是否受到影响。

- 需要向全局和 SharePoint 管理员分配 SharePoint 许可证。 刚分配了 SharePoint 许可证或管理员角色的新创建的帐户在访问 SharePoint 时可能会遇到问题，例如“拒绝访问”或“找不到用户”。 请至少留出 24 小时，以便在我们的整个系统中完成同步。 我们理解，24 小时可能看起来很长。 在许多情况下，我们已经在研究解决方案。

- 如果允许的访问时间段非常小，则 Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) 用户可能会遇到访问被拒的情况，请参阅[对 PIM 帐户的访问被拒绝](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)。