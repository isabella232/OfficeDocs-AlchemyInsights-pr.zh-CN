---
title: 配置文件同步
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a32cf9e623d1be7a2c85ef4951c6eb7f001b7db0
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28277427"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>何时我的配置文件更改同步到 SharePoint 用户配置文件应用程序？

SharePoint Online 使用 Active Directory 导入计时器作业 （AD 导入） 导入用户配置文件应用程序的用户和组。 
  
1. AD 导入同步从 SharePoint Online 目录存储更改为用户配置文件应用程序。批量处理的这些更改。
    
2. 计时器作业运行，直到同步所做的更改。
    
> [!NOTE]
> 要运行的作业的时间取决于要处理的更改的数量。大量更改的时间。服务级别协议 (SLA) 指明，将在 24 小时内中用户配置文件应用程序中反映到 SharePoint Online 目录中的用户的更改。 
  
[有关 SharePoint Online 中的用户配置文件同步的详细信息](https://go.microsoft.com/fwlink/?linkid=875671)
  

