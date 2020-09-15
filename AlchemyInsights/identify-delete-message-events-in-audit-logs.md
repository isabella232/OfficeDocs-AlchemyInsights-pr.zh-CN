---
title: 确定审核日志中的删除邮件事件
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696503"
---
# <a name="audit-logs-for-deleted-email-messages"></a>已删除电子邮件的审核日志

从2019年1月起，Microsoft 将默认启用邮箱审核日志记录。 否则，若要查看特定用户的删除邮件事件，需要手动启用审核的删除操作。 如果已为您的组织或特定用户启用邮箱审核日志记录，请执行以下步骤。

1. 登录到 [Microsoft 365 安全 & 合规中心](https://protection.office.com/)

2. 单击 " **搜索和调查** "，然后选择 " **审核日志搜索**"。

3. 在 " **开始日期** " 和 " **结束日期** " 字段中选择日期范围。 指定要调查的用户 () 删除这些项目的用户的用户名。 在 " **活动** " 字段中，选择 " **已删除邮件" 文件夹** ，并 **将邮件移动到 "已删除**邮件" 文件夹。

4. 单击"搜索"。

在结果中，选择一个审核记录。 在 "详细信息" 浮出控件中，单击 " **详细信息**"。 有关已删除项目的其他信息 (例如，在删除项目时主题行和项目的位置) 显示在 " **AffectedItems** " 字段中。 **ClientInfoString**属性将显示在 outlook 中是否进行了删除、outlook 网页上 (以前称为 Outlook web App) 或任何其他设备。

有关详细信息，请参阅 [确定为邮箱设置电子邮件转发](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)。

**注意**：不能使用 "审核日志" 功能检索已删除的项目。 若要在 web 上的 Outlook 中检索已删除的邮件，请参阅 [在 Outlook Web App 中恢复已删除的项目](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)。
