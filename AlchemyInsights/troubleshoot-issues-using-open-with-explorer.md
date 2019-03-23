---
title: 使用 "使用资源管理器打开" 解决问题
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 03bb3ad01a716390ec50845b29ddf6cc81a83116
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2019
ms.locfileid: "30759284"
---
# <a name="fix-problems-with-open-with-explorer"></a>使用 "使用资源管理器打开" 解决问题

修复了使用 "**使用资源管理器打开**" 命令在 SharePoint 或 OneDrive 中打开文档库时遇到的常见问题: 
  
- 使用 internet explorer 10 或 internet explorer 11。 **打开方式浏览器**与 Microsoft Edge、Google Chrome、Firefox 和其他 Microsoft Edge 不兼容。 在除 Internet Explorer 之外的所有浏览器中禁用了 "**使用资源管理器打开**"。 
    
- 在 SharePoint 库的新式体验中不提供 "**使用资源管理器打开**"。 改**为使用文件资源管理器中的视图**。 **在文件资源管理器中选择 "****查看选项** \>视图"。 文件资源管理器中的视图与 Microsoft Edge、Google Chrome、Firefox 和其他项不兼容。 "**文件资源管理器**" 中的视图仅在 Internet Explorer 中可用。 
    
- 请确保 WebClient 服务正在运行。 在 Windows 搜索框中, 键入 "运行", 选择 "运行桌面应用", 键入 services.msc, 然后按 enter。 向下滚动到 WebClient 服务, 并确保 "**状态**" 列显示 "正在运行"。 如果不是, 请双击该服务, 单击 "**开始**", 然后单击 **"确定"**。 (您可能需要先在 "**启动类型**" 框中选择 "**手动**" 或 "**自动**" 来启用该服务。) 
    
> [!NOTE]
> 如果需要复制或移动多个文件和文件夹一次, 则在文件资源管理器中打开库非常方便, 但如果要定期在库中工作, 则建议将其同步。 要解决在文件资源管理器中打开的问题, 请参阅[在资源管理器中打开](https://go.microsoft.com/fwlink/?linkid=871665)。 有关设置同步的信息, 请参阅[sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666)。
  
有关详细信息, 请参阅文章[如何使用 "使用资源管理器打开" 命令来解决 SharePoint Online 中的问题](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)。 
  

