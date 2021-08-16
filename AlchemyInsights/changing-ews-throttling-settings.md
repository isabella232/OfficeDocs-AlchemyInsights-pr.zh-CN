---
title: 更改 EWS 限制设置
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: f99bb449b542760c6c8d51ee399c774fbe36e3f7f40520b5eb23f39d9d7c08dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968367"
---
# <a name="changing-ews-throttling-settings"></a>更改 EWS 限制设置

请运行我们的自动测试，该测试将允许你修改针对迁移持续时间的 EWS 限制策略。 请注意，即使运行之后，EWS 导入也仍然限制为每个邮箱每 5 分钟 150mb；若要达到更高的迁移吞吐量速度，请同时迁移更多用户。

请注意，EWS 限制策略更改对以下迁移类型没有影响（使用 Microsoft 工具）：混合、直接转换/暂存（RPC/HTTP）、IMAP、G 套件、公共文件夹或 PST 导入服务。