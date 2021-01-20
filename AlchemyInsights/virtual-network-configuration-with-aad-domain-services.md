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
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="7a150-102">通过 AAD 域服务的虚拟配置</span><span class="sxs-lookup"><span data-stu-id="7a150-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="7a150-103">通过 AAD 域服务的虚拟配置包含下列步骤：</span><span class="sxs-lookup"><span data-stu-id="7a150-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="7a150-104">在 Azure 门户上查看域的运行状况 https://aka.ms/aadds-health</span><span class="sxs-lookup"><span data-stu-id="7a150-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="7a150-105">在门户上查看阻止在 Azure Active Directory 中同步所需端口的规则的 NSG https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="7a150-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="7a150-106">确保在与你的 Azure Active Directory 域服务管理域相同的 Azure 区域中部署你的虚拟网络。</span><span class="sxs-lookup"><span data-stu-id="7a150-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="7a150-107">确保当前你没有某个与在虚拟网络上可用的域名重名的域。</span><span class="sxs-lookup"><span data-stu-id="7a150-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="7a150-108">有关 Azure 虚拟网络设计注意事项和支持 AAD 域服务的更多信息，请参阅[虚拟网络注意事项](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations)。</span><span class="sxs-lookup"><span data-stu-id="7a150-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

