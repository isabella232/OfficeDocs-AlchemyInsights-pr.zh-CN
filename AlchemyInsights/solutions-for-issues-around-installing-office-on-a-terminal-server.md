---
title: 关于在终端服务器上安装 office 的问题的解决方案
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 85f24284-af6f-4624-b6be-901a4a9206eb
ms.openlocfilehash: df1a50031196fbd79662cee620fc41c7be14e179
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47738447"
---
# <a name="solutions-for-issues-around-installing-office-on-a-terminal-server"></a>关于在终端服务器上安装 office 的问题的解决方案

若要使用共享计算机激活，您必须具有包含适用于企业的 Microsoft 365 应用程序的订阅。
  
- 验证是否已启用共享计算机激活
- 验证激活是否成功
- 查看共享计算机激活的错误消息：
- "我们在你的帐户中找到的产品不能用于在共享计算机方案中激活 Office"
  
此错误表示你没有包含适用于企业的 Microsoft 365 应用程序的订阅。

"未经许可的产品"

- 检查是否为用户分配了适用于企业的 Microsoft 365 应用的许可证。
- 检查用户是否使用其用户帐户登录。
- 确认共享计算机和 Internet 之间具有可靠连接。

有关其他故障排除提示，请参阅： [排查共享计算机激活的问题](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)