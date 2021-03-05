---
title: 读取已删除事件的审核日志
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464370"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>读取已删除事件的审核日志

下面是如何进行此操作：

1. 转到 [Office 365 安全&合规中心](https://go.microsoft.com/fwlink/p/?linkid=2077143)。
1. 选择 **"搜索**  >  [**审核日志搜索"。**](https://go.microsoft.com/fwlink/?linkid=2103759)
    > [!NOTE]
    > 如果看到需要打开该功能的通知，请继续，然后现在将其打开。 如果未启用此功能，搜索结果将无法从以前的日期提取数据。
1. 选择 **"** 活动"，然后查找 **Exchange 邮箱活动**。 选择 **"已删除邮件"文件夹中的** "已删除邮件"和"将邮件 **移动到已删除邮件"** 文件夹选项。 完成后，单击窗格外部以最小化 **"活动"** 窗格。
1. 指定日期范围，然后在"用户"框中，选择要调查的用户的用户名。 一次可以选择多个用户。
1. 选择 **"搜索"。** 活动显示在"结果 **"下**。
1. 若要查看详细信息，请选择一个活动，然后选择 **"详细信息"。** 有关已删除项目的其他信息（如主题行和项目被删除时的位置）将显示在 **AffectedItems** 字段中。
    > [!NOTE]
    > 你无法还原使用"已删除邮件"功能审核日志项目。 若要还原已删除的项目，请参阅"恢复已删除项目"[或Outlook Web App。](https://go.microsoft.com/fwlink/?linkid=2103759)

若要了解更多信息，请参阅["搜索 Office 365 审核日志排查常见方案。](https://go.microsoft.com/fwlink/?linkid=2103944)
