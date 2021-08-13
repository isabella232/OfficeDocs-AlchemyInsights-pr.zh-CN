---
title: 将驱动器映射到驱动器时拒绝SharePoint
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
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: 1ed67ec926c3e73f7a16b927729255505dfe93a0ae442a5dff9400afafb41d8e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938721"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a>修复了SharePoint网络驱动器的库的问题

当您浏览到映射的网络驱动器时，您可能会看到以下消息之一：
  
- **\\路径不可访问。您可能没有使用此网络资源的权限。请与此服务器的管理员联系，了解您是否具有访问权限。**

- **访问被拒绝。在此位置打开文件之前，必须先将网站添加到受信任的网站列表，浏览到该网站，然后选择自动登录选项。**

[获取有关映射的网络驱动器疑难解答的帮助](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)。
  
将库映射为网络驱动器是临时的，仅在 Internet Explorer。 相反[，SharePoint新客户端同步OneDrive 同步文件](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx)随[需要客户端](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx)。 无需本地存储空间即可访问所有 OneDrive 中的文件。
  