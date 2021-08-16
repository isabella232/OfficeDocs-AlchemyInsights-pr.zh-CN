---
title: 限制访问SharePoint或OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b7b68df2ae24b09fe9b01bd67c31a89e37f284a512bc1ecb097ef52fae5ae7d6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54075030"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>限制访问SharePoint或OneDrive

在SharePoint和OneDrive中，您仅向希望具有访问权限的组或个人授予访问权限，从而限制对文件、文件夹和列表等项目的访问。 默认情况下，SharePoint中的权限继承自层次结构的上一层。 因此，文件从文件夹继承其权限，该文件夹从库继承其权限，而库从网站继承其权限。
  
可以在较高级别共享 (例如共享整个网站集) 如果您不想共享网站上的所有项目，可以中断继承。 但是，我们不建议这样做，因为这会使将来保留权限变得更加复杂和混乱。 下面是您可以改为执行哪些功能：
  
- 例如，如果要共享文件夹（其中一个文件除外）的所有内容，将该文件移动到不共享的新位置。
    
- 如果文件夹中有两个子文件夹，并且希望与组 A 和组 B 共享一个子文件夹，并且只允许组 A 访问第二个子文件夹，请与组 A 共享父文件夹，然后向第一个子文件夹添加组 B。
    
[停止共享文件或文件夹 ](https://go.microsoft.com/fwlink/?linkid=2008861)
  

