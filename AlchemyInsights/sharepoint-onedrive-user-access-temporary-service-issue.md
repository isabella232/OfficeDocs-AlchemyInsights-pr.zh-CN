---
title: 性能问题-SharePoint或OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 08bdc2527147279063e3f66a1767203e5ccdc1dd4fd8b871f2800d3f71b9a233
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093676"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint或OneDrive用户速度慢、无法访问或不可用

如果OneDrive或SharePoint网站对以前具有访问权限的多个用户不可用，则可能是临时服务问题。 [检查服务运行状况仪表板](https://portal.office.com/adminportal/home#/servicehealth)。

**添加和许可用户**

确保为[企业版中的用户Microsoft 365许可证](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)。


**分配权限**

如果用户已分配有 Sharepoint 许可证，但仍收到拒绝访问消息，请确保他们分配了 [适当的权限](https://docs.microsoft.com/sharepoint/understanding-permission-levels) 级别。

**考虑使用访问请求功能**

访问 [请求功能](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) 允许用户请求访问他们当前无权查看的内容。

**允许自定义脚本可能导致访问被拒绝问题**

在某些情况下，允许自定义 *脚本功能可能会* 显示拒绝访问。 有关受影响的功能的列表、安全注意事项以及禁用该功能的功能。 请访问允许 [或阻止自定义脚本](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)。

