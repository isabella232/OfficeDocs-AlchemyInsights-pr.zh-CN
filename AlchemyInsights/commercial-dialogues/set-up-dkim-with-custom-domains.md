---
title: 使用自定义域设置 DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735505"
---
# <a name="set-up-dkim-with-custom-domains"></a><span data-ttu-id="da4f5-102">使用自定义域设置 DKIM</span><span class="sxs-lookup"><span data-stu-id="da4f5-102">Set up DKIM with custom domains</span></span>

<span data-ttu-id="da4f5-103">您必须为 DNS 中每个自定义域发布两条 CNAME 记录。</span><span class="sxs-lookup"><span data-stu-id="da4f5-103">You must publish two CNAME records for each custom domain in DNS.</span></span> <span data-ttu-id="da4f5-104">为此，请使用以下格式：</span><span class="sxs-lookup"><span data-stu-id="da4f5-104">To do this, use the following format:</span></span>

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> <span data-ttu-id="da4f5-105">**DomainGUID** 是自定义域的自定义 MX 记录中 **.mail.protection.outlook.com** 左侧的文本 (例如，域域的 contoso-com **contoso.com) 。**</span><span class="sxs-lookup"><span data-stu-id="da4f5-105">**DomainGUID** is the text to the left of **.mail.protection.outlook.com** in the customized MX record for the custom domain (for example, contoso-com for the domain **contoso.com**).</span></span> <span data-ttu-id="da4f5-106">**InitialDomain** 是注册 Office 365 域时所使用的域 (例如，contoso.onmicrosoft.com) 。 </span><span class="sxs-lookup"><span data-stu-id="da4f5-106">**InitialDomain** is the domain you used when you signed up for Office 365 (for example, **contoso.onmicrosoft.com**).</span></span>

<span data-ttu-id="da4f5-107">有关 DNS 记录详细信息，请参阅在任何 DNS 托管提供商处为 [Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)创建 DNS 记录。</span><span class="sxs-lookup"><span data-stu-id="da4f5-107">For more information about DNS records, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>