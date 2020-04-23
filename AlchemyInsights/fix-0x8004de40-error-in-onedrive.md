---
title: 修复 OneDrive 中的0x8004de40 错误
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716018"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>修复 OneDrive 中的0x8004de40 错误

如果您收到 OneDrive 的0x8004de40 错误：

- 在连接到您的 Acitve Directory 域时，重新启动受影响的计算机。
- 如果重新启动不能解决问题，请从 Azure AD 中脱离并重新加入设备。 

**注意**：在执行这些步骤时，您应在公司网络上。 如果无法连接到公司基础结构（例如出差时），请不要执行这些步骤。 

- 打开提升的命令提示符。 
- 若要打开提升的命令提示符，请单击 "**开始**"，右键单击 "**命令提示符**"，然后单击 "**以管理员身份运行**"。
- 键入*dsregcmd/leave* ，然后按**enter**。
- 完成后，键入*dsregcmd/join* ，然后按**enter**。
- 完成后，关闭命令提示符。
- 重新启动计算机，然后登录到 OneDrive。