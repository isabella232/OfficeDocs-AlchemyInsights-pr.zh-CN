---
title: 启动 OneDrive 时出现0x8004de40 错误
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/30/2020
ms.locfileid: "48815967"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>启动 OneDrive 时出现0x8004de40 错误

如果你在登录 OneDrive 时收到错误 **0x8004de40** ，请在连接到你的工作或学校域时重新启动计算机。 如果重新启动后收到此错误，请在连接到工作或学校域时尝试以下操作：

1. 单击 "开始"，在 "搜索" 框中键入 **cmd** 或 **命令提示符**  ，右键单击 "命令提示符" 应用，然后选择 "  **以管理员身份运行** "。 如果系统提示您输入管理员密码或进行确认，请键入密码或单击 " **允许** "。  

2. 在命令提示符窗口中，键入 **dsregcmd/leave**  并等待该命令完成。 然后键入 **dsregcmd/join** 并等待该命令完成。
3. 重新启动计算机。
