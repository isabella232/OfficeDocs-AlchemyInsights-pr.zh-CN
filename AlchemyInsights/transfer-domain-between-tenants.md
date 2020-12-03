---
title: 租户之间的转移域
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/2/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002570"
- "7305"
ms.openlocfilehash: d696c9d095fb6b2b374d8c5872e94cc7e32dceb8
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/02/2020
ms.locfileid: "49560550"
---
# <a name="transfer-domain-between-tenants"></a>租户之间的转移域

可以手动从一个租户中删除自定义域（如 forthcoffee.com），然后在新的租户中进行验证。

按照以下步骤 [删除域](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/remove-a-domain)。 然后在新租户中，转到 "**设置**  >  **域**" "  >  **添加域**"。

有关更复杂的方案，请参阅 [Microsoft 365 租户到租户迁移](https://docs.microsoft.com/microsoft-365/enterprise/microsoft-365-tenant-to-tenant-migrations)。

**另请注意**：
- 无法在租户之间删除或移动初始 onmicrosoft.com 域。
- 无法在租户之间移动从 Microsoft 购买的自定义域。