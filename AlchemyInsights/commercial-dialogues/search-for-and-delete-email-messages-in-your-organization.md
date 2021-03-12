---
title: 在组织中搜索并删除电子邮件
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736067"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>在组织中搜索并删除电子邮件

请按以下步骤操作：

1. 如果你不是全局管理员，则必须将你的帐户添加到电子 **数据** 展示管理员角色组或合规性搜索管理角色中，才能 **搜索邮件**。 若要删除邮件，你需要加入组织管理角色 **组** 或搜索和清除管理 **角色**。 这些角色的权限在安全与合规中心 [&分配。](https://protection.office.com)
2. [创建内容搜索](https://docs.microsoft.com/office365/securitycompliance/content-search) 以查找要删除的邮件。
3. [连接到安全与合规中心 PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)。 如果你使用的是 MFA，请参阅以下说明：使用多重身份验证&安全中心 [PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. 删除邮件：运行 `New-ComplianceSearchAction` cmdlet 删除邮件。 已删除的邮件将移动到用户的"可恢复的项目"文件夹。 有关示例命令，请参阅步骤 [3：删除邮件。](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
