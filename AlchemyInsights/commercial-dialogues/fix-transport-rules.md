---
title: 修复传输规则
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736152"
---
# <a name="fix-transport-rules"></a>修复传输规则

自定义邮件流规则影响此邮件。 若要查看确切的规则，请执行下列操作：

1. 在提交结果中的" **其他信息"下**，记下 **GUID** 或 **策略名称**。
2. 启动 Exchange 命令行管理程序。 有关详细信息，请参阅[Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432)。
3. 使用提交 (GUID 运行此命令  **) ：Get-TransportRule -identity "GUID" | fl * Description***
4. 查看说明以查看影响邮件的已配置条件。

若要了解更多信息，请参阅 [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523)。
