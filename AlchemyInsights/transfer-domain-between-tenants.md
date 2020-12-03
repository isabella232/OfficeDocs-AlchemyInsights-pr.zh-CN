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
# <a name="transfer-domain-between-tenants"></a><span data-ttu-id="8069f-102">租户之间的转移域</span><span class="sxs-lookup"><span data-stu-id="8069f-102">Transfer domain between tenants</span></span>

<span data-ttu-id="8069f-103">可以手动从一个租户中删除自定义域（如 forthcoffee.com），然后在新的租户中进行验证。</span><span class="sxs-lookup"><span data-stu-id="8069f-103">A custom domain such as forthcoffee.com can be manually removed from one tenant and then verified in a new tenant.</span></span>

<span data-ttu-id="8069f-104">按照以下步骤 [删除域](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/remove-a-domain)。</span><span class="sxs-lookup"><span data-stu-id="8069f-104">Follow these steps to [Remove a domain](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/remove-a-domain).</span></span> <span data-ttu-id="8069f-105">然后在新租户中，转到 "**设置**  >  **域**" "  >  **添加域**"。</span><span class="sxs-lookup"><span data-stu-id="8069f-105">Then in the new tenant go to **Settings** > **Domains** > **Add domain**.</span></span>

<span data-ttu-id="8069f-106">有关更复杂的方案，请参阅 [Microsoft 365 租户到租户迁移](https://docs.microsoft.com/microsoft-365/enterprise/microsoft-365-tenant-to-tenant-migrations)。</span><span class="sxs-lookup"><span data-stu-id="8069f-106">For more complex scenarios, see [Microsoft 365 tenant-to-tenant migrations](https://docs.microsoft.com/microsoft-365/enterprise/microsoft-365-tenant-to-tenant-migrations).</span></span>

<span data-ttu-id="8069f-107">**另请注意**：</span><span class="sxs-lookup"><span data-stu-id="8069f-107">**Also note**:</span></span>
- <span data-ttu-id="8069f-108">无法在租户之间删除或移动初始 onmicrosoft.com 域。</span><span class="sxs-lookup"><span data-stu-id="8069f-108">The initial onmicrosoft.com domain cannot be deleted or moved between tenants.</span></span>
- <span data-ttu-id="8069f-109">无法在租户之间移动从 Microsoft 购买的自定义域。</span><span class="sxs-lookup"><span data-stu-id="8069f-109">A custom domain purchased from Microsoft cannot be moved between tenants.</span></span>