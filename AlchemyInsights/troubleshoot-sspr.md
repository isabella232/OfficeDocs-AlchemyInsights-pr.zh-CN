---
title: SSPR 疑难解答
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50428570"
---
# <a name="troubleshoot-sspr"></a>SSPR 疑难解答

**配置密码重置时遇到问题**

- 如果你是管理员，并且正在查找如何启用自助服务密码重置，请参阅教程"启用 [SSPR"，](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)为组织配置密码重置。 你可能还需要查看 [许可要求](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)。 您必须在组织中分配至少一个许可证。
    - **仅云用户** - 任何 Office 365 (O365) 付费 SKU 或 Azure AD Basic
    - **云和/或** 本地用户 - Azure AD Premium P1 或 P2、企业移动性 + 安全性 (EMS) 或安全生产企业 (SPE) 
- 有关自助服务密码重置的其他问题，请查看 [我们的常见问题解答](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)。

**我收到错误消息**

查看本文以查找常见错误及其解决方案 [：自助密码重置疑难解答](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**密码重置策略有问题**

- 如果密码重置策略未如预期方式运行，或者对密码重置策略有疑问，请查看本文 [：Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)中的密码策略和限制。
- 密码重置策略不适用于管理员。 Microsoft 对任意 Azure 管理员角色强制执行强默认双门密码重置策略。 确保您正在与不是管理员的用户一起进行测试。 有关管理员重置策略详细信息，请参阅本文： [管理员重置策略差异](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)。

**我不想我的用户注册密码重置的其他安全信息**

可以使用 API、 (或 Azure AD Connect 为) 预填充电子邮件和电话属性的数据。 若要了解如何阅读：

- [在不要求用户注册的情况下部署密码重置](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [密码重置使用的数据](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**我希望用户注册其他安全信息以重置密码**

1. 让用户通过引导他们注册其安全信息以重置自助服务[密码aka.ms/ssprsetup。](https://mysignins.microsoft.com/security-info)
1. 在用户或管理员 (填充用户密码后) ，将用户aka.ms/sspr以便用户能够重置自己的密码。 [](https://passwordreset.microsoftonline.com/)
1. 如果用户仍遇到问题，他们很可能是联合用户或密码 **哈希同步** 用户。 这意味着密码写回服务可能存在问题。