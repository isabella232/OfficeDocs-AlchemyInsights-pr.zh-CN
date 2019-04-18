---
title: 在审核日志中标识 IP 地址和客户端
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 7e30a638de5926aa11b8ae637613a48076d7bdc9
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909063"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>在审核日志中标识 IP 地址和客户端

用户或管理员对应的活动的 IP 地址显示在审核日志中。 还记录客户端信息。 以下是确定此类信息的步骤

1. 登录到[Office 365 安全 & 合规中心](https://protection.office.com/)

2. 单击 "**搜索和调查**", 然后选择 "**审核日志搜索**"。

   如果你对特定活动感兴趣, 请从 "**活动**" 列表中选择该活动。 如果不是, 则将返回选定用户的所有活动 (默认设置)。

   **注意**: 某些活动可能在 "**活动**" 菜单中不可用;但是, 如果选择 "**显示所有活动的结果**", 则将返回这些审核项目 (默认设置)。

3. 在 "**用户**" 字段中指定用户名, 为活动选择适当的日期范围, 然后单击 "**搜索**"。

在结果中, 可以在 "结果" 窗格中看到该活动的 IP 地址。 选择 "审核记录" 可查看 "**详细**信息" 浮出控件中的详细信息 (例如, 客户端、执行操作的用户等)。

有关详细信息, 请参阅[查找用于访问已损坏帐户的计算机的 IP 地址](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account)。
