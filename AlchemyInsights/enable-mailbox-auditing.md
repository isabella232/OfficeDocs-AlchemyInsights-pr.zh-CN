---
title: 启用邮箱审核
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: bd94ec10f9df2e72ec6e3d8552d2eb80212a9d78
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28276868"
---
# <a name="enable-mailbox-auditing"></a>启用邮箱审核

若要为单个用户或整个组织中启用邮箱审核必须从远程电源命令行管理程序运行以下 cmdlet:
  
 **单个用户**
  
Set-mailbox-Identity"Jane Dow"AuditEnabled $true
  
 **组织**
  
Get-mailbox ResultSize 不受限制的筛选 {RecipientTypeDetails-eq"UserMailbox"} |设置邮箱 AuditEnabled $true
  
[了解更多](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

