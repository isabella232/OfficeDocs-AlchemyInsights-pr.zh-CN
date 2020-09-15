---
title: ADFS 联合证书即将到期
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686704"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS 联合证书即将到期

若要解决此问题，请按照下列步骤操作：
  
1. 在计算机上安装适用于 Windows PowerShell 的 Microsoft Azure Active Directory 模块 (如果尚未安装该模块) 。 若要执行此操作，请转到 [使用 Windows PowerShell 管理 AZURE AD](https://aka.ms/aadposh)。

2. 按照 [联合用户登录 Microsoft 365、Azure 或 Intune 时](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)的 "应用场景1： ad fs 令牌签名证书已过期" 一节中的步骤操作，请按照 ad fs 中的 "应用程序访问站点时遇到问题" 错误中的步骤操作。

3. 按照 [更新或修复 Microsoft、Azure 或 Intune 中的联盟域的设置](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)中的步骤操作。

    若要了解有关续订联合身份验证证书的详细信息，请参阅 [续订 Microsoft 365 和 Azure Active Directory 的联合身份验证证书](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)。
