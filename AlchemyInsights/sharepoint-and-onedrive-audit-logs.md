---
title: 经典 SharePoint 审核日志报告
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662198"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>SharePoint 和 OneDrive 审核日志

## <a name="sharepoint-classic-audit-logs"></a>SharePoint 经典审核日志

SPO 旧审核已迁移到统一审核日志 (UAL) 。 所有 SPO 的旧审核报告现在都将通过 UAL 供电，旧的审核信号已迁移到 UAL。

关键更改：

* 修整功能不可用。
* 选择要审核的特定事件不可用。 有关默认情况下可用的已审核事件的完整列表，请参阅 [本文档](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) 。
* "**自定义报告**" 下的 "**位置**" 选项不可用。
* " **打开或下载文档** 事件" 选项不可用。

[配置网站集的审核设置](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint 和 OneDrive 新式统一审核日志与合规性

* [打开/关闭统一审核日志记录](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

SharePoint 或 OneDrive 中不需要其他配置。

使用审核日志搜索检查文件的活动 (s) 、folder (s) 、用户 () 、权限：

* [文件和页面活动](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [文件夹活动](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [共享和访问请求活动](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [同步活动](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [网站管理活动](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

有关如何检索这些事件的详细信息，请参阅 [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)。
