---
title: 您的本地联合身份验证服务证书之一即将过期
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
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 45a679e83aa8f07d65d2e7e84d7eb2a2b5a721e8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810042"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>您的本地联合身份验证服务证书之一即将过期

若要解决此问题，请按照下列步骤操作：
  
- 安装 Microsoft Azure Active Directory 模块，Windows PowerShell在 (（如果尚未安装该模块) ）。 为此，请转到 Azure [Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- 按照联合用户登录 [Microsoft 365、Azure](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)或 Intune 时 AD FS 中"方案 1： AD FS 令牌签名证书过期"部分中的步骤操作，从 AD FS 访问站点时出现问题。
    
- 按照如何在 [Microsoft 365、Azure](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)或 Intune 中更新或修复联合域的设置中的步骤操作。
    
有关续订联合身份验证证书的信息，请参阅 [O365](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)和 Azure AD 的证书续订。
  

