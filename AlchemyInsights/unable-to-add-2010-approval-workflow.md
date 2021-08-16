---
title: 无法添加 2010 审批工作流
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: e74c842f8b4be321664f8c2f1f58c570d0724d80edb1264add0647bf313bc82f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020326"
---
# <a name="unable-to-add-2010-approval-workflow"></a>无法添加 2010 审批工作流

在 Microsoft SharePoint 网站集中，无法将全局可重用工作流 (如"Approval - SharePoint 2010") 列表或库。
  
若要解决此问题，请按照下列步骤操作： 
  
1. 在 SharePoint Designer 2013 中打开网站集的根网站。
  
2. 在"**网站对象"下**，选择"**工作流"。** 
  
3. 在"**工作流"** 功能区的"新建 **"** 部分，选择"**可重用工作流"。** 
  
4. 在" **创建可重用工作流"** 表单上，输入名称 ** *Repair2010* **。 对于 **"平台类型****"，SharePoint"2010 工作流**"，然后单击"确定 **"。** 
  
1. 在"**工作流"功能** 区的"保存 **"** 部分，选择"发布 **"。** 
  
2. 在"**工作流"功能** 区的"管理 **"** 部分，选择"**全局发布"。** 在出现的确认对话框中，选择"确定 **"。** 
  
3. 在 Web 浏览器中，找到网站集的根网站，**然后访问"** 网站集设置 \> **网站集功能"。** 切换 **工作流** 功能： 
  
·如果该功能已 *激活，请单击*"**停用"，** 然后单击"激活 **"。** 
  
·如果功能已停用 *，请单击*"激活 **"。** 
  
有关详细信息，请参阅以下 [文章](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)。
  

