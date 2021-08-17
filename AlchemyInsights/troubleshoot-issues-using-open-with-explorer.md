---
title: 使用"使用资源管理器打开"解决问题
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 0cbcfb506295d5732f7109be7a103bbdef530a529c7408c6d9d45a7b38a89915
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54048146"
---
# <a name="fix-problems-with-open-with-explorer"></a>修复了"使用资源管理器打开"的问题

修复了使用"使用资源管理器打开"命令在 SharePoint 或 OneDrive **中打开文档库的** 常见问题： 
  
- 使用 Internet Explorer 10 或 Internet Explorer 11。 **使用资源管理器打开** 与浏览器Microsoft Edge Google Chrome、Firefox 和其他设备不兼容。 **"使用资源管理器** 打开"在除浏览器之外的所有浏览器中Internet Explorer。 
    
- **"使用资源管理器** 打开"在新式体验中不适用于SharePoint库。 请 **改为使用文件资源管理器中的视图** 。 选择 **"查看文件** \> **资源管理器"中的"查看"选项**。 文件资源管理器中的视图与 Microsoft Edge、Google Chrome、Firefox 等不兼容。 **在文件资源管理器中查看** ，仅在 Internet Explorer。 
    
- 确保 WebClient 服务正在运行。 在"Windows"框中，键入"运行"，选择"运行桌面应用"，键入 services.msc，然后按 Enter。 向下滚动到 WebClient 服务，并确保" **状态"** 列显示"正在运行"。 如果没有，请双击该服务，再单击 **"启动**"，然后单击"确定 **"。**  (可能需要先在"启动类型"框中选择"手动"或"自动"来启用该服务。)  
    
> [!NOTE]
> 如果需要复制或移动多个文件和文件夹一次，在文件资源管理器中打开库很方便，但如果你想要定期在库中工作，我们建议同步它。 若要解决在文件资源管理器中打开的问题，请参阅 [在资源管理器中打开](https://go.microsoft.com/fwlink/?linkid=871665)。 有关设置同步的信息，请参阅使用SharePoint[客户端同步OneDrive 同步文件](https://go.microsoft.com/fwlink/?linkid=871666)。
  
有关详细信息，请参阅文章[如何使用](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)"使用资源管理器打开"命令排查 SharePoint Online 中的问题。 
  

