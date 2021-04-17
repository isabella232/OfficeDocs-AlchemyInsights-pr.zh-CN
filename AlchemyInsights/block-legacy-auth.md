---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820168"
---
# <a name="blocking-legacy-authentication"></a>阻止旧式身份验证

旧式身份验证是指由以下客户端发出的身份验证请求的术语：

- 不使用新式身份验证的较旧 Office 客户端 (例如，Office 2010 客户端) 。

- 任何使用旧版邮件协议（比如 IMAP/SMTP/POP3）的客户端。

有关阻止旧版身份验证和启用新式验证的信息，请参阅阻止 [旧式身份验证](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)。

Azure Active Directory (Azure AD) 中的安全默认值，可以更轻松地保护组织的安全并帮助保护组织。 安全默认值包含针对常见攻击的预配置安全设置。
有关安全默认值详细信息，请参阅什么是[安全默认值？。](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) 

**注意**：如果租户是在 2019 年 10 月 22 日当天或之后创建的，则可能会遇到新的默认安全行为，并且已在租户中启用安全默认值。  为了保护所有用户，正在向创建的所有新租户推出安全默认值。
