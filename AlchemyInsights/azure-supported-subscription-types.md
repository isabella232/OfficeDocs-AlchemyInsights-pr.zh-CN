---
title: 支持的订阅类型
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6675"
ms.openlocfilehash: f11eabdc18f708e34a6a10c67bc3e7416330cbf34aec20209b42252ffa0ab018
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072150"
---
# <a name="supported-subscription-types"></a>支持的订阅类型

请查看支持的订阅类型以继续操作。

[支持的订阅类型](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**转移帐单所有权**

将 Azure 门户用作需要转移订阅的帐单帐户的“[帐户管理员](https://ms.portal.azure.com/)”

- 在“**成本管理 + 帐单**”上搜索。 从左侧窗格选择 **“订阅”**。 你可能需要选择计费范围，然后再选择“**订阅**”或 “**Azure 订阅**”（具体取决于访问权限）。
- 选择要转移的订阅的“转移帐单所有权”
- 输入帐户的电子邮件地址，该帐户的用户是订阅的新所有者的帐单管理员，然后选择 **发送转移请求**
- 用户将收到一封电子邮件，其中包含检查转移请求的说明。 若要批准转移请求，用户可选择电子邮件中的链接，并按照说明进行操作。

注意：如果你将订阅的帐单所有权转移到另一个 Azure AD 租户中的用户帐户，则所有[基于角色的访问控制（RBAC）](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)以便在订阅中管理资源的权限将被永久删除。 只有新所有者才拥有在订阅中管理资源的权限。 有关详细信息，请参阅“[将订阅转移到另一个 Azure AD 租户中的用户](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)”。

**转移订阅的所有权**

“订阅所有权转移”的先决条件是：用于管理订阅中的资源的基于角色的访问权限（RBAC）将失去访问权限。 有关将现有订阅添加到租户的详细信息，请参阅“[将 Azure 订阅关联或添加到 Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support)”。

- 当前计费周期中包含现有未清金额的“订阅转移”将不会被转移到新帐户中的支付工具。 新帐户中的用户可用的唯一信息是上个月的订阅费用。 其他使用情况和帐单历史记录不会随订阅转移。
- 仅在企业协议门户支持企业协议（EA）订阅的帐单所有权转移
- 将面向信贷的订阅（如 Visual Studio、BizSpark、Microsoft 合作伙伴网络等）转移给新用户需要具有 Visual Studio/Microsoft 合作伙伴网络许可证以接受转移请求
- 所有资源（如虚拟机、磁盘和网站）均已成功转移到新帐户。 跨租户订阅转移中的以下资源可能会受到影响：

**Azure AD 域服务**

密钥保管库

- [SQL 相关用户和数据库](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support)可能会受到影响，尤其是当客户使用与 Azure Active Directory 相关的身份验证时
- 使用 Azure Active Directory 身份验证配置的 **应用服务** 可能会受到影响
- 取消 Azure 订阅后，已连接至 Azure 订阅的 **Visual Studio Team** 服务帐户可能会暂时失去访问权限

**推荐文档**

接受帐单所有权后的步骤：

- 若要保留帐单所有权，但想要更改订阅类型，请参阅：“[将 Azure 订阅切换到其他优惠](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)”
- [转移 Visual Studio、Microsoft 合作伙伴网络（MPN）和即付即用开发/测试订阅](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [转移企业协议（EA）订阅的帐单所有权](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [转移所有权常见问题](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [有关转移所有权问题的疑难解答](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)