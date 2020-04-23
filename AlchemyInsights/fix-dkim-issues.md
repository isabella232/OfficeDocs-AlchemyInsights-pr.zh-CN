---
title: 修复 DKIM 安装问题
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717552"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="e93fd-102">修复 DKIM 安装问题</span><span class="sxs-lookup"><span data-stu-id="e93fd-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="e93fd-103">如果您在为您的自定义域启用 DKIM 时遇到问题，请使用以下步骤：</span><span class="sxs-lookup"><span data-stu-id="e93fd-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="e93fd-104">大多数 DKIM 安装问题与不正确的 DNS 记录有关。</span><span class="sxs-lookup"><span data-stu-id="e93fd-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="e93fd-105">验证 DKIM CNAME 记录（**而不**是 TXT 记录）的格式是否正确。</span><span class="sxs-lookup"><span data-stu-id="e93fd-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="e93fd-106">有关详细信息，请参阅本[主题](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)。</span><span class="sxs-lookup"><span data-stu-id="e93fd-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="e93fd-107">在您的域的 DNS 托管服务（通常是您的域注册机构）中创建或更新 DKIM DNS 记录后，请等待 DNS 记录传播。</span><span class="sxs-lookup"><span data-stu-id="e93fd-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="e93fd-108">如果无法在管理中心创建 DKIM DNS 记录，则可以\<将 CustomDomain\>替换为自定义域（例如，contoso.com），并在[Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)中运行此命令：。 `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`</span><span class="sxs-lookup"><span data-stu-id="e93fd-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
