---
title: 确定审核日志中的删除邮件事件
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 93f8a192af6e689e2b2d04013f35b8da2b69e607
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909061"
---
# <a name="audit-logs-for-deleted-email-messages"></a>已删除电子邮件的审核日志

从2019年1月起, Microsoft 将默认启用邮箱审核日志记录。 否则, 若要查看特定用户的删除邮件事件, 需要手动启用审核的删除操作。 如果已为您的组织或特定用户启用邮箱审核日志记录, 请执行以下步骤。

1. 登录到[Office 365 安全 & 合规中心](https://protection.office.com/)

2. 单击 "**搜索和调查**", 然后选择 "**审核日志搜索**"。

3. 在 "**开始日期**" 和 "**结束日期**" 字段中选择日期范围。 指定要调查的用户的用户名 (删除这些项目的用户)。 在 "**活动**" 字段中, 选择 "**已删除邮件" 文件夹**, 并**将邮件移动到 "已删除**邮件" 文件夹。

4. 单击"搜索"。

在结果中, 选择一个审核记录。 在 "详细信息" 浮出控件中, 单击 "**详细信息**"。 在 " **AffectedItems** " 字段中显示有关已删除项目的其他信息 (例如, 在删除项目时的主题行和位置)。 **ClientInfoString**属性将显示在 outlook、outlook 网页 (以前称为 Outlook web App) 或任何其他设备上是否发生了删除。

有关详细信息, 请参阅[确定为邮箱设置电子邮件转发](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items)。

**注意**: 不能使用 "审核日志" 功能检索已删除的项目。 若要在 web 上的 Outlook 中检索已删除的邮件, 请参阅[在 outlook web App 中恢复已删除的项目](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)。
