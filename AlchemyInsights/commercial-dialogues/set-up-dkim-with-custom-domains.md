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
ms.openlocfilehash: cb1f621dffc88464c339b55998efb5440cfd775c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332297"
---
# <a name="set-up-dkim-with-custom-domains"></a>使用自定义域设置 DKIM

您必须为 DNS 中每个自定义域发布两条 CNAME 记录。 为此，请使用以下格式：

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
**注意****：DomainGUID** 是 **自定义域的自定义** MX 记录中 .mail.protection.outlook.com 左侧的文本 (例如，域 contoso.com) 。  **InitialDomain** 是注册域时所使用的域Office 365 (例如 **，contoso.onmicrosoft.com) 。**

有关 DNS 记录详细信息，请参阅在任何[DNS](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)托管提供商上为 dns Office 365。