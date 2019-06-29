---
title: ADFS 联合身份验证证书即将过期
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: b014e350d5f6f1a61feb223e3d3fd0a1f56f5872
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35357955"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="2caf7-102">ADFS 联合身份验证证书即将过期</span><span class="sxs-lookup"><span data-stu-id="2caf7-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="2caf7-103">若要解决此问题, 请按照下列步骤操作:</span><span class="sxs-lookup"><span data-stu-id="2caf7-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="2caf7-104">在计算机上安装适用于 Windows PowerShell 的 Microsoft Azure Active Directory 模块 (如果尚未安装该模块)。</span><span class="sxs-lookup"><span data-stu-id="2caf7-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="2caf7-105">若要执行此操作, 请转到[使用 Windows PowerShell 管理 AZURE AD](https://aka.ms/aadposh)。</span><span class="sxs-lookup"><span data-stu-id="2caf7-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="2caf7-106">按照[联合用户登录 Office 365、Azure 或 Intune 时](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)的 "应用场景 1: ad fs 令牌签名证书已过期" 一节中的步骤操作, 请按照 ad fs 中的 "应用程序访问站点时遇到问题" 错误一节中的步骤操作。</span><span class="sxs-lookup"><span data-stu-id="2caf7-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="2caf7-107">按照[如何更新或修复 Office 365、Azure 或 Intune 中的联盟域的设置](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)中的步骤操作。</span><span class="sxs-lookup"><span data-stu-id="2caf7-107">Follow the steps in [How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>

    <span data-ttu-id="2caf7-108">若要了解有关续订联合身份验证证书的详细信息, 请参阅[续订 Office 365 和 Azure Active Directory 的联合身份验证证书](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)。</span><span class="sxs-lookup"><span data-stu-id="2caf7-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
