---
title: 使用资源管理器打开不起作用
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 7680766b53bd5e85789375d3f9e9ab635780ec6c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538453"
---
# <a name="open-with-explorer-isnt-working"></a>使用资源管理器打开不起作用

如果**使用资源管理器打开**或**在文件资源管理器中查看**不起作用, 请按照下面的步骤操作, 以确保将 WebClient 服务设置为 "**正在运行**"。 例如, 当服务未运行时, 可能需要很长时间才能打开 SharePoint 或 OneDrive 库。 
  
1. 在 Windows 搜索框中, 键入 "运行", 选择 "运行桌面应用", 键入 "services.msc", 然后选择 "**输入**"。
    
2. 向下滚动到 WebClient 服务并检查 "**状态**" 列。 如果 WebClient 服务状态未**运行**, 请双击该服务, 单击 "**开始**", 然后单击 **"确定"**。 如果需要, 可通过在 "**启动类型**" 框中选择 "**手动**" 或 "**自动**" 来启用服务。 
    
> [!NOTE]
> 要解决在文件资源管理器中打开的问题, 请参阅[在资源管理器中打开](https://go.microsoft.com/fwlink/?linkid=871665)。 浏览同步作为更好的替代方法:[使用新的 OneDrive 同步客户端同步 SharePoint 文件](https://go.microsoft.com/fwlink/?linkid=871666)。 
  

