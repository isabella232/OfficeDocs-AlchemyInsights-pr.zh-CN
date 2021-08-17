---
title: 设置 DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108546"
---
# <a name="setup-dkim"></a>设置 DKIM

有关为自定义域中的自定义域配置 DKIM 的完整Microsoft 365[请参阅此处](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)。

1. 对于每个 **自定义** 域，需要在域的 DNS 托管服务中创建两个 **DKIM** CNAME 记录 (通常是域注册机构) 。 例如，contoso.com 和 fourthcoffee.com 四条 DKIM CNAME 记录：两条用于 contoso.com，两条用于 fourthcoffee.com。

   每个自定义 **域的** DKIM CNAME 记录使用以下格式：

   - **主机名**： `selector1._domainkey.<CustomDomain>`

     **指向地址或值**： `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**：3600

   - **主机名**： `selector2._domainkey.<CustomDomain>`

     **指向地址或值**： `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**：3600

   \<DomainGUID\> 是自定义域的自定义 MX 记录中左侧的文本 (例如，对于自定义域 `.mail.protection.outlook.com` `contoso-com` contoso.com) 。 \<InitialDomain\>是注册域时所使用的域Microsoft 365 (例如，contoso.onmicrosoft.com) 。

2. 为自定义域创建 CNAME 记录后，请完成以下说明：

   a. [sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.

   b. 选择左上角的应用启动器图标，然后选择“**管理员**”。

   c. 在左下侧导航中，展开“管理”并选择“Exchange”。

   d. 转到保护  >  **DKIM**。

   e. 选择该域，**然后选择"为此** 域启用 **DKIM 签名对邮件进行签名"。** 为每个自定义域重复执行这一步。
