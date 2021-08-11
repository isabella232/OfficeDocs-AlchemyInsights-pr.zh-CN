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
ms.openlocfilehash: 8d656d5660b7c6e6d32d32a06c3dbf49c45e4ca04c4422128f1c4ea62413afa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53967323"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>读取已删除事件的审核日志

下面将对此进行说明：

1. 转到安全Office 365[合规&中心](https://go.microsoft.com/fwlink/p/?linkid=2077143)。
1. 选择 **"搜索**  >  [**审核日志搜索"。**](https://go.microsoft.com/fwlink/?linkid=2103759)
    > [!NOTE]
    > 如果看到需要启用该功能的通知，请继续，然后现在打开它。 如果未启用此功能，搜索结果将无法从以前的日期提取数据。
1. 选择 **"活动**"，然后查找 **Exchange活动"**。 选择" **已删除邮件"文件夹中的** "已删除邮件"和" **将邮件移动到已删除邮件"** 文件夹选项。 完成后，在窗格外单击以最小化" **活动"** 窗格。
1. 指定日期范围，然后在"用户 **"框中，** 选择要调查的用户的用户名。 一次可以选择多个用户。
1. 选择“**搜索**”。 这些活动出现在“**结果**”下。
1. 若要查看详细信息，请选择一个活动， **然后选择详细信息**。 有关已删除项目的其他信息（如主题行和项目被删除时的位置）将显示在 **AffectedItems** 字段中。
    > [!NOTE]
    > You can't restore deleted items using the 审核日志 feature. 若要还原已删除的项目，请参阅恢复已删除项目[或电子邮件Outlook Web App。](https://go.microsoft.com/fwlink/?linkid=2103759)

若要了解更多信息，请参阅[搜索Office 365 审核日志常见方案疑难解答](https://go.microsoft.com/fwlink/?linkid=2103944)。
