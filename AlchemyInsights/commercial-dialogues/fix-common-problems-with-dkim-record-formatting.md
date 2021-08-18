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
ms.openlocfilehash: e55175e7613d220eaf956d3c7fd02213dcd5803d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323980"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>修复 DKIM 记录格式的常见问题

大多数 DKIM 设置问题与错误的 DNS 记录相关。

若要修复 DKIM 设置问题，请验证 DKIM CNAME 记录 (不是TXT 记录) 格式。 有关详细信息，请参阅在 Office 365 中手动设置[DKIM 需要Office 365。](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)

如果需要有关 DNS 记录的一般帮助，请参阅在任何[DNS](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)托管提供商上为 dns Office 365。

**注意**：在域的 DNS 托管服务创建或更新 DKIM DNS 记录后，需要等待 DNS 记录传播。
