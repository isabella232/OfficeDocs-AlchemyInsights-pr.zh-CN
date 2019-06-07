---
title: Office 365 中的安装 DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764879"
---
# <a name="setup-dkim-in-office-365"></a>Office 365 中的安装 DKIM

在 Office 365 中为自定义域配置 DKIM 的完整说明如下[](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)所示。

1. 对于**每个**自定义域, 您需要在您的域的 DNS 托管服务 (通常为域注册机构) 中创建**两个**DKIM CNAME 记录。 例如, contoso.com 和 fourthcoffee.com 需要四个 DKIM CNAME 记录: 两个用于 contoso.com, 两个用于 fourthcoffee.com。

   **每个**自定义域的 DKIM CNAME 记录使用以下格式:

   - **主机名**:`selector1._domainkey.<CustomDomain>`

     **指向 "地址" 或 "值**":`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **主机名**:`selector2._domainkey.<CustomDomain>`

     **指向 "地址" 或 "值**":`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\>是自定义域的自定义 MX `.mail.protection.outlook.com`记录 (例如, `contoso-com`域 contoso.com) 的左侧文本。 \<InitialDomain\>是注册 Office 365 时使用的域 (例如, contoso.onmicrosoft.com)。

2. 为自定义域创建 CNAME 记录后, 请完成以下说明:

   a. 使用您的 工作或学校帐户[登录到 Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4)。

   b. 选择左上角的应用启动器图标，然后选择“**管理员**”。

   c. In the lower-left navigation, expand **Admin** and choose **Exchange**.

   d. 转到**保护** > **DKIM**。

   e. 选择域, 然后选择 " **** 为**此域使用 DKIM 签名启用签名邮件**"。 为每个自定义域重复执行这一步。
