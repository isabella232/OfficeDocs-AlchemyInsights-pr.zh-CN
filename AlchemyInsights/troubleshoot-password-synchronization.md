---
title: 密码同步疑难解答
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 165e0ff4b2136b727450946d2c47756ebee7d393
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353095"
---
# <a name="troubleshoot-password-synchronization"></a>密码同步疑难解答

若要解决没有与 Azure AD Connect 版本1.1.614.0 或更高版本同步的密码的问题, 请执行以下操作:
  
1. 使用 "以**管理员身份运行**" 选项在 Azure AD Connect 服务器上打开新的 Windows PowerShell 会话。

2. 运行**ExecutionPolicy RemoteSigned**或 ExecutionPolicy 不**受限制的设置**。

3. 启动 Azure AD Connect 向导。

4. 导航到 "**其他任务**" 页, 选择 "**疑难解答**", 然后单击 "**下一步**"。

5. 在 "疑难解答" 页上, 单击 "**启动" 以启动 PowerShell 中的 "疑难解答"** 菜单。

6. 在主菜单中, 选择 "**密码同步疑难解答**"。

7. 在子菜单中, 选择 "**密码同步" 根本不起作用**。

**了解故障排除任务的结果**
  
故障排除任务将执行以下检查:
  
- 验证是否已为 Azure AD 租户启用密码同步功能。

- 验证 Azure AD Connect 服务器是否未处于暂存模式。

- 对于每个现有的本地 Active Directory 连接器 (对应于现有的 Active Directory 林):

- 
  - 验证是否已启用密码同步功能。

  - 在 Windows 应用程序事件日志中搜索密码同步检测信号事件。

  - 对于内部部署 Active Directory 连接器下的每个 Active Directory 域:

  - 验证是否可以从 Azure AD Connect 服务器访问域。

  - 验证本地 Active Directory 连接器使用的 Active Directory 域服务 (AD DS) 帐户是否具有密码同步所需的正确用户名、密码和权限。

有关疑难解答密码同步的更多帮助, 请参阅[密码同步与 AZURE AD Connect Sync 疑难解答](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization)。
  