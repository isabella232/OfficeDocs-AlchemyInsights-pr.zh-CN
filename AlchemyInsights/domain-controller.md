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
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886782"
---
# <a name="domain-controller"></a><span data-ttu-id="9606f-102">域控制器</span><span class="sxs-lookup"><span data-stu-id="9606f-102">Domain controller</span></span>

<span data-ttu-id="9606f-103">**无法启用 AAD-DS 或部署出现故障**</span><span class="sxs-lookup"><span data-stu-id="9606f-103">**Unable to enable AAD-DS or deployment is failing**</span></span>

<span data-ttu-id="9606f-104">若要解决 Azure AD 域服务 (AAD-DS) 无法启用或部署故障的问题，请执行下列步骤：</span><span class="sxs-lookup"><span data-stu-id="9606f-104">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="9606f-105">如果你在使用现有的虚拟网络，请检查阻止在门户的 AAD-DS 中同步所需端口的规则的 NSG https://aka.ms/aadds-networking。</span><span class="sxs-lookup"><span data-stu-id="9606f-105">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="9606f-106">查看你的错误消息是否在 https://aka.ms/aadds-troubleshoot-enable 中的疑难解答指南中已有答案。</span><span class="sxs-lookup"><span data-stu-id="9606f-106">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="9606f-107">尝试在新的虚拟网络中部署 Azure AD 域服务。</span><span class="sxs-lookup"><span data-stu-id="9606f-107">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="9606f-108">遵循部署 AAD-DS 的入门指南，指南可在[创建 Azure AD 域服务的教程](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)找到。</span><span class="sxs-lookup"><span data-stu-id="9606f-108">Follow the Getting Started guide on how to deploy AAD-DS, which is available at [Tutorial to Create Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="9606f-109">如果你在部署 Azure AD 域服务时遇到问题，请参阅 [Azure AD 域服务疑难解答](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)来解决常见错误并帮助你正常工作。</span><span class="sxs-lookup"><span data-stu-id="9606f-109">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="9606f-110">**无法禁用 AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="9606f-110">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="9606f-111">AAD-DS 无法禁用。</span><span class="sxs-lookup"><span data-stu-id="9606f-111">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="9606f-112">如果你想停止使用托管域，必须将其删除。</span><span class="sxs-lookup"><span data-stu-id="9606f-112">If you wish to stop using your managed domain, it must be deleted.</span></span>

<span data-ttu-id="9606f-113">如果你遇到问题，想要解决常见错误消息或想查看相关的疑难解答步骤，请参阅 [Azure Active Directory 域服务疑难解答](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)。</span><span class="sxs-lookup"><span data-stu-id="9606f-113">If you run into issues, to resolve common error messages and for associated troubleshooting steps to help you get things running again, see [Troubleshoot Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span></span>
