---
title: 启用成本管理
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599053"
---
# <a name="enable-cost-management"></a>启用成本管理

**为您的组织禁用的成本是什么意思？**

使用 Enterprise 协议 (EA) 或 Microsoft Customer 协议 (MCA) 帐户的组织可以禁用对成本信息和定价信息的访问。

登录到 Azure 门户后，他们可以使用计费 Api 以编程方式获取发票 (一旦选择了) 和使用详细信息。

**如何允许其他用户访问发票**

1. 转到 Azure 门户中的 " **订阅" 边栏** 。
2. 选择 " **发票** "，然后 **访问发票**。
3. 打开访问权限，然后保存更改，以允许订阅范围的角色中的用户下载发票。

> [!NOTE]
> 帐户管理员还可以将配置为通过电子邮件发送发票。 若要了解详细信息，请参阅 [在电子邮件中获取发票](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?)。

**如何将用户添加到帐单阅读者角色**

1. 转到 Azure 门户中的 " **订阅" 边栏** 。
2. 选择 " **(IAM) 的" 访问控制** "，然后单击" **添加**"。
3. 在 "**选择角色**" 页中选择 "**帐单阅读** 者"。
4. 键入要邀请的用户的电子邮件，然后单击 **"确定"** 以发送邀请。
5. 按照邀请电子邮件中提供的说明，以付费阅读者的形式登录。 有关详细信息，请参阅 [授予对帐单的访问权限](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in)。

**推荐的文档**

- [通过 EA 门户启用 DA 和 AO 视图](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [成本管理中包括的成本](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [支持的 Microsoft Azure 提供](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [查看成本分析中的成本](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [提供对帐单信息的访问权限](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [检查 Microsoft 客户协议的访问权限](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






