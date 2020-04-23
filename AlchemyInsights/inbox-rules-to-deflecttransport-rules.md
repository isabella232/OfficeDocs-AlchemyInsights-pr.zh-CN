---
title: 929 deflectTransport 规则的收件箱规则
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: 6b6e64c0332a579e8f6132b08f2f89b15eb4de27
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43724582"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="4bb00-102">邮件流规则（也称为传输规则）</span><span class="sxs-lookup"><span data-stu-id="4bb00-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="4bb00-103">邮件流规则的一般概述： [Exchange Online 中的邮件流规则（传输规则）](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="4bb00-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>

- <span data-ttu-id="4bb00-104">设置邮件流规则： [Exchange Online 中的邮件流规则过程](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="4bb00-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>

- <span data-ttu-id="4bb00-105">创建、修改和删除邮件流规则：[管理邮件流规则](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="4bb00-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>

<span data-ttu-id="4bb00-106">您还可以在 Exchange Online PowerShell 中管理邮件流规则。</span><span class="sxs-lookup"><span data-stu-id="4bb00-106">You can also manage mail flow rules in Exchange Online PowerShell.</span></span> <span data-ttu-id="4bb00-107">有关详细信息，请参阅[new-transportrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) （view）、 [new-transportrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) （创建）、 [New-transportrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) （删除）、 [new-transportrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) （修改现有）、 [disable-new-transportrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) （禁用现有）和[Enable-new-transportrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) （启用现有）。</span><span class="sxs-lookup"><span data-stu-id="4bb00-107">For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span>

<span data-ttu-id="4bb00-108">其他邮件流规则 cmdlet： [get-transportruleaction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) （列出可用操作）、 [get-transportrulepredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) （列出可用条件和例外）、[导出-export-transportrulecollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) （导出规则）和[export-transportrulecollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) （导入规则）。</span><span class="sxs-lookup"><span data-stu-id="4bb00-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span>
