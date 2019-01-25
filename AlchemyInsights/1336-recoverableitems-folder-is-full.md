---
title: 1336 RecoverableItems 文件夹已满
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: ee96abfa179c36ebaf43dbd327d4608b849395d3
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29459414"
---
# <a name="the-recoverable-items-folder-is-full"></a>可恢复邮件文件夹已满

Office 365 中的 Exchange Online 邮箱，可恢复邮件文件夹的默认存储限制为 30 GB。如果邮箱置于诉讼保留电子数据展示保留或已分配给 Office 365 保留策略，可恢复邮件文件夹的存储限制会自动增加到 100 GB。
  
当可恢复邮件文件夹达到的存储限制时，邮箱功能将受到影响以下方式：
  
- 用户无法从邮箱中删除项目。
    
- 托管文件夹助理无法基于保留标记或托管文件夹设置删除项目。
    
- 已启用的单个项目恢复或置于保持状态的邮箱，写入时复制页保护过程无法保持用户编辑的项目的版本。
    
- 具有邮箱审核日志记录启用的邮箱，可以在可恢复邮件文件夹中的审核子文件夹中保存没有邮箱审核日志条目。
    
对于不是置于保持状态的邮箱，管理员可以使用`Search-Mailbox -SearchDumpsterOnly -DeleteContent`命令在 Exchange Online PowerShell 中删除可恢复邮件文件夹中的项目。有关详细信息，请参阅以下主题： 
  
- [搜索和删除邮件](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- Search-Mailbox
    
对于处于保持状态的邮箱，管理员必须删除保留，他们可以从可恢复邮件文件夹的已删除的项目之前。有关详细信息，请参阅[删除在可恢复项目文件夹中的基于云的邮箱的保留的项目](https://docs.microsoft.com/en-us/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)。
  
为了帮助防止成为完整可恢复邮件文件夹，管理员可以提高可恢复的项目文件夹上邮箱保留和设置将项目从可恢复邮件文件夹移动到用户的存档邮箱保留策略的存储限制邮箱。请参阅[提高可恢复的项目上的邮箱配额保留](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold)。
  

