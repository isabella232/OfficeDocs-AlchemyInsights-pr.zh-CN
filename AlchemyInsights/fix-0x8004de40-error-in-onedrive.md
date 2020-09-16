---
title: 修复 OneDrive 中的0x8004de40 错误
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745120"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>修复 OneDrive 中的0x8004de40 错误

如果您收到 OneDrive 的0x8004de40 错误：

- 在连接到您的 Acitve Directory 域时，重新启动受影响的计算机。
- 如果重新启动不能解决问题，请从 Azure AD 中脱离并重新加入设备。 

**注意**：在执行这些步骤时，您应在公司网络上。 当您无法连接到公司基础结构时，请不要执行这些步骤 (例如，在旅行) 。 

- 打开提升的命令提示符。 
- 若要打开提升的命令提示符，请单击 " **开始**"，右键单击 " **命令提示符**"，然后单击 " **以管理员身份运行**"。
- 键入 *dsregcmd/leave* ，然后按 **enter**。
- 完成后，键入 *dsregcmd/join* ，然后按 **enter**。
- 完成后，关闭命令提示符。
- 重新启动计算机，然后登录到 OneDrive。