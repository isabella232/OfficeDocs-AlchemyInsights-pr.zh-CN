---
title: 不接收 SharePoint 和 OneDrive 警报
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/25/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 80423791ad558fc414d50608c73f823036432e14
ms.sourcegitcommit: 5e6a805fb0b41d714ca1cf90e23b8e2daa90f90e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37205505"
---
# <a name="not-receiving-sharepoint-and-onedrive-alerts"></a>不接收 SharePoint 和 OneDrive 警报

首先检查电子邮件中的 "垃圾邮件" 或 "垃圾邮件" 文件夹。

然后，确定是否**未传递所有警报**，或者是否未传递来自特定文件或库**的单个警报**。

- 如果**未传递来自多个文件或库的所有警报**，请访问[服务运行状况仪表板](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fadmin.microsoft.com%2FAdminPortal%2FHome%23%2Fservicehealth&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0)，以检查任何可能与 SharePoint 或 Exchange 一起发生的咨询/事件。 问题可能与 SharePoint 通知功能或通过 Exchange 的电子邮件延迟有关。 此外，请注意是否正在传递其他电子邮件—如果不是，则问题可能与 Exchange 延迟有关。
- 如果**未传递来自特定文件或库的单个警报**，请尝试删除并重新创建它。 请参阅[管理、查看或删除 SharePoint 警报](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2Fmanage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2%3Fui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax%2Fepn3E%3D&reserved=0)以重新创建警报。

> [!NOTE]
> - 无法将通知发送到通讯组。 仅支持 Security 和 O365 组。
> - 您不能自定义警报电子邮件模板。 必须使用 Microsoft Flow 或 SharePoint Designer 工作流来实现这些。
