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
ms.openlocfilehash: c3623aee9ab3592254ffb25aade7d52a2c7ddd49fde939956162cd4008d5ba19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003559"
---
# <a name="enable-cost-management"></a>启用成本管理

**"为组织禁用成本"意味着什么？**

使用 企业协议 (EA) 或 Microsoft 客户协议 (MCA) 帐户的组织可以禁止访问成本信息和定价信息。

登录到 Azure 门户后，他们可以使用计费 API 以编程方式在选择加入 (获取发票) 和使用详细信息。

**如何允许其他用户访问发票**

1. 转到 Azure **门户中的订阅** 边栏选项卡。
2. 选择 **"发票"，****然后选择"访问发票"。**
3. 打开访问权限，然后保存更改，以允许订阅范围内的角色中的用户下载发票。

> [!NOTE]
> 帐户管理员还可以配置为通过电子邮件发送发票。 若要了解更多信息，请参阅 [通过电子邮件获取发票](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?)。

**如何将用户添加到计费读取者角色**

1. 转到 Azure **门户中的订阅** 边栏选项卡。
2. 选择 **"IAM (访问控制)** 然后单击"添加 **"。**
3. 在 **"选择角色** "页 **中选择"计费读者** "。
4. 键入要邀请的用户的电子邮件，然后单击 **"确定"** 以发送邀请。
5. 按照邀请电子邮件中提供的说明以计费读者登录。 有关详细信息，请参阅授予对 [计费的访问权限](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in)。

**推荐文档**

- [通过 EA 门户启用 DA 和 AO 视图](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [成本管理中包含的成本](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [受支持的Microsoft Azure产品/服务](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [查看成本分析中的成本](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [提供对计费信息的访问权限](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [检查 Microsoft 客户协议的访问权限](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






