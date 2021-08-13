---
title: 恢复不再位于"已删除邮件"文件夹中的项目
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/2/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "7320"
ms.openlocfilehash: 81a7a2e9623c788743fad99e15c4d771bb12a6c1c81f35a9d2a6a0729ecf8db7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062326"
---
# <a name="recover-an-item-thats-no-longer-in-your-deleted-items-folder"></a>恢复不再在"已删除邮件"文件夹中的项目

If you can't find an item in the Deleted Items folder， the next place to look is the Recoverable Items folder. 这是一个隐藏文件夹，当：
- 它们将从"已删除邮件"文件夹中删除。
- "已删除邮件"文件夹由您或 IT 管理员设置的策略清空。
- You delete an item by selecting it and pressing **Shift+Delete**.

若要查看和恢复已移动到"可恢复的项目"文件夹的项目，
1. 在 Web 浏览器中使用组织电子邮件管理者提供的 URL 登录到 Outlook Web App。 输入用户名和密码，然后选择"**登录"。**
1. 在电子邮件文件夹列表中，右键单击"**已删除邮件"，** 然后选择 **"恢复已删除邮件..."。**
1. 如有必要，使用搜索框查找要恢复的项目。
1. 找到项目后，选择它，**然后单击恢复。**
   恢复的项目将移动到每个项目类型的默认位置。
    - 邮件转到收件箱。
    - 日历项目将转到您的日历。
    - 联系人转到"联系人"文件夹。
    - 任务转到"任务"文件夹。

**使用技巧"可恢复的项目"文件夹中的项目**

- "可恢复的项目"文件夹中项目的删除日期是项目移动到"已删除邮件"文件夹时的日期。 这不是将项目移动到"可恢复的项目"文件夹的日期。
- "可恢复的项目"文件夹中的项目没有图标，因此看起来都非常相似。
    - 如果要查找联系人，请查找具有该联系人姓名但没有主题行的项目。
    - 如果要查找日历约会，请查找没有人员姓名或主题行的项目。
    - 如果要查找联系人、日历约会或任务查找该项目的文本。
- 若要恢复多个项目，请将鼠标悬停在每个项目上，然后选中它旁边的复选框，单击"恢复 **"。** 还可以恢复多个相邻项目，方法为选中第一个项目的复选框，按住 **Shift** 键，然后选中最后一个项目的复选框。 选择所有项目后，选择"恢复 **"。**
- 你可以清除"恢复已删除 **项目"列表中的** 项目。 只需选择该项目，然后选择"清除 **"。** 如果清除某个项目，将不能使用"恢复已删除的项目"将其恢复。 清除邮件不会将其从清除之前进行的任何备份中删除。
- 您的组织可能已经指定"可恢复的项目"文件夹中的项目可用于恢复的长时间。 例如，可能有一个策略删除已删除邮件文件夹中 30 天的所有内容，还有另一个策略允许你恢复"可恢复的项目"文件夹中的项目，最多再保留 14 天。
