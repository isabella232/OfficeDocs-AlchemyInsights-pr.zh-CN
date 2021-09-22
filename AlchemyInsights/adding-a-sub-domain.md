---
title: 添加子域
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2021
ms.locfileid: "59475936"
---
# <a name="adding-a-sub-domain"></a>添加子域

子域可以添加到与父域相同的或不同的租户。 在任一情况下，都必须在注册机构网站上管理自己的 DNS 设置。 如果已允许 Microsoft 使用 NS 记录管理 DNS 设置，或者从 Microsoft 购买了域，则如果不首先更改此域，则不能添加子域。

首先添加父域，然后添加子域。 如果子域位于同一租户中，则无需其他验证。 如果向单独的租户添加子域，在添加域和所选服务的其他 DNS 记录之前，需要 DNS txt 记录才能进行所有权验证。

- 若要添加域或子域，请按照"添加域 [](https://admin.microsoft.com/Adminportal#/Domains/Wizard)"向导操作，或手动添加域或子域，方法为访问"设置域""  >    >  **添加域"。**

如有必要：

- 若要更改管理现有域的 DNS 设置的用户，请转到"设置域"，选中域旁边的复选框，然后选择  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains)"管理 **DNS"。** 在向导中， **选择"添加你自己的 DNS 记录** "并完成向导。
- 若要将子域添加到 Microsoft 购买的域，首先将域转移到另一个注册机构，然后进行上述更改以管理你自己的 DNS 记录。 有关说明，请参阅 [将域从 Microsoft 转移到另一台主机](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)。
- 如果您收到一条错误，指出您的域已被您组织的其他成员或人员使用，则首先需要接管此非托管帐户，然后才能使用该域。 有关说明，请参阅以管理员角色接管非托管[Azure Active Directory。](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover)
