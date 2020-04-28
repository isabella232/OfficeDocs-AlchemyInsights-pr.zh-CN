---
title: 使用传输规则进行加密
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 3f16c7e7be99a50cd57f47ea2801b3022c4aec95
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915045"
---
# <a name="encryption-with-transport-rules"></a><span data-ttu-id="13577-102">使用传输规则进行加密</span><span class="sxs-lookup"><span data-stu-id="13577-102">Encryption with transport rules</span></span>

<span data-ttu-id="13577-103">在 [Exchange 管理中心](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) 中，可使用邮件流规则中的 Office 邮件加密 (OME) 功能来触发邮件加密。</span><span class="sxs-lookup"><span data-stu-id="13577-103">In the [Exchange Admin Center](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), you can use Office Message Encryption(OME) capabilities in your mail flow rules to trigger message encryption.</span></span> <span data-ttu-id="13577-104">选择“传输规则”条件上的“**应用 Office 365 邮件加密和权限保护**”选项。</span><span class="sxs-lookup"><span data-stu-id="13577-104">Choose the **Apply Office 365 Message Encryption and rights protection** option on the Transport Rule condition.</span></span>

- <span data-ttu-id="13577-105">有关详细信息，请参阅[定义用于加密的邮件流规则](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)。</span><span class="sxs-lookup"><span data-stu-id="13577-105">For more information, see [Define Mail flow rule to encrypt](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

- <span data-ttu-id="13577-106">在 Powershell 中，使用 [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet 并将 *ApplyOME* 参数设置为 $true。</span><span class="sxs-lookup"><span data-stu-id="13577-106">In Powershell, use the [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet and set the *ApplyOME* parameter to $true.</span></span>
