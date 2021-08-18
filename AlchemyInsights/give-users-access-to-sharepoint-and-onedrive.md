---
title: 向用户授予SharePoint和OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: e3d645f3c45525107f42a074899a30ef26bd559e5c5657e7b8ef69d406357b32
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088890"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>向用户授予SharePoint和OneDrive

> [!NOTE]
> 如果OneDrive或SharePoint网站对以前具有访问权限的多个用户不可用，则可能是临时服务问题。 [检查服务运行状况仪表板](https://portal.office.com/adminportal/home#/servicehealth)
  
如果希望组织成员能够登录并使用 SharePoint 和 OneDrive，则需要为用户添加帐户，并确保他们拥有允许其访问 SharePoint 和 OneDrive 的许可证。 添加用户的最简单方法是在 Microsoft 365 管理中心。
  
1. 转到"活动 [用户"页Microsoft 365 管理中心，](https://portal.office.com/adminportal/home#/users)然后单击"**添加用户"。**
    
2. 填写用户信息，并确保在"产品许可证"下分配许可证 **，SharePoint"Online"。** 
    
请注意，如果允许在组织中进行外部共享，用户可以与组织SharePoint OneDrive共享内容。 无需向这些外部用户授予许可证。 您也不需要为帐户添加帐户，除非共享设置为"仅现有外部用户"。 在这种情况下，如果用户不在组织目录中，你需要在 Azure AD 管理中心中将它们添加为来宾用户。
  

