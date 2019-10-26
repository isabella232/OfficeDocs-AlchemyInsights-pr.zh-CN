---
title: 使用 Intune 进行条件访问
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/25/2019
ms.locfileid: "36504984"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="462b0-102">使用 Intune 进行条件访问</span><span class="sxs-lookup"><span data-stu-id="462b0-102">Conditional Access with Intune</span></span>

<span data-ttu-id="462b0-103">使用 Intune**条件访问**需要3个步骤：</span><span class="sxs-lookup"><span data-stu-id="462b0-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="462b0-104">创建一个**条件访问策略**，用于定义要保护的资源，以及访问这些资源时需要满足的条件。</span><span class="sxs-lookup"><span data-stu-id="462b0-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="462b0-105">例如，在访问公司电子邮件之前，设备必须兼容。</span><span class="sxs-lookup"><span data-stu-id="462b0-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="462b0-106">创建**符合性策略**，以定义在将设备视为合规之前必须满足的设置。</span><span class="sxs-lookup"><span data-stu-id="462b0-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="462b0-107">例如，设备的 pin 必须至少为6位数，然后才认为合规。</span><span class="sxs-lookup"><span data-stu-id="462b0-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="462b0-108">确保**合规性策略**和**条件访问策略**都针对所需的用户组。</span><span class="sxs-lookup"><span data-stu-id="462b0-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="462b0-109">这可能需要在 Azure Active Directory 中创建特定的用户组。</span><span class="sxs-lookup"><span data-stu-id="462b0-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="462b0-110">阅读更多：</span><span class="sxs-lookup"><span data-stu-id="462b0-110">Read more:</span></span>
  
- [<span data-ttu-id="462b0-111">条件访问最佳实践</span><span class="sxs-lookup"><span data-stu-id="462b0-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="462b0-112">条件访问入门</span><span class="sxs-lookup"><span data-stu-id="462b0-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

