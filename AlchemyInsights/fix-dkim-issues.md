---
title: 修复 DKIM 安装问题
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744940"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="c67c2-102">修复 DKIM 安装问题</span><span class="sxs-lookup"><span data-stu-id="c67c2-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="c67c2-103">如果您在为您的自定义域启用 DKIM 时遇到问题，请使用以下步骤：</span><span class="sxs-lookup"><span data-stu-id="c67c2-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="c67c2-104">大多数 DKIM 安装问题与不正确的 DNS 记录有关。</span><span class="sxs-lookup"><span data-stu-id="c67c2-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="c67c2-105">验证 DKIM CNAME 记录 (**不** 是 TXT 记录，) 格式是否正确。</span><span class="sxs-lookup"><span data-stu-id="c67c2-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="c67c2-106">有关详细信息，请参阅本 [主题](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)。</span><span class="sxs-lookup"><span data-stu-id="c67c2-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="c67c2-107">在您的域的 DNS 托管服务上创建或更新 DKIM DNS 记录之后 (通常情况下，您的域注册机构) ，等待 DNS 记录传播。</span><span class="sxs-lookup"><span data-stu-id="c67c2-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="c67c2-108">如果无法在管理中心创建 DKIM DNS 记录，则可以 \<CustomDomain\> 将其替换为自定义域 (例如，contoso.com) 并在 [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)中运行此命令： `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` 。</span><span class="sxs-lookup"><span data-stu-id="c67c2-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
