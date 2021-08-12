---
title: 0x8004de40时出现错误OneDrive
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
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946569"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40时出现错误OneDrive

如果在登录到 0x8004de40时收到OneDrive错误，请重新启动计算机，同时连接到工作或学校域。 如果在重新启动后收到此错误，请在连接到工作或学校域时尝试以下操作：

1. 单击"开始"，在搜索框中键入 **cmd** 或命令提示符，右键单击命令提示符应用，然后选择"以 **管理员角色运行"。** 如果系统提示你输入管理员密码或进行确认，请键入密码，或单击"允许 **"。**  

2. 在命令提示符窗口中，键入 **dsregcmd /leave**  并等待命令完成。 然后键入 **dsregcmd /join** 并等待命令完成。
3. 重新启动计算机。
