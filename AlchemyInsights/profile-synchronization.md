---
title: 配置文件同步
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: d1a72a85767e36fefbfa8eee266befcaf2e48af0
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371974"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>何时将我的配置文件更改同步到 SharePoint 用户配置文件应用程序？

SharePoint Online 使用 Active Directory 导入计时器作业 (AD 导入) 将用户和组导入到用户配置文件应用程序中。 
  
1. AD 导入将更改从 SharePoint Online 目录存储同步到用户配置文件应用程序。 这些更改在批处理中进行处理。
    
2. 计时器作业将一直运行, 直到更改被同步。
    
> [!NOTE]
> 作业运行所需的时间取决于要处理的更改数量。 大量更改需要较长时间。 服务级别协议 (SLA) 指出对 SharePoint Online 目录中的用户所做的更改将在24小时内反映到用户配置文件应用程序中。 
  
[有关 SharePoint Online 中的用户配置文件同步的详细信息](https://go.microsoft.com/fwlink/?linkid=875671)
  

