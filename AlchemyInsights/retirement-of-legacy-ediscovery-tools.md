---
title: 旧电子数据展示工具的退休
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 94cd2127240be5faacd397ba6255fdb16e364308
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/26/2020
ms.locfileid: "46902610"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>旧电子数据展示工具的退休

由于 Microsoft 365 合规性中心中新增和改进的电子数据展示功能的结果，以下旧的电子数据展示工具和 commandlet 将在接下来的几个月内退出：

- Exchange 管理中心内的[就地电子数据展示](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery)和[就地保留](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)。

- 支持就地电子数据展示和就地保留的 Exchange Online PowerShell cmdlet。  (这些 cmdlet 共同标识为 *-New-mailboxsearch cmdlet。 ) 这包括以下 cmdlet：

    - [新 New-mailboxsearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [启动-New-mailboxsearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [New-mailboxsearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [New-mailboxsearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Exchange Online PowerShell 中的 [搜索邮箱](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet。
- Exchange Web Services API 中的以下操作：
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [高级电子数据展示1.0 版](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**停用的时间线**：
- **2020 年7月1日** 您无法再创建新的搜索和保留，但您可以通过您自己的风险运行、编辑和删除现有搜索。 Microsoft 支持不再支持 EAC 中的就地电子数据展示 & 保留。
    
- **2020 年10月1日** 就地电子数据展示 & 保留 EAC 中的功能将被置于只读模式，因此您只能删除现有的搜索和保留。

**有关详细信息，请参阅**：

 - [将旧式电子数据展示搜索和保留迁移到 Microsoft 365 合规性中心](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [旧版电子数据展示工具的停用](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [有关就地电子数据展示和就地保留的常见问题解答](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



