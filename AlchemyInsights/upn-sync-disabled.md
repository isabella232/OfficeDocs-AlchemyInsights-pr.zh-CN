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
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782141"
---
# <a name="upn-sync-disabled"></a>UPN 同步已禁用

如果你在 2016 年 3 月 30 日之前开始同步到 Azure AD，请运行以下 Azure AD PowerShell cmdlet 以仅为组织启用 UPN 软匹配：
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
对于在 2016 年 3 月 30 日或之后开始同步到 Azure AD 的组织，将自动启用 UPN 软匹配。
  
若要了解有关在 UPN 和其他同步功能上启用软匹配功能的信息，请参阅 [Azure AD Connect 同步服务功能](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)。
  

