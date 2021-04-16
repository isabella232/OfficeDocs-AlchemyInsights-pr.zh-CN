---
title: 使用传输规则进行加密
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
- "9002635"
- "5154"
ms.openlocfilehash: dfd77bc83b4b278e3630858f54fdfb109ade2a14
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813858"
---
# <a name="encryption-with-transport-rules"></a><span data-ttu-id="9a2be-102">使用传输规则进行加密</span><span class="sxs-lookup"><span data-stu-id="9a2be-102">Encryption with transport rules</span></span>

<span data-ttu-id="9a2be-103">在 [Exchange 管理中心](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) 中，可使用邮件流规则中的 Office 邮件加密 (OME) 功能来触发邮件加密。</span><span class="sxs-lookup"><span data-stu-id="9a2be-103">In the [Exchange Admin Center](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), you can use Office Message Encryption(OME) capabilities in your mail flow rules to trigger message encryption.</span></span> <span data-ttu-id="9a2be-104">选择“传输规则”条件上的“**应用 Office 365 邮件加密和权限保护**”选项。</span><span class="sxs-lookup"><span data-stu-id="9a2be-104">Choose the **Apply Office 365 Message Encryption and rights protection** option on the Transport Rule condition.</span></span>

- <span data-ttu-id="9a2be-105">有关详细信息，请参阅[定义用于加密的邮件流规则](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)。</span><span class="sxs-lookup"><span data-stu-id="9a2be-105">For more information, see [Define Mail flow rule to encrypt](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

- <span data-ttu-id="9a2be-106">在 Powershell 中，使用 [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet 并将 *ApplyOME* 参数设置为 $true。</span><span class="sxs-lookup"><span data-stu-id="9a2be-106">In Powershell, use the [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet and set the *ApplyOME* parameter to $true.</span></span>
