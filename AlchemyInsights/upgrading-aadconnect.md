---
title: 932升级 AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806029"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="8381a-102">升级 Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="8381a-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="8381a-103">默认情况下，启用了 Azure AD Connect 的自动升级，这有助于确保你运行的是最新版本。</span><span class="sxs-lookup"><span data-stu-id="8381a-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="8381a-104">若要验证自动升级设置，请在 Azure AD PowerShell 中使用 **ADSyncAutoUpgrade** cmdlet。</span><span class="sxs-lookup"><span data-stu-id="8381a-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="8381a-105">Cmdlet 将返回以下值之一：</span><span class="sxs-lookup"><span data-stu-id="8381a-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="8381a-106">**Enabled**：已启用自动升级。</span><span class="sxs-lookup"><span data-stu-id="8381a-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="8381a-107">**Disabled**：自动升级已禁用。</span><span class="sxs-lookup"><span data-stu-id="8381a-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="8381a-108">已**挂起**：系统不再符合接收自动升级的条件。</span><span class="sxs-lookup"><span data-stu-id="8381a-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="8381a-109">您不能配置此值;它是由系统设置的。</span><span class="sxs-lookup"><span data-stu-id="8381a-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="8381a-110">有关详细信息，请参阅 [自动升级](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)。</span><span class="sxs-lookup"><span data-stu-id="8381a-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="8381a-111">若要下载最新版本的 Azure AD Connect，请转到 [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) 。</span><span class="sxs-lookup"><span data-stu-id="8381a-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
