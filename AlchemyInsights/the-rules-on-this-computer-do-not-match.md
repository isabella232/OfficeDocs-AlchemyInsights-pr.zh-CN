---
title: 错误：此计算机上规则不匹配
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: b77573e9d94195e1f0ef4a1566c45a30d53b7e68e502aeb834e2ca5b9e6c5c76
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981103"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>错误：此计算机上规则不匹配

To see updated status of this known issue， see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Outlook团队在内部版本 12928.10000 中实施了修补程序。 修复程序已在预览体验成员 - 快，并将于 2020 年 6 月底转到每月频道。 获得固定版本后，你最后一次可能会收到提示"要保留哪些规则"。 在系统提示时选择"服务器"，然后返回到Outlook，然后重新启用任何已禁用的规则。

在修补程序可用之前，请使用以下解决方法：

**解决方法**：最近的报告中，仅针对在桌面版中创建客户端规则Outlook问题。 如果您继续遇到此问题，请考虑删除规则，然后仅在 OWA (Outlook Web App) 创建和编辑规则，直到问题得到解决。

如果无法手动删除规则，则可以通过运行 Outlook /cleanrules 来Outlook运行 Outlook.exe 命令。 这将同时删除客户端和服务器规则。 它将删除"帐户配置文件"中所有帐户Outlook规则。 命令行开关一文进一步记录了此命令。

