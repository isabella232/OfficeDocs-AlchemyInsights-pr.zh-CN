---
title: 无法激活缺少的工作流
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 44fd3c2d1e8b278b47c0fde6d48c7cbcbaa5c324
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543915"
---
# <a name="missing-workflow-failed-to-activate"></a>无法激活缺少的工作流

在 Microsoft SharePoint 网站集中, 无法将全局可重用工作流 (如 "审批-SharePoint 2010") 添加到列表或库。
  
若要解决此问题, 请按照下列步骤操作: 
  
1. 在 SharePoint Designer 2013 中打开网站集的根网站。
  
2. 在 "**网站对象**" 下, 选择 "**工作流**"。 
  
3. 在 "**工作流**" 功能区的 "**新建**" 部分, 选择 "**可重用工作流**"。 
  
4. 在 "**创建可重用工作流**" 表单中, 输入名称 * * *Repair2010* * *。 对于 "**平台类型**", 单击 " **SharePoint 2010 工作流**", 然后单击 **"确定"**。 
  
1. 在 "**工作流**" 功能区的 "**保存**" 部分, 选择 "**发布**"。 
  
2. 在 "**工作流**" 功能区的 "**管理**" 部分, 选择 "**全局发布**"。 在出现的确认对话框中, 选择 **"确定"**。 
  
3. 在 web 浏览器中, 找到网站集的根网站, 然后访问 "**网站设置** \> "**网站集功能**。 然后, 切换**工作流**功能: 
  
·如果功能已*激活*, 请单击 "**停用",** 然后单击 "**激活**"。 
  
·如果*禁用*该功能, 请单击 "**激活**"。 
  
有关详细信息, 请参阅以下[文章](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)。
  

