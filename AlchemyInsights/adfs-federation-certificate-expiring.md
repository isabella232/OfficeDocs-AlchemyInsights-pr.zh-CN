---
title: ADFS 联合身份验证证书过期
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: c608489be8497233d9d4f87ec53649026b823250
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28277308"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="39b87-102">ADFS 联合身份验证证书过期</span><span class="sxs-lookup"><span data-stu-id="39b87-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="39b87-103">若要解决此问题，请按照下列步骤：</span><span class="sxs-lookup"><span data-stu-id="39b87-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="39b87-p101">（如果尚未安装该模块），请在计算机上安装 Microsoft Azure Active Directory 的 Windows PowerShell 的模块。要执行此操作，请转到[管理使用 Windows PowerShell 的 Azure AD](https://aka.ms/aadposh)。</span><span class="sxs-lookup"><span data-stu-id="39b87-p101">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed). To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>
    
2. <span data-ttu-id="39b87-106">请按照"方案 1: AD FS 令牌签名证书过期"部分的["时出现问题访问网站"从 AD FS 的联合的用户登录到 Office 365、 Azure 或 Intune 时的错误](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)。</span><span class="sxs-lookup"><span data-stu-id="39b87-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
3. <span data-ttu-id="39b87-107">按照[如何更新或修复 Office 365、 Azure 或 Intune 中的联盟域的设置](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)中的步骤。</span><span class="sxs-lookup"><span data-stu-id="39b87-107">Follow the steps in [How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
    <span data-ttu-id="39b87-108">若要了解有关续订联合身份验证证书的详细信息，请参阅[续订 for Office 365 和 Azure Active Directory 的联合身份验证证书](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs)。</span><span class="sxs-lookup"><span data-stu-id="39b87-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
    

