---
title: AAD Connect Health 出现问题
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50453288"
---
# <a name="problem-with-aad-connect-health"></a>AAD Connect Health 出现问题

- 确保您有权执行此操作。 默认情况下，全局管理员具有访问权限。 此外，可以使用基于 [角色的访问控制](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) 将注册权限委派给参与者。
- 确保所需的终结点已启用，并且由于防火墙未阻止。 有关详细信息，请参阅 [要求](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)。
- 由于出站通信受到网络层 SSL 检查，注册可能会失败。
- 确保已验证 Azure AD Connect Health 的通知设置。 请查看你的设置。 本指南 [可帮助](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) 你了解如何配置 Azure AD Connect 运行状况通知的通知设置。
- 若要了解有关 AAD Connect Health 同步报告以及如何下载它，请参阅对象 [级同步报告](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)。

若要对 AAD Connect Health 警报进行故障排除，请按照 [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) 数据新鲜度警报的疑难解答指南操作，有关常见问题，请参阅 [Common AAD Connect Health 安装问题](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)。
