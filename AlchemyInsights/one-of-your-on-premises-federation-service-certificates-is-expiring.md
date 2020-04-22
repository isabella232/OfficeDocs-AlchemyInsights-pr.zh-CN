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
ms.openlocfilehash: 24c369c61ad7cf7a9fe101ac29271c32e5159c1f
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43761373"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>你的本地联合身份验证服务证书之一即将过期

若要解决此问题，请按照下列步骤操作：
  
- 在计算机上安装适用于 Windows PowerShell 的 Microsoft Azure Active Directory 模块（如果尚未安装该模块）。 为此，请转到[Azure Active Directory PowerShell For Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- 按照[联合用户登录 Office 365、Azure 或 Intune 时](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)的 "应用场景1： ad fs 令牌签名证书已过期" 一节中的步骤操作，请按照 ad fs 中的 "应用程序访问站点时遇到问题" 错误一节中的步骤操作。
    
- 按照 t 操作方法中的步骤操作[，了解如何更新或修复 Office 365、Azure 或 Intune 中的联盟域的设置](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)。
    
有关续订联合身份验证证书的详细信息，请参阅[用于 O365 和 AZURE AD 的证书续订](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)。
  

