---
title: 1491-search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: ''
ms.openlocfilehash: 881a579d7098578452c994b7ac66fe22a1d90dc2
ms.sourcegitcommit: 5182c9a73641079be59740e4524434b2e8be613a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29964809"
---
# <a name="content-search-not-returning-expected-results"></a>不返回预期的结果的内容搜索

当从 Office 365 安全性 & 合规性中心运行内容搜索，您可能会收到意外的搜索结果。考虑以下因素会影响搜索结果：

- **内容位置和搜索条件**： 确保已选择正确的内容位置和搜索条件。如果您运行大型搜索 （具有多个位置），请考虑将其拆分为多个搜索。

- **部分，索引项目**： 从邮箱[部分，索引项目](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search)包含中估计的搜索结果。但是，从 SharePoint 和 OneDrive 中的网站的部分索引的项目不包括在搜索估计。

- **搜索失败**： 搜索数量较大的邮箱 （超过十万名邮箱），如果可能会显示搜索错误，如 CS008 009 和 CS012 002 的错误代码)。在这种情况下，重试失败的内容位置的搜索。请参阅[本文](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search)的详细信息。
