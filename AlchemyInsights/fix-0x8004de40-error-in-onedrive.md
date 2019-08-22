---
title: 修复 OneDrive 中的0x8004de40 错误
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525049"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>修复 OneDrive 中的0x8004de40 错误

如果您收到 OneDrive 的0x8004de40 错误:

- 在连接到您的 Acitve Directory 域时, 重新启动受影响的计算机。
- 如果重新启动不能解决问题, 请从 Azure AD 中脱离并重新加入设备。 

**注意**: 在执行这些步骤时, 您应在公司网络上。 如果无法连接到公司基础结构 (例如出差时), 请不要执行这些步骤。 

- 打开提升的命令提示符。 
- 若要打开提升的命令提示符, 请单击 "**开始**", 右键单击 "**命令提示符**", 然后单击 "**以管理员身份运行**"。
- 键入*dsregcmd/leave* , 然后按**enter**。
- 完成后, 键入*dsregcmd/join* , 然后按**enter**。
- 完成后, 关闭命令提示符。
- 重新启动计算机, 然后登录到 OneDrive。