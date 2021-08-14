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
ms.openlocfilehash: b223bad66fb7cc6d1d7c0a2b3ccc7a081c061b4974060dbcafec84dfb24eb782
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923634"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>我的配置文件更改何时同步到SharePoint用户配置文件应用程序？

SharePointOnline 使用 Active Directory 导入计时器作业 (AD 导入) 将用户和组导入用户配置文件应用程序。 
  
1. AD 导入将更改从 SharePoint Online 目录存储同步到用户配置文件应用程序。 这些更改将分批处理。
    
2. 计时器作业将一直运行，直到同步更改。
    
> [!NOTE]
> 运行作业所花的时间取决于要处理的更改数。 大量更改需要更长时间。 服务级别协议 (SLA) 规定，对 SharePoint Online 目录中的用户更改将在 24 小时内反映在用户配置文件应用程序中。 
  
[有关 SharePoint Online 中的用户配置文件同步详细信息](https://go.microsoft.com/fwlink/?linkid=875671)
  

