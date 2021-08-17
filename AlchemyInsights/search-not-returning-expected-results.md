---
title: 1491-search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052700"
---
# <a name="content-search-not-returning-expected-results"></a>内容搜索未返回预期结果

从安全与合规Microsoft 365运行&搜索时，您可能会收到意外的搜索结果。 请考虑以下可能影响搜索结果的因素：

- **内容位置和搜索条件**：确保选择了正确的内容位置和搜索条件。 如果运行了具有多个 (的大型搜索) ，请考虑拆分为多个搜索。

- **部分索引项目**[：邮箱](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search)中的部分索引项目包含在估计的搜索结果中。 但是，来自网站和网站SharePoint索引OneDrive不包括在搜索估计中。

- 搜索失败：在搜索 (邮箱数超过 100，000) 时，可能会收到搜索错误，错误代码包括 CS008-009 和 CS012-002) 。 在这种情况下，请仅重试对失败的内容位置的搜索。 有关详细信息  [，](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) 请参阅本文。
