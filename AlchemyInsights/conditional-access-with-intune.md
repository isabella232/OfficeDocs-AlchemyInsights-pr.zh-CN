---
title: 使用 Intune 的条件访问
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 59f1aefaeec3d655b2388b00e7d58a8c2338504b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29459790"
---
# <a name="conditional-access-with-intune"></a>使用 Intune 的条件访问

使用 Intune**条件访问**需要三个步骤： 
  
- 创建一个定义哪些资源正在受保护，并且需要访问这些资源必须满足的条件的**条件的访问策略**。例如，设备必须访问公司的电子邮件之前兼容。 
    
- 创建**合规性策略**，以定义前符合的设备必须满足的设置。例如，设备必须至少为 6 位数的 pin，才会被认为兼容。 
    
- 确保**合规性策略**和**条件的访问策略**针对所需的用户组。这可能需要在 Azure Active Directory 中创建特定的用户组。 
    
阅读详细信息
  
- [条件访问最佳实践](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/best-practices)
    
- [条件访问入门](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

