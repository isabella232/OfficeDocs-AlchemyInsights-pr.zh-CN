---
title: 启用邮箱审核
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 81041685cf383a231a9a9739d6daffd6039b4602
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403737"
---
# <a name="enable-mailbox-auditing"></a>启用邮箱审核

若要为单个用户或整个组织启用邮箱审核, 必须从远程 Power Shell 运行以下 cmdlet:
  
 **单个用户**
  
Set-邮箱-Identity "Jane Dow"-AuditEnabled $true
  
 **组织**
  
ResultSize 无限制-筛选器 {RecipientTypeDetails-eq "UserMailbox"} |Set-邮箱-AuditEnabled $true
  
[了解更多](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

