---
title: 配置域服务
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884559"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>无法启用 AAD-DS 或部署出现故障

若要解决 Azure AD 域服务 (AAD-DS) 无法启用或部署故障的问题，请执行下列步骤：

1. 如果你在使用现有的虚拟网络，请检查阻止在门户的 AAD-DS 中同步所需端口的规则的 NSG https://aka.ms/aadds-networking。
2. 查看你的错误消息是否在 https://aka.ms/aadds-troubleshoot-enable 中的疑难解答指南中已有答案。
3. 尝试在新的虚拟网络中部署 Azure AD 域服务。
4. 遵循部署 AAD-DS 的入门指南：[创建并配置 AAD 域服务](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)。
5. 如果你在部署 Azure AD 域服务时遇到问题，请参阅 [Azure AD 域服务疑难解答](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)来解决常见错误并帮助你正常工作。 

**无法禁用 AAD-DS**

AAD-DS 无法禁用。 如果你想停止使用托管域，必须将其删除。
要删除你的托管域，请参阅[删除 AAD 域服务](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds)。



