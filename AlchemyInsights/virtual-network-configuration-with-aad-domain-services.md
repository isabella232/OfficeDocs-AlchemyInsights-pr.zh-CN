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
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884556"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>通过 AAD 域服务的虚拟配置

通过 AAD 域服务的虚拟配置包含下列步骤： 

1. 在 Azure 门户上查看域的运行状况 https://aka.ms/aadds-health
2. 在门户上查看阻止在 Azure Active Directory 中同步所需端口的规则的 NSG https://aka.ms/aadds-networking
3. 确保在与你的 Azure Active Directory 域服务管理域相同的 Azure 区域中部署你的虚拟网络。
4. 确保当前你没有某个与在虚拟网络上可用的域名重名的域。

有关 Azure 虚拟网络设计注意事项和支持 AAD 域服务的更多信息，请参阅[虚拟网络注意事项](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations)。

