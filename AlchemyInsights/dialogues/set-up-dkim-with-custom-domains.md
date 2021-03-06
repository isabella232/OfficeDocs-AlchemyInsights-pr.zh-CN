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
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500685"
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
> [!NOTE]
> **DomainGUID** 是自定义域 (（例如，域域的 contoso-com）的自定义 MX 记录中 **.mail.protection.outlook.com** 左侧 **的文本** contoso.com) 。 **InitialDomain** 是注册 Office 365 时所使用的域 (例如，contoso.onmicrosoft.com) 。 

有关 DNS 记录详细信息，请参阅在任何 DNS 托管提供商处为 [Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)创建 DNS 记录。