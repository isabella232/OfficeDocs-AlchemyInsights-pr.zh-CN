---
title: 转移 Azure 账单所有权
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2020
ms.locfileid: "48840581"
---
# <a name="transfer-azure-billing-ownership"></a>转移 Azure 账单所有权

以帐单帐户的管理员身份登录到 [Azure 门户](https://portal.azure.com/)（该帐单帐户拥有你想要转移的订阅）。 如果不确定你是否是管理员，或需要确定谁才是管理员，请参阅“[确认帐户帐单管理员](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa)”。

- 在“ **成本管理 + 帐单** ”上搜索。
- 从左侧窗格选择“ **订阅** ”。 你可能需要选择计费范围，然后再选择“ **订阅** ”或 “ **Azure 订阅** ”（具体取决于访问权限）。
- 选择要转移的订阅的“ **转移帐单所有权** ”
- 输入帐户的电子邮件地址，该帐户的用户是订阅的新所有者的帐单管理员，然后选择 **发送转移请求**
- 用户将收到一封电子邮件，其中包含检查转移请求的说明。 若要批准转移请求，用户可选择电子邮件中的链接，并按照说明进行操作。

**注意** ：如果你将订阅的帐单所有权转移到另一个 Azure AD 租户中的用户帐户，则所有[基于角色的访问控制（RBAC）](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)以便在订阅中管理资源的权限将被永久删除。 只有新所有者才拥有在订阅中管理资源的权限。 有关详细信息，请参阅“[将订阅转移到另一个 Azure AD 租户中的用户](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)”。

**推荐文档**

- [将 Azure 订阅的帐单所有权转移到其他帐户](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [关于转移 Azure 订阅的帐单所有权](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [转移 Visual Studio、Microsoft 合作伙伴网络（MPN）和即付即用开发/测试订阅](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [转移所有权常见问题](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [有关转移所有权问题的疑难解答](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
