---
title: 配置文件同步
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801759"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>何时将我的配置文件更改同步到 SharePoint 用户配置文件应用程序？

SharePoint Online 使用 Active Directory 导入计时器作业 (AD 导入) 将用户和组导入用户配置文件应用程序中。 
  
1. AD 导入将更改从 SharePoint Online 目录存储同步到用户配置文件应用程序。 这些更改在批处理中进行处理。
    
2. 计时器作业将一直运行，直到更改被同步。
    
> [!NOTE]
> 作业运行所需的时间取决于要处理的更改数量。 大量更改需要较长时间。 服务级别协议 (SLA) 声明对 SharePoint Online 目录中的用户所做的更改将在用户配置文件应用程序中在24小时内反映出来。 
  
[有关 SharePoint Online 中的用户配置文件同步的详细信息](https://go.microsoft.com/fwlink/?linkid=875671)
  

