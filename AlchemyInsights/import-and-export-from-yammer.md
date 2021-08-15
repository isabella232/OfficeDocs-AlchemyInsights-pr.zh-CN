---
title: 从 Yammer 导入和导出
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: 3ead2702c2fbd26b2e5596e26e9189c2f97baf93c93ec3cbd57f15c855b5128e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54001462"
---
# <a name="import-and-export-from-yammer"></a>从 Yammer 导入和导出

**导入**

根据你的 Yammer 网络是否处于[适用于 Microsoft 365 的本机模式](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)，用户导入选项会有所不同。

- **非本机模式**：可以使用组设置中的“[从地址簿添加](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294)”（最多 100 个用户）将用户导入组，或在“网络管理”中使用“[批量更新](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users)”将用户导入网络。
- **本机模式**：组成员资格和网络成员资格操作应从 [Microsoft 365 管理门户网站](https://docs.microsoft.com/microsoft-365/admin/add-users)、[Azure AD 门户网站](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)或使用其他 Azure AD 选项执行。 本机模式下的网络不可再访问批量更新和其他旧版功能。

> [!IMPORTANT]
> 即使在另一个网络中使用了数据导出功能，Yammer 也不支持从“网络管理”中导入内容。 可通过合作伙伴解决方案或 Yammer REST API 重新发布内容。

**导出**

[在“网络管理”中导出网络数据](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data)允许从 Yammer 网络导出内容，包括消息和文件。 附件可能很大，并且会导致需要花费大量时间才能完成导出。 我们建议使用[数据导出 API](https://developer.yammer.com/docs/data-export-api) 按区块导出每天或每周的活动网络。 Microsoft 支持不会为此提供自定义脚本。

存在单独的 [GDPR 导出](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise)，用于导出单个用户的内容。