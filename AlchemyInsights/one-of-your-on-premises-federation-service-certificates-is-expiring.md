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
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>一个内部部署联合身份验证服务证书即将过期

若要解决此问题，请按照下列步骤：
  
- （如果尚未安装该模块），请在计算机上安装 Microsoft Azure Active Directory 的 Windows PowerShell 的模块。若要执行此操作，请转到[Azure Active Directory PowerShell 图形](https://docs.microsoft.com/en-us/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- 请按照"方案 1: AD FS 令牌签名证书过期"部分的["时出现问题访问网站"从 AD FS 的联合的用户登录到 Office 365、 Azure 或 Intune 时的错误](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)。
    
- 按照 t[如何更新或修复 Office 365、 Azure 或 Intune 中的联盟域的设置](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)中的步骤。
    
有关续订联合身份验证证书的详细信息，请参阅[证书续订 O365 和 Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs)。
  

