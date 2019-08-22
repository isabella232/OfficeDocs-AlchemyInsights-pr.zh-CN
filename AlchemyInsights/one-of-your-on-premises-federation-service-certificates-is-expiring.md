---
title: 你的本地联合身份验证服务证书之一即将过期
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 00cbc77cb178d59a3115e44874a16f506e4408c6
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543555"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>你的本地联合身份验证服务证书之一即将过期

若要解决此问题, 请按照下列步骤操作:
  
- 在计算机上安装适用于 Windows PowerShell 的 Microsoft Azure Active Directory 模块 (如果尚未安装该模块)。 为此, 请转到[Azure Active Directory PowerShell For Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- 按照[联合用户登录 Office 365、Azure 或 Intune 时](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)的 "应用场景 1: ad fs 令牌签名证书已过期" 一节中的步骤操作, 请按照 ad fs 中的 "应用程序访问站点时遇到问题" 错误一节中的步骤操作。
    
- 按照 t 操作方法中的步骤操作[, 了解如何更新或修复 Office 365、Azure 或 Intune 中的联盟域的设置](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)。
    
有关续订联合身份验证证书的详细信息, 请参阅[用于 O365 和 AZURE AD 的证书续订](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)。
  

