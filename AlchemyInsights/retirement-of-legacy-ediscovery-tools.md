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
ms.openlocfilehash: 2e7f898ac1a9e9469f633192be18e2a3a362023c83c9e510593196b5a4a0daf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074637"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>停用旧版电子数据展示工具

由于 Microsoft 365 合规中心中新增和改进了电子数据展示功能，以下旧版电子数据展示工具和命令let 将在几个月后停用：

- [管理中心](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery)中的就地电子数据展示[](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)和Exchange保留。

- 支持Exchange Online电子数据展示和保留In-Place PowerShell cmdlet In-Place。  (这些 cmdlet 统称为 *-MailboxSearch cmdlet。) 包括以下 cmdlet：

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- PowerShell 中的[Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet Exchange Online。
- web 服务 API 中的Exchange操作：
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**停用时间线**：
- **2020 年 7 月 1 日** 你无法再创建新的搜索和保留，但可以自行承担运行、编辑和删除现有搜索的风险。 Microsoft 支持不再支持In-Place EAC &电子数据展示保留。
    
- **2020 年 10** 月 1 In-Place EAC 中的电子数据展示 & 保留功能将置于只读模式，因此只能删除现有搜索和保留。

**有关详细信息，请参阅**：

 - [将旧版电子数据展示搜索和保留迁移到Microsoft 365 合规中心](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [旧版电子数据展示工具的停用](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [有关电子数据展示In-Place保留的常见问题In-Place常见问题](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



