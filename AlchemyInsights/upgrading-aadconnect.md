---
title: 932升级 AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 0bbb847bb1381330065ebba6e109795908b06490
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2019
ms.locfileid: "30778732"
---
# <a name="upgrade-azure-ad-connect"></a>升级 Azure AD Connect

默认情况下, 启用了 Azure AD Connect 的自动升级, 这有助于确保你运行的是最新版本。 若要验证自动升级设置, 请在 Azure AD PowerShell 中使用**ADSyncAutoUpgrade** cmdlet。 cmdlet 将返回以下值之一: 
  
- **enabled**: 已启用自动升级。 
    
- **disabled**: 自动升级已禁用。 
    
- 已**挂起**: 系统不再符合接收自动升级的条件。 您不能配置此值;它是由系统设置的。 
    
有关详细信息, 请参阅[自动升级](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)。
  
若要下载最新版本的 Azure AD Connect, 请[https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)转到。
  

