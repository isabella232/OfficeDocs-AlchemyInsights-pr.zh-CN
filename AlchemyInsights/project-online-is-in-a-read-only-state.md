---
title: Project Online为只读状态
ms.author: pebaum
author: pebaum
manager: pamg
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1776"
- "9000205"
ms.openlocfilehash: 988d87ca43f5394728b77561edd8e26fa0668f4ad876a5fcd09cf739092a4d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54063006"
---
# <a name="project-online-is-in-a-read-only-state"></a>Project Online为只读状态

有三个常见Project Online可能进入只读状态：

1. 组织只有Project Online 协作版许可证 () 许可证。 这不足以使网站保持活动状态，它最终将取消预配。 我们将网站放在只读状态，以便管理员知道有错误，并可以获取正确的许可证。 管理员将需要添加一个Project Online Professional和/或高级版许可证。 此时，网站将退出只读。 有关详细信息，请参阅比较Project[管理解决方案](https://products.office.com/project/compare-microsoft-project-management-software?tab=1)。
2. 已达到分配的配额。 有关详细信息，请参阅配额[Project Web App配额](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota)。 检查[配置时间按时间按](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online)时间Project Online汇总以查看报告粒度对配额使用情况的影响。
3. 只读可能是维护期间可能会发生的非常临时的情况。 我们的客户甚至不会注意到大多数维护，你通常不会看到此情况，但有时遇到短期只读情况。
