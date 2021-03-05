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
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449056"
---
# <a name="password-synchronization"></a>密码同步

**密码哈希同步完全不起作用**

密码哈希同步不起作用时客户遇到的一些常见问题包括：

- Azure AD Connect 用于与本地 Active Directory 进行通信的 Active Directory帐户不会被授予复制目录更改和复制目录更改所有权限，密码同步需要这些权限 - 你需要通过向 Active Directory 帐户授予这些权限来解决此问题。
- 在管理员将用户 Sign-In 方法从密码同步更改为其他选项（如Azure AD Connect 向导中的 **AD FS** 联盟）后，密码哈希同步被禁用 - 可以通过在Azure AD Connect 向导中重新启用密码哈希同步功能来解决此问题。
- 本地 Active Directory 的连接问题。 例如，Azure AD Connect 无法访问某些域控制器，或者所需的端口被防火墙[](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports)阻止 - 你需要通过确保 Azure AD Connect 服务器和本地 Active Directory 之间的连接正常工作来解决此问题。
- Azure AD Connect 服务器当前处于暂存模式，这可能会导致服务器无法执行密码哈希 - 若要解决问题，请按照"Azure [AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)同步密码同步疑难解答"一节中介绍的步骤操作 - 不同步密码。

**密码哈希同步对部分用户不起作用**

1. 如果你注意到用户未同步密码哈希，请使用 Azure AD Connect中的疑难解答任务来调查和解决问题。 执行以下任务：

    a. [在向导中运行疑难解答任务](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [使用疑难解答 cmdlet 调查特定用途的密码哈希同步问题](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. 为用户启用本地 Active Directory 用户对象必须在下一次 **登录选项时更改** 密码。 启用此选项后，将为用户分配一个临时密码，并提示用户在下次登录时更改密码。 Azure AD Connect 不会将临时密码同步到 Azure AD。

若要解决上述问题，请执行以下任一任务：

- 要求用户登录到本地应用程序 (例如，Windows 桌面) 更改密码。 新密码将同步到 Azure AD。
- 让管理员更新用户密码，而不启用"用户下次登录时必须更改密码"选项，并与用户共享新密码。

3. 未正确为对象同步或密码同步配置本地Active Directory 用户对象。 若要解决此问题，请按照 Azure AD Connect 同步的密码哈希同步疑难解答 [中所述的步骤操作](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)。







