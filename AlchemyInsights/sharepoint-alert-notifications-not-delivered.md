---
title: SharePoint通知未送达
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: 05bd913098372a57d3061e8c516a6a6b4f0a9bdafde02acc930062d6281d06dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957891"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>SharePoint通知未送达

请检查电子邮件中的"垃圾邮件"文件夹，因为有时可能会显示警报。

确定是否 **未传递所有警报，** 或者是否未传递来自特定文件或库的单个警报。

- **不发送单个警报**：如果未传递来自特定文件或库的单个警报，您可以尝试删除并重新创建它。 请参阅[管理、查看或删除SharePoint警报以](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2)重新创建警报。
- 所有警报均 **未送达**：如果未传递来自多个文件或库的所有警报，请访问服务运行状况仪表板，以检查 [](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)SharePoint 或 Exchange 中是否发生任何警报/事件。 问题可能是电子邮件SharePoint警报功能或延迟Exchange。 此外，还必须注意其他电子邮件是否正在传递，如果未传递，则问题可能Exchange延迟。

警报常见问题解答：

- 无法向通讯组发送通知，仅支持安全组和 O365 组。
- 无法自定义通知电子邮件模板;你需要使用 Microsoft FLOW 或SharePoint设计器工作流来实现这些目的。

## <a name="related-topics"></a>相关主题

想要尝试在 Microsoft Flow Online SharePoint？

- [创建Flow](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint 和 Flow](https://flow.microsoft.com//blog/sharepoint-and-flow/)
