---
title: 停用 Azure 权限管理服务（RMS）
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5070"
- "9002278"
ms.openlocfilehash: 6bacfd0e383c1a7c02b50e60f9626a733ee68cbc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745777"
---
# <a name="decommission-azure-rights-management-service-rms"></a><span data-ttu-id="d4e4d-102">停用 Azure 权限管理服务（RMS）</span><span class="sxs-lookup"><span data-stu-id="d4e4d-102">Decommission Azure Rights Management Service (RMS)</span></span>

<span data-ttu-id="d4e4d-103">停用 Azure 权限管理服务前，请确保你拥有 Azure 信息保护租户密钥副本和合适的受信任发布域（TPD）。</span><span class="sxs-lookup"><span data-stu-id="d4e4d-103">Make sure that you have a copy of your Azure Information Protection tenant key and a suitable trusted publishing domain (TPD) before you deactivate the Azure Rights Management service.</span></span>

<span data-ttu-id="d4e4d-104">有关取消和停用 Azure 信息保护的其他资源，请参阅：</span><span class="sxs-lookup"><span data-stu-id="d4e4d-104">For additional resources about decommissioning and deactivating protection for Azure Information Protection, see:</span></span>

- [<span data-ttu-id="d4e4d-105">教程：配置 Azure 信息保护策略设置和创建新标签</span><span class="sxs-lookup"><span data-stu-id="d4e4d-105">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [<span data-ttu-id="d4e4d-106">什么是 Azure 信息保护？</span><span class="sxs-lookup"><span data-stu-id="d4e4d-106">What is Azure Information Protection?</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="d4e4d-107">有关使用 Azure 信息保护常见方案的操作指南</span><span class="sxs-lookup"><span data-stu-id="d4e4d-107">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
    
- [<span data-ttu-id="d4e4d-108">如何将 Azure 信息保护标签迁移到统一的敏感度标签</span><span class="sxs-lookup"><span data-stu-id="d4e4d-108">How to migrate Azure Information Protection labels to unified sensitivity labels</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)  
    
- [<span data-ttu-id="d4e4d-109">Azure 信息保护定价</span><span class="sxs-lookup"><span data-stu-id="d4e4d-109">Azure Information Protection pricing</span></span>](https://azure.microsoft.com/pricing/details/information-protection)  
    
- [<span data-ttu-id="d4e4d-110">Azure 信息保护要求</span><span class="sxs-lookup"><span data-stu-id="d4e4d-110">Azure Information Protection requirements</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
    
- [<span data-ttu-id="d4e4d-111">如何从 Azure 门户激活权限管理保护服务</span><span class="sxs-lookup"><span data-stu-id="d4e4d-111">How to activate the Rights Management protection service from the Azure portal</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-use/activate-azure)