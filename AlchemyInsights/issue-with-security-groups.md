---
title: 安全组问题
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: d8a3c011a3a7cba6c0b1cd00ac0eb587b75bbb5b06d96ef9fd75313734e74fd0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925731"
---
# <a name="issue-with-security-groups"></a>安全组问题

**如果收到网络错误 AADDS104**

无效网络安全组规则是Azure Active Directory Domain Services（AD DS）出现网络错误的最常见原因。 虚拟网络的网络安全组必须允许访问特定的端口和协议。 如果这些端口受阻，Azure 平台就无法监控或更新托管域。 Azure AD 和 Azure AD DS 之间的同步也会受到影响。 请确保保持默认端口的开放，以避免服务中断。

若要了解并解决网络安全组配置问题的常见警报，请参阅 [添加并验证安全组](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)。
