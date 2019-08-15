---
title: 未传递 SharePoint 通知通知
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: e682a1b3dbd0d3a1c2e52be725dd2b57fc66109a
ms.sourcegitcommit: a2c866d2f3cdc1e18a33a5b2a4209340e83ca3c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/14/2019
ms.locfileid: "36404792"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>未传递 SharePoint 通知通知

请检查电子邮件中的垃圾邮件文件夹, 有时会出现通知。

确定是否**未传递所有警报**, 或者是否未传递来自特定文件或库**的单个警报**。

- **不传递单个警报**: 如果未传递来自特定文件或库的单个通知, 则可以尝试删除并重新创建它。 请参阅[管理、查看或删除 SharePoint 警报](https://support.office.com/en-us/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=en-US&ad=US#ID0EAADAAA=Online)以重新创建警报。
- **未传递所有警报**: 如果未传递来自多个文件或库的所有警报, 请访问[服务运行状况仪表板](https://admin.microsoft.com/AdminPortal/Home#/servicehealth), 以检查 SharePoint 或 Exchange 可能发生的任何咨询/事件。 问题可能与 SharePoint 通知功能或通过 Exchange 的电子邮件延迟有关。 此外, 请务必注意是否正在传递其他电子邮件, 如果没有, 则可能是 Exchange 延迟问题。

有关警报的常见问题解答:

- 无法向通讯组发送通知, 仅支持安全和 O365 组。
- 您不能自定义通知电子邮件模板;您需要使用 Microsoft FLOW 或 SharePoint Designer 工作流来实现这些。

详细信息:

- **通知设置**: 有关设置通知的详细信息, 请参阅[创建通知以在 SharePoint 中的文件或文件夹发生更改时收到通知](https://support.office.com/en-us/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918)。
- **警报疑难解答**: 有关排除警报的详细信息, 请参阅[用户不接收 SharePoint Online 警报通知](https://docs.microsoft.com/en-us/sharepoint/support/sites/no-alert-notifications)。
- **高级 O365 合规性警报策略**: 有关设置这些警报的详细信息, 请参阅[合规性警报策略](https://docs.microsoft.com/en-us/office365/securitycompliance/alert-policies)。
- **SharePoint 和 OneDrive 审核日志**: 有关如何检索这些事件的详细信息, 请参阅[Search the Audit log](https://docs.microsoft.com/en-us/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)。
- **高级威胁防护发送的警报**: 请参阅[适用于 SharePoint 和 OneDrive 的 ATP](https://docs.microsoft.com/en-us/office365/securitycompliance/atp-for-spo-odb-and-teams)。
- **数据丢失防护策略发送的警报**: 请参阅[DLP 策略的电子邮件通知](https://docs.microsoft.com/en-us/office365/securitycompliance/use-notifications-and-policy-tips)。

## <a name="related-topics"></a>相关主题

想要在 SharePoint Online 中试用 Microsoft 流吗？

- [创建流](https://support.office.com/en-us/article/create-a-flow-for-a-list-or-library-in-sharepoint-online-or-onedrive-for-business-a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint 和流](https://flow.microsoft.com/en-us/blog/sharepoint-and-flow/)
