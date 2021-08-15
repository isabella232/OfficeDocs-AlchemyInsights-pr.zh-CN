---
title: 查看工作流时拒绝访问
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955191"
---
# <a name="access-denied-when-viewing-a-workflow"></a>查看工作流时拒绝访问

SharePoint 2013 如果 SharePoint 组的成员身份未设置为"任何人"，则尝试向 SharePoint 组发送电子邮件的工作流可能会失败，并出现"拒绝访问"错误消息。
  
 **若要解决此问题，请执行以下步骤：**
  
 1. 允许每个人查看组SharePoint成员。
  
 2. 从SharePoint"或"抄送"行中删除组。
  
 3. 如果无法更改组的成员可见性，则向"目标"或"抄送"行SharePoint用户。
  
若要查看更多详细信息，请参阅 HTTP [Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)。
  