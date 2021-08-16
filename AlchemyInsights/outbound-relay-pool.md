---
title: 出站中继池
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: 8750c9036f258d9c5edc94bb027d564140bbd9914712cc1f25ff3abc3f4b9468
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54041576"
---
# <a name="outbound-relay-pool"></a>出站中继池

Microsoft 正在对配置进行一些更改，以通过 Microsoft 365 中继或转发Microsoft 365。 在某些情况下，邮件使用特殊的中继池通过 Microsoft 365转发或中继。 使用中继池发送的邮件最终可能位于收件人的垃圾邮件文件夹中。 有关详细信息，请参阅出 [站传递池](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

为了避免使用中继池的情况，请确保转发/中继邮件满足以下条件之一：

- 出站发件人是租户的接受域。
- 发件人策略 (SPF) 在邮件发送到邮件时通过Microsoft 365。
- 当邮件发送到 (时) P2 发件人域中的域密钥标识的邮件和 DKIM Microsoft 365。
 
满足上述条件的邮件不会通过中继池中继。

如果域的 MX 记录指向第三方或本地服务器，请使用增强的筛选，以确保 SPF 验证对入站电子邮件正确无误，并避免通过中继池发送电子邮件。

**如何判断中继池是否受到影响？**

如果转发或中继的电子邮件使用上述条件之一，则邮件不会通过中继池中继。 但是，如果邮件通过中继池发送，则出站服务器 IP 在 40.95.0.0/16 范围内，出站服务器名称将 **rly** 包括在名称中。

