---
title: 0x8004de40 OneDrive 时出现错误
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813642"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 OneDrive 时出现错误

如果在登录 OneDrive **0x8004de40** 收到错误消息，请重启计算机，同时连接到工作或学校域。 如果在重新启动后收到此错误，请在连接到工作或学校域时尝试以下操作：

1. 单击"开始"，在搜索框中键入 **cmd** 或命令提示符，右键单击命令提示符应用，然后选择"以 **管理员角色运行"。** 如果系统提示你输入管理员密码或进行确认，请键入密码，或单击"允许 **"。**  

2. 在命令提示符窗口中，键入 **dsregcmd /leave**  并等待命令完成。 然后键入 **dsregcmd /join** 并等待命令完成。
3. 重新启动计算机。
