---
title: 部署加载项Microsoft 365 应用版
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/30/2021
ms.locfileid: "52107499"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>部署加载项Microsoft 365 应用版

建议使用集中部署将外接程序Office组织内部的用户和组。 若要部署外接程序，请按照以下步骤操作：

**注意：** 若要以单个用户Office加载项，请参阅在加载项程序中查看、管理和Office [加载项](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)。 此外，请确保启用单独Office应用商店加载项的购置。 

1. 确保您的环境满足使用集中部署部署外接程序的要求。 有关详细信息，请参阅 [要求](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)。
2. 转到 **设置**  >  **集成应用** 在 Microsoft 365 管理中心获取  >  应用以部署外接程序。 

注意： 

- 集成应用要求管理员具有全局管理员或Exchange管理员权限。

- 将外接程序部署到多个用户时，我们建议使用组而不是单个用户进行分配。 有关详细信息，请参阅 [将加载项分配给用户和组的注意事项](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)。

- 集中部署不支持嵌套组或具有父组的组的用户。 有关详细信息，请参阅用户 [和组分配](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)。

- 确保为用户启用 Microsoft 365 App Management Service (GUID：'0517ffae-825d-4aff-999e-3f2336b8a20a') 。 有关详细信息，请参阅配置 [应用属性](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)。

- 如果使用集成应用部署加载项时遇到问题，请尝试使用加载项 [进行部署](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)。

有关更多信息，请参阅：

[在管理中心部署外接程序](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
[在管理中心管理外接程序](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
[使用集中部署 PowerShell cmdlet 管理外接程序](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
[通过Office中心集中部署发布Microsoft 365加载项](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
[疑难解答：用户看不到外接程序](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
[排查Office加载项中的用户错误](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)