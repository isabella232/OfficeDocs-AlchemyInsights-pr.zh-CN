---
title: 接收 SharePoint 和 OneDrive 警报时的延迟
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 02/04/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 0bc9f614047e06e8654a9b3ff64e87427f33139f
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/04/2020
ms.locfileid: "41771205"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>接收 SharePoint 和 OneDrive 警报时的延迟

- 首先检查电子邮件中的 "垃圾邮件" 或 "垃圾邮件" 文件夹。
- 如果**延迟来自多个文件或库的所有警报**，请访问[服务运行状况仪表板](https://nam06.safelinks.protection.outlook.com/?url=https://admin.microsoft.com/AdminPortal/Home%23/servicehealth&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0)，以检查任何可能与 SharePoint 或 Exchange 发生的咨询/事件。 问题可能与 SharePoint 通知功能或通过 Exchange 的电子邮件延迟有关。 此外，请注意是否正在传递其他电子邮件—如果不是，则问题可能与 Exchange 延迟有关。
- 如果**未传递来自特定文件或库的单个警报**，请尝试删除并重新创建它。 请参阅[管理、查看或删除 SharePoint 警报](https://nam06.safelinks.protection.outlook.com/?url=https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax/epn3E%3D&reserved=0)以重新创建警报。

> [!NOTE]
> - 无法将通知发送到通讯组。 仅支持 Security 和 O365 组。
> - 您不能自定义警报电子邮件模板。 必须使用 Microsoft Flow 或 SharePoint Designer 工作流来实现这些。
