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
ms.openlocfilehash: 7dd9c98bd45c29702fbc6cc14bf82bf7bce7d89d
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630059"
---
# <a name="audit-logs-for-deleted-email-messages"></a>已删除电子邮件的审核日志

从 2019 年 1 月开始，Microsoft 默认启用邮箱审核日志记录。 否则，若要查看特定用户的删除邮件事件，需要手动启用删除操作进行审核。 如果已针对您的组织或特定用户启用邮箱审核日志记录，请按照以下步骤操作。

1. 登录到 Microsoft 365[合规中心](https://protection.office.com/)

2. 单击 **"搜索和调查"，** 然后选择"**审核日志搜索"。**

3. 在"开始日期"和"结束日期 **"** 字段中 **选择日期** 范围。 指定要调查的用户的用户名 (已删除项目的用户) 。 在" **活动"** 字段中， **选择"已删除邮件"文件夹中** 的"已删除邮件"和"将 **邮件移动到已删除邮件"文件夹**。

4. 单击"搜索"。

在结果中，选择审核记录。 在详细信息飞出中，单击 **"详细信息"。** 有关已删除项目的其他信息 (，例如主题行和项目在删除项目时) 显示在 **AffectedItems** 字段中。 **ClientInfoString** 属性将显示删除是否发生在 Outlook、Outlook 网页版 (以前Outlook Web App) 设备中。

有关详细信息，请参阅确定 [谁为邮箱设置了电子邮件转发](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)。

**注意**：无法检索使用"已删除邮件"功能审核日志项。 若要检索邮件中的已删除Outlook 网页版，请参阅恢复邮件中的已删除[Outlook Web App。](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)
