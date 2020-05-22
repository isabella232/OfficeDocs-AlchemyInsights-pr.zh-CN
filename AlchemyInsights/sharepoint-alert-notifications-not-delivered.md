---
title: 未传递 SharePoint 通知通知
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: 363f3c79a3b62f3017e6c873f1be3dd195cab883
ms.sourcegitcommit: 5296874062b16f945d9a7a7a9ab29ec53686310b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44343085"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>未传递 SharePoint 通知通知

请检查电子邮件中的垃圾邮件文件夹，有时会出现通知。

确定是否**未传递所有警报**，或者是否未传递来自特定文件或库**的单个警报**。

- **不传递单个警报**：如果未传递来自特定文件或库的单个通知，则可以尝试删除并重新创建它。 请参阅[管理、查看或删除 SharePoint 警报](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2)以重新创建警报。
- **未传递所有警报**：如果未传递来自多个文件或库的所有警报，请访问[服务运行状况仪表板](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)，以检查 SharePoint 或 Exchange 可能发生的任何咨询/事件。 问题可能与 SharePoint 通知功能或通过 Exchange 的电子邮件延迟有关。 此外，请务必注意是否正在传递其他电子邮件，如果没有，则可能是 Exchange 延迟问题。

有关警报的常见问题解答：

- 无法向通讯组发送通知，仅支持安全和 O365 组。
- 您不能自定义通知电子邮件模板;您需要使用 Microsoft FLOW 或 SharePoint Designer 工作流来实现这些。

## <a name="related-topics"></a>相关主题

想要在 SharePoint Online 中试用 Microsoft 流吗？

- [创建流](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint 和流](https://flow.microsoft.com//blog/sharepoint-and-flow/)
