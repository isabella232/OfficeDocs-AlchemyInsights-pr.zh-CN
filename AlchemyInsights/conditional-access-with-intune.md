---
title: 使用 Intune 的条件访问
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29935918"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="a9486-102">使用 Intune 的条件访问</span><span class="sxs-lookup"><span data-stu-id="a9486-102">Conditional Access with Intune</span></span>

<span data-ttu-id="a9486-103">使用 Intune**条件访问**需要三个步骤：</span><span class="sxs-lookup"><span data-stu-id="a9486-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="a9486-p101">创建一个定义哪些资源正在受保护，并且需要访问这些资源必须满足的条件的**条件的访问策略**。例如，设备必须访问公司的电子邮件之前兼容。</span><span class="sxs-lookup"><span data-stu-id="a9486-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="a9486-p102">创建**合规性策略**，以定义前符合的设备必须满足的设置。例如，设备必须至少为 6 位数的 pin，才会被认为兼容。</span><span class="sxs-lookup"><span data-stu-id="a9486-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="a9486-p103">确保**合规性策略**和**条件的访问策略**针对所需的用户组。这可能需要在 Azure Active Directory 中创建特定的用户组。</span><span class="sxs-lookup"><span data-stu-id="a9486-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="a9486-110">阅读的详细信息：</span><span class="sxs-lookup"><span data-stu-id="a9486-110">Read more:</span></span>
  
- [<span data-ttu-id="a9486-111">条件访问最佳实践</span><span class="sxs-lookup"><span data-stu-id="a9486-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="a9486-112">条件访问入门</span><span class="sxs-lookup"><span data-stu-id="a9486-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

