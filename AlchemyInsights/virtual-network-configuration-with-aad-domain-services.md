---
title: 通过 AAD 域服务的虚拟配置
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
- "7927"
- "9004397"
ms.openlocfilehash: 03a6ec63ba8e2779b0fe3f0381606af2c0748f8b848baaa7cd88b61317bd7a5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072834"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>通过 AAD 域服务的虚拟配置

通过 AAD 域服务的虚拟配置包含下列步骤： 

1. 在 Azure 门户上查看域的运行状况 https://aka.ms/aadds-health
2. 在门户上查看阻止在 Azure Active Directory 中同步所需端口的规则的 NSG https://aka.ms/aadds-networking
3. 确保在与你的 Azure Active Directory 域服务管理域相同的 Azure 区域中部署你的虚拟网络。
4. 确保当前你没有某个与在虚拟网络上可用的域名重名的域。

有关 Azure 虚拟网络设计注意事项和支持 AAD 域服务的更多信息，请参阅[虚拟网络注意事项](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations)。

