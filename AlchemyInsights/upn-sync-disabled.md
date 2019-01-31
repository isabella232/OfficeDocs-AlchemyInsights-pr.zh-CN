---
title: 禁用的 UPN 同步
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
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 027782bb2a6b892df6201f3c3bf55151ef7b9db7
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657961"
---
# <a name="upn-sync-disabled"></a>禁用的 UPN 同步

如果您启动同步到 Azure AD 之前 2016，年 3 月 30，运行以下的 Azure AD PowerShell cmdlet，以便为您的组织仅 UPN 软匹配：
  
 **设置 MsolDirSyncFeature-功能 EnableSoftMatchOnUpn-启用 $True**
  
自动启动同步到当天或之后 2016 年 3 月 30，Azure AD 的组织开启 UPN 软匹配。
  
要了解有关启用软匹配 UPN 和其他同步功能，请参阅[Azure AD 连接同步服务功能](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)。
  

