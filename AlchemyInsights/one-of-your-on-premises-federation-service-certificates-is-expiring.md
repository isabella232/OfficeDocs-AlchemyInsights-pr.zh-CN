---
title: 一个内部部署联合身份验证服务证书即将过期
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 89a4dd910d43d70e849be19d5f88e281f6d19834
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28277048"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="8ae26-102">一个内部部署联合身份验证服务证书即将过期</span><span class="sxs-lookup"><span data-stu-id="8ae26-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="8ae26-103">若要解决此问题，请按照下列步骤：</span><span class="sxs-lookup"><span data-stu-id="8ae26-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="8ae26-p101">（如果尚未安装该模块），请在计算机上安装 Microsoft Azure Active Directory 的 Windows PowerShell 的模块。若要执行此操作，请转到[Azure Active Directory PowerShell 图形](https://docs.microsoft.com/en-us/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="8ae26-p101">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed). To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/en-us/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="8ae26-106">请按照"方案 1: AD FS 令牌签名证书过期"部分的["时出现问题访问网站"从 AD FS 的联合的用户登录到 Office 365、 Azure 或 Intune 时的错误](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)。</span><span class="sxs-lookup"><span data-stu-id="8ae26-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="8ae26-107">按照 t[如何更新或修复 Office 365、 Azure 或 Intune 中的联盟域的设置](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)中的步骤。</span><span class="sxs-lookup"><span data-stu-id="8ae26-107">Follow the steps in t[How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="8ae26-108">有关续订联合身份验证证书的详细信息，请参阅[证书续订 O365 和 Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs)。</span><span class="sxs-lookup"><span data-stu-id="8ae26-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

