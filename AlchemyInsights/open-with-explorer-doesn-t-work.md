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
ms.openlocfilehash: 2ba6f08b40dd194bf1ffd9a455a134a2fc553b51
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321851"
---
# <a name="open-with-explorer-isnt-working"></a>使用资源管理器打开不工作

如果 **"使用资源管理器打开**"或"在文件资源管理器中查看"不起作用，请确保按照以下步骤将 WebClient 服务设置为"正在运行"。   例如，当服务未运行时，可能需要很长时间SharePoint或OneDrive库。 
  
1. 在"Windows"框中，键入"运行"，选择"运行桌面应用"，键入 services.msc，然后选择 **"Enter"。**
    
2. 向下滚动到 WebClient 服务并检查" **状态"** 列。 如果 WebClient 服务状态未 **运行**，请双击该服务，单击"**启动**"，然后单击"确定 **"。** 如果需要，通过在"启动类型"框中选择"**手动**"或"自动 **"来启用** 该服务。 
    
**注意**：若要解决在文件资源管理器中打开的问题，请参阅 [在资源管理器中打开](https://go.microsoft.com/fwlink/?linkid=871665)。 探索同步作为更好的替代方法[：SharePoint客户端同步OneDrive 同步文件](https://go.microsoft.com/fwlink/?linkid=871666)。 
  

