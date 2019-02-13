---
title: ADFS 联合身份验证证书过期
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 55529265d2356a911624026107fb639f93e29abd
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29925370"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS 联合身份验证证书过期

若要解决此问题，请按照下列步骤：
  
1. （如果尚未安装该模块），请在计算机上安装 Microsoft Azure Active Directory 的 Windows PowerShell 的模块。要执行此操作，请转到[管理使用 Windows PowerShell 的 Azure AD](https://aka.ms/aadposh)。
    
2. 请按照"方案 1: AD FS 令牌签名证书过期"部分的["时出现问题访问网站"从 AD FS 的联合的用户登录到 Office 365、 Azure 或 Intune 时的错误](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)。
    
3. 按照[如何更新或修复 Office 365、 Azure 或 Intune 中的联盟域的设置](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)中的步骤。
    
    若要了解有关续订联合身份验证证书的详细信息，请参阅[续订 for Office 365 和 Azure Active Directory 的联合身份验证证书](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)。
    

