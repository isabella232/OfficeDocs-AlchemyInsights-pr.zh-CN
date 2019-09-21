---
title: 经典 SharePoint 审核日志报告
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068013"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>SharePoint 和 OneDrive 审核日志

**SharePoint 和 OneDrive 新式统一审核日志与合规性**

- [打开/关闭统一审核日志记录](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

SharePoint 或 OneDrive 中不需要其他配置。

- 使用审核日志搜索检查文件、文件夹、用户、权限的活动的活动：

    - [文件和页面活动](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [文件夹活动](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [共享和访问请求活动](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [同步活动](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [网站管理活动](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- 有关如何检索这些事件的详细信息，请参阅[Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)。

**SharePoint 经典审核日志**

我们已将 SPO 旧审核迁移到统一审核日志（UAL）。 这实际上意味着所有 SPO 的旧审核报告现在都将通过 UAL 供电，旧的审核信号已迁移到 UAL。

关键更改：

- 无法使用修整功能。
- 您在其中选择要审核的特定事件的部分不可用。 有关默认情况下可用的已审核事件的完整列表，请参阅[本文档](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)。
- "**自定义报告**" 下的 "位置" 选项不可用。 
- "打开或下载文档" 事件不可用。 

