---
title: 932 升级 AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9add88a0e4a2590639cbfc546afdcdf5e6aa4886
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28277736"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="4da4d-102">升级 Azure AD 连接</span><span class="sxs-lookup"><span data-stu-id="4da4d-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="4da4d-p101">默认情况下，为 Azure AD 连接，这有助于确保您正在运行的最新版本启用自动升级。若要验证升级的自动设置，请在 Azure AD PowerShell 中使用**Get ADSyncAutoUpgrade** cmdlet。此 cmdlet 将返回下列值之一：</span><span class="sxs-lookup"><span data-stu-id="4da4d-p101">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version. To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell. The cmdlet will return one of following values:</span></span> 
  
- <span data-ttu-id="4da4d-106">**Enabled**： 启用自动升级。</span><span class="sxs-lookup"><span data-stu-id="4da4d-106">**Enabled**: Automatic upgrade is enabled.</span></span> 
    
- <span data-ttu-id="4da4d-107">**禁用**： 禁用自动升级。</span><span class="sxs-lookup"><span data-stu-id="4da4d-107">**Disabled**: Automatic upgrade is disabled.</span></span> 
    
- <span data-ttu-id="4da4d-p102">**Suspended**： 系统不再可以接收自动升级。您不能配置此值;它是由系统设置。</span><span class="sxs-lookup"><span data-stu-id="4da4d-p102">**Suspended**: The system is no longer eligible to receive automatic upgrades. You can't configure this value; it's set by the system.</span></span> 
    
<span data-ttu-id="4da4d-110">有关详细信息，请参阅[自动升级](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)。</span><span class="sxs-lookup"><span data-stu-id="4da4d-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>
  
<span data-ttu-id="4da4d-111">若要下载最新版本的 Azure AD 连接，请转到[https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)。</span><span class="sxs-lookup"><span data-stu-id="4da4d-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
  

