---
title: 查看工作流时访问被拒绝
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 43369c600687d6ac253f70a8535dc2bd0d41687e
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29918816"
---
# <a name="access-denied-when-viewing-a-workflow"></a>查看工作流时访问被拒绝

如果 SharePoint 组的成员的未设置为所有人，带有"访问被拒绝"错误消息可能失败尝试向 SharePoint 组发送电子邮件的 SharePoint 2013 工作流。
  
 **若要解决此问题，请执行以下步骤：**
  
 1. 允许所有人查看 SharePoint 组的成员。 
  
 2. 移除 SharePoint 组收件人或抄送行的电子邮件。 
  
 3. 明确将用户添加到收件人或抄送行如果不能更改 SharePoint 组的成员资格可见。 
  
若要查看更多详细信息请参考[HTTP 未经授权到 /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)。
  

