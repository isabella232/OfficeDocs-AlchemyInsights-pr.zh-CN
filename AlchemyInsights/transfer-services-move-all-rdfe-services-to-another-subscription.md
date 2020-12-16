---
title: 传输服务 - 将所有 RDFE 服务移动到其他订阅
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2020
ms.locfileid: "49681452"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>传输服务 - 将所有 RDFE 服务移动到其他订阅

**移动资源**

可以使用 Azure 门户、Azure PowerShell、Azure CLI 或 REST API 将 Azure 资源移动到同一订阅下的另一个 Azure 订阅或资源组，以移动资源。

在移动资源之前，请参阅：

- [移动资源前检查表](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [可以移动的服务](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [如何验证移动](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [服务移动指南](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

若要将现有资源移动到其他资源组或订阅，可以使用：

- [Azure 门户](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

教程： [将 Azure 资源移动到其他资源组或订阅](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Azure 资源管理器错误疑难解答**

请参阅以下文章，了解一些常见的 Azure 部署错误，并接收解决这些问题的信息。 如果找不到部署错误的错误代码，请参阅["查找错误代码"。](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)

- [解决部署错误](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [将 Azure 资源移动到新资源组或订阅疑难解答](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

请注意，如果你想要升级 Azure 订阅，例如从免费切换到即付即用，你将需要转换你的订阅。

- 若要升级免费试用版，请参阅将免费试用版或 Microsoft Imagine Azure 订阅升级到即付 [即用](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)。
- 若要更改即付即用帐户，请参阅将 Azure 即付即用订阅更改为 [其他优惠](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)。

**若要向 Azure Active Directory 租户添加或关联 Azure 订阅：**

1. 从 Azure 门户的"订阅"页面登录并选择 [想要使用的订阅](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)。
2. 选择 **"更改目录"。**
3. 查看出现的任何警告，然后选择"更改 **"。**
4. 订阅的目录已更改，你将收到一条成功消息。
5. 使用 *目录切换* 程序转到新目录。 可能需要 10 分钟才能正确显示所有内容。

**建议的文档**

- [转移 Azure 订阅的所有权](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [将资源移动到新资源组或订阅](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [使用 Azure 门户管理资源](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
