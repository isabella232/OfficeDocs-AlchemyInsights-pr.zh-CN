---
title: 1491-搜索-不返回-预期结果
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709217"
---
# <a name="content-search-not-returning-expected-results"></a>内容搜索未返回预期结果

在从 Microsoft 365 安全 & 合规中心运行内容搜索时，您可能会收到意外的搜索结果。 请考虑可能影响您的搜索结果的以下内容：

- **内容位置和搜索条件**：请确保已选择正确的内容位置和搜索条件。 如果您运行的是大型搜索（包含多个位置），请考虑将其拆分为多个搜索。

- **部分索引项目**：估计的搜索结果中包含来自邮箱的[部分索引项目](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search)。 但是，搜索估计中不包含来自 SharePoint 和 OneDrive 中的网站的部分索引项。

- **搜索失败**：搜索大量邮箱（超过100000个邮箱）时，您可能会收到搜索错误，其中包含错误代码，如 CS008-009 和 CS012-002）。 在这种情况下，请仅对发生故障的内容位置重试搜索。 有关详细信息，请参阅[本文](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search)。
