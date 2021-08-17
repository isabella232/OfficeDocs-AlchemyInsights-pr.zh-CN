---
title: '域控制器 '
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: b044e69cef177c5a1ad38c2d27a297d90ba7f55e7b2e75fff2e390869241f325
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057884"
---
# <a name="domain-controller"></a>域控制器

**无法启用 AAD-DS 或部署出现故障**

若要解决 Azure AD 域服务 (AAD-DS) 无法启用或部署故障的问题，请执行下列步骤：

1. 如果你在使用现有的虚拟网络，请检查阻止在门户的 AAD-DS 中同步所需端口的规则的 NSG https://aka.ms/aadds-networking。
2. 查看你的错误消息是否在 https://aka.ms/aadds-troubleshoot-enable 中的疑难解答指南中已有答案。
3. 尝试在新的虚拟网络中部署 Azure AD 域服务。
4. 遵循部署 AAD-DS 的入门指南，指南可在[创建 Azure AD 域服务的教程](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)找到。
5. 如果你在部署 Azure AD 域服务时遇到问题，请参阅 [Azure AD 域服务疑难解答](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)来解决常见错误并帮助你正常工作。 

**无法禁用 AAD-DS**

AAD-DS 无法暂停。如果要停止使用托管域，则必须将其删除。

如果你遇到问题，想要解决常见错误消息或想查看相关的疑难解答步骤，请参阅 [Azure Active Directory 域服务疑难解答](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)。
