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
ms.openlocfilehash: 454ce626862bb4a2361abccd92ad0099b534388c
ms.sourcegitcommit: 059ad2936788266ea9714ec8c66d407d7261aeb6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/29/2020
ms.locfileid: "49736868"
---
# <a name="transfer-azure-billing-ownership"></a>转移 Azure 账单所有权

以拥有你想要转移的订阅的帐单帐户管理员身份登录到 [Azure 门户](https://portal.azure.com/)。 如果不确定你是否为管理员，或如果需要确定谁是管理员，请参阅[确认帐户帐单管理员](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa)。

1. 在 _成本管理 + 帐单_ 上搜索。
1. 从左侧窗格选择“**订阅**”。 根据访问权限，可能需要选择计费范围，然后再选择 **订阅** 或 **Azure 订阅**。
1. 选择要转移的订阅的 **转移帐单所有权**。
1. 输入帐户的电子邮件地址，该帐户的用户将为订阅的新所有者的帐单管理员，然后选择 **发送转移请求**。
1. 用户将收到一封电子邮件，其中包含检查转移请求的说明。 若要批准转移请求，用户可选择电子邮件中的链接，并按照说明进行操作。

请注意，如果你将订阅的帐单所有权转移到另一个 Azure AD 租户中的用户帐户，则将永久删除用于管理订阅中资源的所有[基于角色的访问控制（RBAC）](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)分配。 仅新的所有者才拥有在订阅中管理资源的权限。 有关如何为订阅更改目录的更多信息，请参见[将订阅转移到另一个 Azure AD 租户中的用户](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)。

_**对发票的重要影响：**_ 如果已转让 Azure 订阅的帐单所有权，则费用将按比例分配。 你将能够按照以下方式访问发票：  

1. 从  Azure 门户中的 [订阅页面中](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)选择你的订阅，作为 [可以访问发票的用户](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)，然后选择 **发票**。
1. 点击 **下载发票** 以查看 PDF 发票副本。 如果显示 _不可用_，请参阅 [为何无法查看上次帐单周期的发票？](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)。
1. 你还可通过点击 **帐单周期** 来查看每日使用量，以获取发票的 PDF 格式和详细的每日使用量文件的副本 (.CSV)。 有关更多信息，请参阅 [获取发票和使用情况数据](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)。

**推荐文档**

- [将 Azure 订阅的帐单所有权转移到其他帐户](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [关于转移 Azure 订阅的帐单所有权](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [转移 Visual Studio、Microsoft 合作伙伴网络（MPN）和即付即用开发/测试订阅](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [转移所有权常见问题](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [有关转移所有权问题的疑难解答](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
