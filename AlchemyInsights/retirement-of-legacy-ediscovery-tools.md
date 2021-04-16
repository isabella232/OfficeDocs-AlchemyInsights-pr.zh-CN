---
title: 停用旧版电子数据展示工具
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
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798539"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>停用旧版电子数据展示工具

作为 Microsoft 365 合规中心中新增和改进电子数据展示功能的结果，以下旧版电子数据展示工具和命令let 将在几个月后停用：

- [Exchange 管理中心中的](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) 就 [地](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) 电子数据展示和就地保留。

- 支持电子数据展示和保留In-Place Exchange Online PowerShell In-Place cmdlet。  (这些 cmdlet 统称为 *-MailboxSearch cmdlet。) 包括以下 cmdlet：

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Exchange Online PowerShell 中的 [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet。
- Exchange Web 服务 API 中的以下操作：
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [高级电子数据展示 v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**停用时间线**：
- **2020 年 7 月 1 日** 你无法再创建新的搜索和保留，但可以自行承担运行、编辑和删除现有搜索的风险。 Microsoft 支持不再支持In-Place EAC &电子数据展示保留。
    
- **2020 年 10** 月 1 In-Place EAC 中的电子数据展示 & 保留功能将置于只读模式，因此只能删除现有搜索和保留。

**有关详细信息，请参阅**：

 - [将旧版电子数据展示搜索和保留迁移到 Microsoft 365 合规中心](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [旧版电子数据展示工具的停用](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [有关电子数据展示In-Place保留的常见问题In-Place常见问题](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



