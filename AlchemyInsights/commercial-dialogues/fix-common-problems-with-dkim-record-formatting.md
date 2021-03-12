---
title: 修复 DKIM 记录格式的常见问题
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736180"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>修复 DKIM 记录格式的常见问题

大多数 DKIM 设置问题与错误的 DNS 记录相关。

若要修复 DKIM 设置问题，请验证 DKIM CNAME 记录 (TXT 记录) 格式是否正确。  有关详细信息，请参阅在 [Office 365 中手动设置 DKIM 需要执行哪些操作](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)。

如果需要有关 DNS 记录的一般帮助，请参阅在任何 DNS 托管提供商处为 [Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)创建 DNS 记录。

> [!NOTE]
> 在域的 DNS 托管服务创建或更新 DKIM DNS 记录后，需要等待 DNS 记录传播。
