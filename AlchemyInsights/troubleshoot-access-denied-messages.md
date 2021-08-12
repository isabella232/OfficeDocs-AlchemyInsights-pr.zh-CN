---
title: 拒绝访问邮件疑难解答
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c62186fd346efd539b13cef9c80f5e797ebf80811a21db73f0f07fd86c080d55
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939873"
---
# <a name="troubleshoot-access-denied-messages"></a>拒绝访问邮件疑难解答

如果某人收到对 SharePoint 共享文件夹的"拒绝访问"邮件，则网站集管理员可能已启用"受限访问用户权限锁定模式"。 若要关闭此功能， 
  
1. 浏览到该网站，单击"设置"图标，然后单击"网站 **设置"。**
    
2. 在“网站集管理”下，单击“网站集功能”。
    
3. 在 **"受限访问用户权限锁定模式"旁边，** 单击"**停用"。**
    
如果共享文件夹是发布网站，则也会发生"访问被拒绝"消息。 有关信息，请参阅 [访问共享文件夹时拒绝访问](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb)。
  
如果某人在尝试查看访问请求时收到"拒绝访问"消息，则用户需要添加为网站集管理员或网站 Owners 组的成员。 有关详细信息，请参阅访问 [被拒绝访问请求列表](https://go.microsoft.com/fwlink/?linkid=2004220)。
  
如果用户从本地 Active Directory 中删除并添加回后收到"访问被拒绝"消息，请参阅将用户帐户同步到 Active Directory 时拒绝[Microsoft 365。](https://go.microsoft.com/fwlink/?linkid=2004318)
  

