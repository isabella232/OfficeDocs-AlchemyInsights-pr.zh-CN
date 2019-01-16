---
title: 无法添加默认 2010年审批工作流
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28276880"
---
# <a name="cant-add-default-2010-approval-workflow"></a>无法添加默认 2010年审批工作流

Microsoft SharePoint 网站集，您不能对列表或库添加全局可重用工作流 （如"审批-SharePoint 2010"）。
  
若要解决此问题，请按照下列步骤： 
  
1. 在 SharePoint Designer 2013 中打开的网站集的根网站。
  
2. 在**网站对象**下选择**工作流**。 
  
3. 在**工作流**功能区的**新建**部分中，选择**可重用工作流**。 
  
4. 在**创建可重用工作流**表单上，输入名称 * **Repair2010***。**平台类型**，选择**SharePoint 2010 工作流**，，然后选择**确定**。 
  
5. 在**工作流**功能区的**保存**部分中，选择**发布**。 
  
6. 在**工作流**功能区的**管理**部分中，选择**全局发布**。在显示确认对话框中，选择**确定**。 
  
7. 在 web 浏览器中，找到网站集的根网站，然后访问**网站设置** \> **网站集功能**。然后，切换的**工作流**功能： 
  
·*已激活*功能时，单击**停用，** ，然后单击**激活**。 
  
·如果*已停用*功能，请单击**激活**。 
  
有关详细信息请参阅以下[文章](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)。
  

