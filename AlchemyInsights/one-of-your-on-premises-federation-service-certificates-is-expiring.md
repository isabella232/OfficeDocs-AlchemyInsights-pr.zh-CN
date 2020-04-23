---
title: 你的本地联合身份验证服务证书之一即将过期
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: dafa344ec649002900e98a5e183b3e5f759707e1
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43785293"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="d4d84-102">你的本地联合身份验证服务证书之一即将过期</span><span class="sxs-lookup"><span data-stu-id="d4d84-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="d4d84-103">若要解决此问题，请按照下列步骤操作：</span><span class="sxs-lookup"><span data-stu-id="d4d84-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="d4d84-104">在计算机上安装适用于 Windows PowerShell 的 Microsoft Azure Active Directory 模块（如果尚未安装该模块）。</span><span class="sxs-lookup"><span data-stu-id="d4d84-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="d4d84-105">为此，请转到[Azure Active Directory PowerShell For Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="d4d84-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="d4d84-106">按照[联合用户登录 Microsoft 365、Azure 或 Intune 时](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)的 "应用场景1： ad fs 令牌签名证书已过期" 一节中的步骤操作，请按照 ad fs 中的 "应用程序访问站点时遇到问题" 错误中的步骤操作。</span><span class="sxs-lookup"><span data-stu-id="d4d84-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="d4d84-107">按照[如何更新或修复 Microsoft 365、Azure 或 Intune 中的联盟域的设置](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)中的步骤操作。</span><span class="sxs-lookup"><span data-stu-id="d4d84-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="d4d84-108">有关续订联合身份验证证书的详细信息，请参阅[用于 O365 和 AZURE AD 的证书续订](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)。</span><span class="sxs-lookup"><span data-stu-id="d4d84-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

