---
title: UPN 同步已禁用
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
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038102"
---
# <a name="upn-sync-disabled"></a>UPN 同步已禁用

如果你在 2016 年 3 月 30 日之前开始同步到 Azure AD，请运行以下 Azure AD PowerShell cmdlet 以仅为组织启用 UPN 软匹配：
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
对于在 2016 年 3 月 30 日或之后开始同步到 Azure AD 的组织，将自动启用 UPN 软匹配。
  
若要了解有关在 UPN 和其他同步功能上启用软匹配的信息，请参阅[Azure AD 连接同步服务功能](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)。
  

