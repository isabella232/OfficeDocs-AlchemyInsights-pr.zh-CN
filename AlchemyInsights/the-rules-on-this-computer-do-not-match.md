---
title: 错误：此计算机上的规则不匹配
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c0982da82826d1644f437b19e0d343a59d7ac473
ms.sourcegitcommit: e09af4285c6b81ca0a5320fdb811713ac25748c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/09/2020
ms.locfileid: "44664236"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>错误：此计算机上的规则不匹配

若要查看此已知问题的更新状态，请参阅[此计算机上的规则与 Microsoft Exchange 上的规则不匹配](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Outlook 团队已在内部版本12928.10000 中实施了修补程序。 该修补程序已在有问必答内快速进行，并将于 6 2020 月6日后期进入每月频道。 获得固定生成后，您可能会收到提示 "您想要保留哪条规则" 一次。 出现提示时选择 "服务器"，然后返回到 Outlook 并重新启用已禁用的任何规则。

在修补程序可用之前，请使用以下解决方法：

**解决方法**：在最近的报告中，只有在 Outlook desktop 中创建了客户端规则的客户端才会出现此问题。 如果仍遇到问题，请考虑删除这些规则，然后仅在 OWA （Outlook Web App）中创建和编辑规则，直到问题得到解决。

如果您无法手动删除规则，则可以在通过运行/cleanrules. 启动 outlook 时运行 Outlook 命令。 这将同时删除客户端和服务器规则。 它将删除 Outlook 配置文件中所有帐户的所有规则。 命令行开关一文中会进一步介绍此命令。

