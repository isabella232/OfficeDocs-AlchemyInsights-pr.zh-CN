---
title: 密码日志
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50523080"
---
# <a name="password-logs"></a>密码日志

**访问密码重置审核日志时遇到问题**

若要解决有关访问密码重置审核日志的问题，请执行以下步骤：

确保你有权查看审核日志。 

只有以下角色具有授权：
 - 全局管理员
 - 安全管理员
 - 安全读者

**我想查看自最初部署起的所有密码重置审核事件**

过去 30 天的报告中最多存储了 120，000 个密码重置/注册事件。 下载 CSV 时，此最大限制适用于 UI。 PowerShell 提供 100 万个事件。
有关详细信息，请参阅以下链接：

- [Azure AD 报表和事件 API 中的自助密码重置事件](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [如何使用 PowerShell 快速下载密码重置注册事件](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**我想了解有关密码重置报告功能更多信息**

在 "用户和组"下，在 Azure 门户中检查谁正在注册或重置 Azure AD 密码重置 **重置**。
有关详细信息，请参阅以下链接：

- [密码重置报告概述](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [如何在 Azure 门户中查看密码重置报告](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Azure AD 报表和事件 API 中的自助密码重置事件](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [如何使用 PowerShell 快速下载密码重置注册事件](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


