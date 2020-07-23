---
title: 密码同步疑难解答
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387867"
---
# <a name="troubleshoot-password-synchronization"></a>密码同步疑难解答

若要解决密码同步问题，请使用此 AAD Connect 故障排除任务开始，以确定密码未同步的原因。 若要开始，请转到[管理直接同步](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)。  

1. 在 Azure AD Connect 服务器上打开一个新的 Windows PowerShell 会话，然后选择 "**以管理员身份运行**" 选项。

2. 运行 ExecutionPolicy RemoteSigned 或 ExecutionPolicy 不受限制的设置。

3. 启动 Azure AD Connect 向导。

4. 转到 "其他任务" 页**Troubleshoot**>  >  **下一步**解决问题。

5. 选择 "**启动**" 以打开 PowerShell 故障排除菜单。

6. 选择 "**密码同步疑难解答**"。

    问题通常是不会为特定用户帐户同步密码。

    **备注**如果上一次成功的密码同步曾经过一次，则密码同步将失败。

有关疑难解答密码同步的更多帮助，请参阅[密码哈希同步与 AZURE AD Connect Sync 疑难解答](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)。