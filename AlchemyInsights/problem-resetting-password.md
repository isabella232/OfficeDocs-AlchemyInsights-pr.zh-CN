---
title: 重置密码时出现问题
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50585648"
---
# <a name="problems-resetting-password"></a>重置密码时出现问题

以下是在重置密码和可能的解决方案时可能面临的一些问题：

**我遇到密码重置未涵盖在其他类别中的问题**

- 确保你有权重置密码。 只有全局、密码和用户管理员可以重置用户密码。 全局管理员还可以重置其他特权管理员的密码。
- 确保您了解许可要求：
    - 必须在组织中分配至少一个许可证
        - 仅云用户 - 任何 Office 365 (O365) 付费 SKU 或 Azure AD Basic
        - 云和/或本地用户 - Azure AD Premium P1 或 P2、企业移动性 + 安全性 (EMS) 或安全生产企业 (SPE) 
        - 若要阅读有关许可要求的信息，请参阅文章 [Azure AD 自助服务密码重置的许可要求](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)。

**测试我设置的密码重置策略时遇到问题**

- 最近应用的策略可能需要几分钟才能跨所有数据中心和终点进行复制。 与数据中心的物理距离也会影响更改应用速度。
- 使用最终用户（而不是管理员）进行测试，然后通过一小组用户进行试点。 Azure 门户中配置的策略仅适用于最终用户，不适用于管理员。 Microsoft 对 Azure 管理员角色强制执行强默认双门密码重置策略 (例如：全局管理员、支持管理员、密码管理员等) 
    - 了解有关管理员 [策略的更多信息](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)。

**我想要部署密码重置，但不希望我的用户注册其他安全信息**

为用户预填充数据，以便他们不必这样做！ - 作为管理员，可以在向组织推出密码重置之前为用户设置电话和电子邮件属性。 可以使用 API、PowerShell 或 Azure AD Connect 进行此操作。 有关详细信息，请参阅：
- [无需用户注册即可部署密码重置](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [密码重置使用的数据](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**密码重置按钮灰出**

你无权重置此用户的密码。 只有全局、密码和用户管理员可以重置用户密码。 全局管理员还可以重置其他特权管理员的密码。

**我看不到密码重置边栏选项卡**

你无权重置密码。 只有全局、密码和用户管理员可以重置用户密码。 全局管理员还可以重置其他特权管理员的密码。

**在密码重置中看不到本地集成边栏选项卡**

- 本地集成边栏选项卡仅在混合环境中显示 - 这意味着你正在使用密码写回操作本地用户的密码。
- 如果：
    - 您没有使用密码写回
    - 密码写回的安装/连接存在问题
    - Azure AD Connect 的安装/连接存在问题
    - 有关密码写回问题的更多疑难解答步骤，请参阅"密码写回疑 [难解答"部分](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**不知道如何重置用户密码**

1. 以适当的管理员登录 Azure 门户。
1. 转到"用户和组"边栏选项卡，选择 **"所有用户"。**
1. 从列表中选择用户。
1. 对于所选用户，选择 **"概述**"，然后在命令栏中单击"**重置密码"。**
1. 按照屏幕上的说明进行操作。
    - 仅通过 Azure 门户执行的重置支持密码写回。

**我在 Office 365 管理门户或 Office 365 移动应用程序中重置本地用户密码，但用户仍无法登录**

此门户不支持密码写回。 在 Azure 门户中再次重置用户密码 - portal.azure.com

