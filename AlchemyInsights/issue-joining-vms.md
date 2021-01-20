---
title: 加入虚拟机的问题
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884557"
---
# <a name="issue-joining-vms"></a>加入虚拟机的问题

要解决加入虚拟机时出现的问题，请执行以下步骤：

1. 试试使用 **UPN** 格式（例如，“joeuser@contoso.com”）来代替 **SAMAccountName** 格式 ('CONTOSO\joeuser')。
2. 确保你已经按照 *入门* 中所列步骤启用了密码同步。
3. 确保受影响的用户账户不是 Azure AD 租户中的外部账户。 外部用户无法登陆到托管的域，因为 Azure AD 域服务没有此类用户账户的凭据。
4. 如果受影响的用户账户是仅使用云的用户账户，请在启用 Azure AD 域服务后确保用户已经更改了他们的密码。 此步骤后，Azure AD 域服务所需的凭据哈希值将会生成。
5. 如果从本地目录中同步了受影响的用户，请确认推荐的 Azure AD Connect 版本已经进行过配置，以便进行完整的同步。
6. 如果在确认步骤 4 后问题仍然发生，请在你的同步机器上执行下列命令：
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.