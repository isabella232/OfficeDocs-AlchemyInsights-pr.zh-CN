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
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952959"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS 联合证书即将到期

若要解决此问题，请按照下列步骤操作：
  
1. 如果Microsoft Azure Active Directory模块Windows PowerShell，则 (安装模块以用于) 。 为此，请转到使用"管理[Azure AD Windows PowerShell"。](https://aka.ms/aadposh)

2. 按照联合用户登录[Microsoft 365、Azure 或 Intune 时来自 AD FS](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)的"方案 1： AD FS 令牌签名证书过期"部分中的步骤操作，从 AD FS 访问站点时出现问题。

3. 按照更新或 [修复 Microsoft、Azure](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)或 Intune 中的联合域设置中的步骤操作。

    若要了解有关续订联合身份验证证书的更多信息，请参阅续订联合身份验证证书[Microsoft 365和Azure Active Directory。](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
