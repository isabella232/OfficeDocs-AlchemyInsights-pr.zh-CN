---
title: 启用邮箱审核
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: ae11d6be0789a5662d202b85268480a3d42922c4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703561"
---
# <a name="enable-mailbox-auditing"></a>启用邮箱审核

若要为单个用户或整个组织启用邮箱审核，必须从远程 Power Shell 运行以下 cmdlet：
  
 **单个用户**
  
Set-邮箱-Identity "Jane Dow"-AuditEnabled $true
  
 **组织**
  
ResultSize 无限制-筛选器 {RecipientTypeDetails-eq "UserMailbox"} |Set-邮箱-AuditEnabled $true
  
[了解更多](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

