---
title: 密码同步
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 3cdde086e535d2397b4d1a8a66903121a5217015ca055fb9f8d025b0842f044b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960825"
---
# <a name="password-synchronization"></a>密码同步

**密码哈希同步完全不起作用**

密码哈希同步不起作用时客户遇到的一些常见问题包括：

- Azure AD 连接 用于与本地 Active Directory 通信的 Active Directory 帐户未被授予复制目录更改和复制目录更改所有权限，这是密码同步所需的权限 - 你需要通过向 Active Directory 帐户授予这些权限来解决此问题。
- 在管理员将用户 Sign-In 方法从"密码同步"更改为其他选项（如 Azure AD 连接 向导中的"与 **AD FS** 联盟"）后，将禁用密码哈希同步 -可以通过在 Azure AD 连接 向导中重新启用密码哈希同步功能来解决此问题。
- 本地 Active Directory 的连接问题。 例如，Azure AD 连接 无法访问某些域控制器，或者所需的端口被防火墙阻止 -[](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports)你需要通过确保 Azure AD 连接 服务器和本地 Active Directory 之间的连接正常工作来解决此问题。
- Azure AD 连接 服务器当前处于暂存模式，这可能会导致服务器无法执行密码哈希 - 若要解决问题，请按照使用[Azure AD 连接](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)同步解决密码同步疑难解答 - 没有同步密码部分中介绍的步骤操作。

**密码哈希同步对部分用户不起作用**

1. 如果你注意到用户的密码哈希未同步，请使用 Azure AD 连接中的疑难解答任务来调查和解决问题。 执行以下任务：

    a. [在向导中运行疑难解答任务](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [使用疑难解答 cmdlet 调查特定用途的密码哈希同步问题](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. 为"用户必须在下次登录时更改密码"选项启用本地 Active Directory **用户** 对象。 启用此选项后，将为用户分配一个临时密码，并提示用户在下次登录时更改密码。 Azure AD 连接不会将临时密码同步到 Azure AD。

若要解决以上问题，请执行以下任一任务：

- 要求用户登录本地应用程序 (例如，Windows桌面) 更改密码。 新密码将同步到 Azure AD。
- 让管理员更新用户密码，而不启用选项"用户下次登录时必须更改密码"，并与用户共享新密码。

3. 未针对对象同步或密码同步正确配置本地Active Directory 用户对象。 若要解决此问题，请按照密码哈希同步与 Azure [AD](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)密码哈希同步疑难解答中所述连接同步。







