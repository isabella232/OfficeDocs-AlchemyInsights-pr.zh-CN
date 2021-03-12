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
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="5fd5c-102">在组织中搜索并删除电子邮件</span><span class="sxs-lookup"><span data-stu-id="5fd5c-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="5fd5c-103">请按以下步骤操作：</span><span class="sxs-lookup"><span data-stu-id="5fd5c-103">Follow these steps:</span></span>

1. <span data-ttu-id="5fd5c-104">如果你不是全局管理员，则必须将你的帐户添加到电子 **数据** 展示管理员角色组或合规性搜索管理角色中，才能 **搜索邮件**。</span><span class="sxs-lookup"><span data-stu-id="5fd5c-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="5fd5c-105">若要删除邮件，你需要加入组织管理角色 **组** 或搜索和清除管理 **角色**。</span><span class="sxs-lookup"><span data-stu-id="5fd5c-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="5fd5c-106">这些角色的权限在安全与合规中心 [&分配。](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="5fd5c-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="5fd5c-107">[创建内容搜索](https://docs.microsoft.com/office365/securitycompliance/content-search) 以查找要删除的邮件。</span><span class="sxs-lookup"><span data-stu-id="5fd5c-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="5fd5c-108">[连接到安全与合规中心 PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)。</span><span class="sxs-lookup"><span data-stu-id="5fd5c-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="5fd5c-109">如果你使用的是 MFA，请参阅以下说明：使用多重身份验证&安全中心 [PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="5fd5c-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="5fd5c-110">删除邮件：运行 `New-ComplianceSearchAction` cmdlet 删除邮件。</span><span class="sxs-lookup"><span data-stu-id="5fd5c-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="5fd5c-111">已删除的邮件将移动到用户的"可恢复的项目"文件夹。</span><span class="sxs-lookup"><span data-stu-id="5fd5c-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="5fd5c-112">有关示例命令，请参阅步骤 [3：删除邮件。](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="5fd5c-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
