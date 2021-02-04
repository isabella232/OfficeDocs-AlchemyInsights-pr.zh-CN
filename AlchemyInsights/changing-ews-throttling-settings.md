---
title: 更改 EWS 限制设置
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075887"
---
# <a name="changing-ews-throttling-settings"></a>更改 EWS 限制设置

请运行我们的自动测试，该测试将允许你修改针对迁移持续时间的 EWS 限制策略。 请注意，即使运行之后，EWS 导入也仍然限制为每个邮箱每 5 分钟 150mb；若要达到更高的迁移吞吐量速度，请同时迁移更多用户。

请注意，EWS 限制策略更改对以下迁移类型没有影响（使用 Microsoft 工具）：混合、直接转换/暂存（RPC/HTTP）、IMAP、G 套件、公共文件夹或 PST 导入服务。