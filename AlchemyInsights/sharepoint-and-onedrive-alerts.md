---
title: 接收 SharePoint 和 OneDrive 警报时的延迟
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 27cc744bc57f1c18649e05c5b0df3b315c9c0201
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727233"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>接收 SharePoint 和 OneDrive 警报时的延迟

- 首先检查电子邮件中的 "垃圾邮件" 或 "垃圾邮件" 文件夹。
- 如果 **延迟来自多个文件或库的所有警报**，请访问 [服务运行状况仪表板](https://portal.office.com/adminportal/home?ref=/servicehealth) ，以检查任何可能与 SharePoint 或 Exchange 发生的咨询/事件。 问题可能与 SharePoint 通知功能或通过 Exchange 的电子邮件延迟有关。 此外，请注意是否正在传递其他电子邮件—如果不是，则问题可能与 Exchange 延迟有关。
- 如果 **未传递来自特定文件或库的单个警报**，请尝试删除并重新创建它。 请参阅 [管理、查看或删除 SharePoint 警报](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) 以重新创建警报。

> [!NOTE]
> - 无法将通知发送到通讯组。 仅支持 Security 和 O365 组。
> - 您不能自定义警报电子邮件模板。 必须使用 Microsoft Flow 或 SharePoint Designer 工作流来实现这些。
