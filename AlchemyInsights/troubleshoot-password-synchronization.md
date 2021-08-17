---
title: 密码同步疑难解答
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105738"
---
# <a name="troubleshoot-password-synchronization"></a>密码同步疑难解答

若要解决密码同步问题，请首先使用此 AAD 连接疑难解答任务来确定密码未同步的原因。 若要开始，请转到管理 [直接同步](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)。  

1. 在 Azure AD Windows PowerShell服务器上打开新的 连接 会话，然后选择"以 **管理员方式运行"** 选项。

2. 运行Set-ExecutionPolicy RemoteSigned 或 Set-ExecutionPolicy Unrestricted。

3. 启动 Azure AD 连接向导。

4. 转到"其他任务"页>**下一**  >  **步疑难解答"。**

5. 选择 **"** 启动"以打开 PowerShell 疑难解答菜单。

6. 选择 **密码同步疑难解答**。

    问题通常是特定用户帐户的密码未同步。

    **备注** 如果上次成功执行的密码同步是之前的时间，则密码同步将失败。

有关密码同步疑难解答的更多帮助，请参阅 Troubleshoot [password hash synchronization with Azure AD 连接 sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)。