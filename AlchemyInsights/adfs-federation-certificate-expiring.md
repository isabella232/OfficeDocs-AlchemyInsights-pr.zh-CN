---
title: ADFS 联合证书即将到期
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 3ba6e6a6f93225bc843dfd1a028d31223f01280c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821941"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="bc793-102">ADFS 联合证书即将到期</span><span class="sxs-lookup"><span data-stu-id="bc793-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="bc793-103">若要解决此问题，请按照下列步骤操作：</span><span class="sxs-lookup"><span data-stu-id="bc793-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="bc793-104">安装 Microsoft Azure Active Directory 模块，Windows PowerShell在 (（如果尚未安装该模块) ）。</span><span class="sxs-lookup"><span data-stu-id="bc793-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="bc793-105">为此，请转到使用"管理[Azure AD Windows PowerShell"。](https://aka.ms/aadposh)</span><span class="sxs-lookup"><span data-stu-id="bc793-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="bc793-106">按照联合用户登录 [Microsoft 365、Azure](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)或 Intune 时 AD FS 中"方案 1： AD FS 令牌签名证书过期"部分中的步骤操作，从 AD FS 访问站点时出现问题。</span><span class="sxs-lookup"><span data-stu-id="bc793-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="bc793-107">按照更新或 [修复 Microsoft、Azure](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)或 Intune 中的联合域设置中的步骤操作。</span><span class="sxs-lookup"><span data-stu-id="bc793-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="bc793-108">若要了解有关续订联合身份验证证书的信息，请参阅续订 [Microsoft 365](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)和 Azure Active Directory 的联合身份验证证书。</span><span class="sxs-lookup"><span data-stu-id="bc793-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
