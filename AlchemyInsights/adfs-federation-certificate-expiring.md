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
ms.custom: ''
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 518261787b1b0df99ee7b3dc3e51dec70e4373bc
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32398330"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS 联合身份验证证书即将过期

若要解决此问题, 请按照下列步骤操作:
  
1. 在计算机上安装适用于 Windows PowerShell 的 Microsoft Azure Active Directory 模块 (如果尚未安装该模块)。 若要执行此操作, 请转到[使用 Windows PowerShell 管理 Azure AD](https://aka.ms/aadposh)。
    
2. 按照[联合用户登录 Office 365、Azure 或 Intune 时](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)的 "应用场景 1: ad fs 令牌签名证书已过期" 一节中的步骤操作, 请按照 ad fs 中的 "应用程序访问站点时遇到问题" 错误一节中的步骤操作。
    
3. 按照[如何更新或修复 Office 365、Azure 或 Intune 中的联盟域的设置](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)中的步骤操作。
    
    若要了解有关续订联合身份验证证书的详细信息, 请参阅[续订 Office 365 和 Azure Active Directory 的联合身份验证证书](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)。
    

