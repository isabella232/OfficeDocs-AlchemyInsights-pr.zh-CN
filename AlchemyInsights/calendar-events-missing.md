---
title: 日历事件缺失或未更新
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10932"
- "9001435"
ms.openlocfilehash: af45345bc8779489f5e00dcaee136103e674068e29c77d8c536d012f475c33c5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968666"
---
# <a name="calendar-events-missing-or-not-updating"></a>日历事件缺失或未更新

如果日历事件缺失或未更新，请首先在 Outlook 中查看日历文件夹属性中的项目计数： 

1. 右键单击受影响的用户 **日历** 文件夹，然后选择“**属性**”。

1. 选择“**同步**”选项卡。

如果服务器文件夹和脱机文件夹之间的项目计数不同：

1.  突出显示 **日历** 文件夹。

1.  转到“**发送**”/“**接收**”选项卡，然后选择“**更新文件夹**”。

如果仍未更新日历或缺少事件，请从 [Microsoft 下载中心](https://www.microsoft.com/download/details.aspx?id=28786)下载 Outlook 日历检查工具。 确定日历文件夹中的项目是否超过 5000 个，因为这可能导致日历会议未更新或会议错误等现象。 

有关详细信息，请参阅[缓存模式 .ost 或 .pst 文件中的项目或文件夹过多时的 Outlook 性能问题](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders)。