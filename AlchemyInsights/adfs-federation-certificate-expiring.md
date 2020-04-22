---
title: ADFS 联合身份验证证书即将过期
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710397"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS 联合身份验证证书即将过期

若要解决此问题，请按照下列步骤操作：
  
1. 在计算机上安装适用于 Windows PowerShell 的 Microsoft Azure Active Directory 模块（如果尚未安装该模块）。 若要执行此操作，请转到[使用 Windows PowerShell 管理 AZURE AD](https://aka.ms/aadposh)。

2. 按照[联合用户登录 Microsoft 365、Azure 或 Intune 时](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)的 "应用场景1： ad fs 令牌签名证书已过期" 一节中的步骤操作，请按照 ad fs 中的 "应用程序访问站点时遇到问题" 错误中的步骤操作。

3. 按照[更新或修复 Microsoft、Azure 或 Intune 中的联盟域的设置](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)中的步骤操作。

    若要了解有关续订联合身份验证证书的详细信息，请参阅[续订 Microsoft 365 和 Azure Active Directory 的联合身份验证证书](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)。
