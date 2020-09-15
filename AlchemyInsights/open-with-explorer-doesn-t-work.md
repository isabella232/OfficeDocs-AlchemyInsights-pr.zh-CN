---
title: 使用资源管理器打开不起作用
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694446"
---
# <a name="open-with-explorer-isnt-working"></a>使用资源管理器打开不起作用

如果 **使用资源管理器打开** 或 **在文件资源管理器中查看** 不起作用，请按照下面的步骤操作，以确保将 WebClient 服务设置为 " **正在运行** "。 例如，当服务未运行时，可能需要很长时间才能打开 SharePoint 或 OneDrive 库。 
  
1. 在 Windows 搜索框中，键入 "运行"，选择 "运行桌面应用"，键入 "services.msc"，然后选择 " **输入**"。
    
2. 向下滚动到 WebClient 服务并检查 " **状态** " 列。 如果 WebClient 服务状态未 **运行**，请双击该服务，单击 " **开始**"，然后单击 **"确定"**。 如果需要，可通过在 "**启动类型**" 框中选择 "**手动**" 或 "**自动**" 来启用服务。 
    
> [!NOTE]
> 要解决在文件资源管理器中打开的问题，请参阅 [在资源管理器中打开](https://go.microsoft.com/fwlink/?linkid=871665)。 浏览同步作为更好的替代方法： [使用新的 OneDrive 同步客户端同步 SharePoint 文件](https://go.microsoft.com/fwlink/?linkid=871666)。 
  

