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
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="e542c-102">无法启用 AAD-DS 或部署出现故障</span><span class="sxs-lookup"><span data-stu-id="e542c-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="e542c-103">若要解决 Azure AD 域服务 (AAD-DS) 无法启用或部署故障的问题，请执行下列步骤：</span><span class="sxs-lookup"><span data-stu-id="e542c-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="e542c-104">如果你在使用现有的虚拟网络，请检查阻止在门户的 AAD-DS 中同步所需端口的规则的 NSG https://aka.ms/aadds-networking。</span><span class="sxs-lookup"><span data-stu-id="e542c-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="e542c-105">查看你的错误消息是否在 https://aka.ms/aadds-troubleshoot-enable 中的疑难解答指南中已有答案。</span><span class="sxs-lookup"><span data-stu-id="e542c-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="e542c-106">尝试在新的虚拟网络中部署 Azure AD 域服务。</span><span class="sxs-lookup"><span data-stu-id="e542c-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="e542c-107">遵循部署 AAD-DS 的入门指南：[创建并配置 AAD 域服务](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)。</span><span class="sxs-lookup"><span data-stu-id="e542c-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="e542c-108">如果你在部署 Azure AD 域服务时遇到问题，请参阅 [Azure AD 域服务疑难解答](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)来解决常见错误并帮助你正常工作。</span><span class="sxs-lookup"><span data-stu-id="e542c-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="e542c-109">**无法禁用 AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="e542c-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="e542c-110">AAD-DS 无法禁用。</span><span class="sxs-lookup"><span data-stu-id="e542c-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="e542c-111">如果你想停止使用托管域，必须将其删除。</span><span class="sxs-lookup"><span data-stu-id="e542c-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="e542c-112">要删除你的托管域，请参阅[删除 AAD 域服务](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds)。</span><span class="sxs-lookup"><span data-stu-id="e542c-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>



