---
title: 解决密码同步
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: c71fce8621057093d23891c26f7b0285fdc8b9ed
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28277698"
---
# <a name="troubleshoot-password-synchronization"></a>解决密码同步

若要解决其中没有密码都是同步与 Azure AD 连接版本 1.1.614.0 或更高版本的问题：
  
1. 使用**以管理员身份运行**选项打开新 Azure AD 连接服务器上的 Windows PowerShell 会话。 
    
2. 运行**Set-executionpolicy RemoteSigned**或**不受限制的 Set-executionpolicy**。 
    
3. 启动 Azure AD 连接向导。
    
4. 导航到 * * 其他任务 * * 页上，选择 * * Troubleshoot * *，，单击**下一步**。 
    
5. 在疑难解答页上，单击在 PowerShell 中的**启动启动疑难解答**菜单。 
    
6. 在主菜单中，选择**解决密码同步**。 
    
7. 在 sub 菜单中，选择**根本不起作用密码同步**。 
    
 **了解故障排除任务的结果**
  
故障排除任务可以执行以下检查：
  
- 验证已为您的 Azure AD 租户启用密码同步功能。
    
- 验证 Azure AD 连接服务器不是在调试模式。
    
- 对于每个现有内部部署 Active Directory 连接器 （其对应的现有的 Active Directory 林）：
    
- 
  - 验证已启用的密码同步功能。
    
  - 搜索的 Windows 应用程序事件日志中的密码同步检测信号事件。
    
  - 在内部部署 Active Directory 连接器下的每个 Active Directory 域：
    
  - 验证域从 Azure AD 连接服务器上可以访问。
    
  - 验证内部部署 Active Directory 连接器使用的 Active Directory 域服务 (AD DS) 帐户具有正确的用户名、 密码和所需的密码同步权限。
    
疑难解答密码同步的更多帮助，请参阅[Troubleshoot 与 Azure AD 连接同步的密码同步](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization)。
  

