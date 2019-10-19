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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2019
ms.locfileid: "36504984"
---
# <a name="conditional-access-with-intune"></a>使用 Intune 进行条件访问

使用 Intune**条件访问**需要3个步骤： 
  
- 创建一个**条件访问策略**，用于定义要保护的资源，以及访问这些资源时需要满足的条件。 例如，在访问公司电子邮件之前，设备必须兼容。 
    
- 创建**符合性策略**，以定义在将设备视为合规之前必须满足的设置。 例如，设备的 pin 必须至少为6位数，然后才认为合规。 
    
- 确保**合规性策略**和**条件访问策略**都针对所需的用户组。 这可能需要在 Azure Active Directory 中创建特定的用户组。 
    
阅读更多：
  
- [条件访问最佳实践](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [条件访问入门](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

