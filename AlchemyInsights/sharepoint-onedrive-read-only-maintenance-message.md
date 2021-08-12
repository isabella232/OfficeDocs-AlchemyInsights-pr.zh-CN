---
title: Read-Only尝试使用"维护"或"维护"SharePoint OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: edcdea2f5c0647b92c230dd1d86549173e72997fc885195cde688b3b17710a2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910536"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only尝试使用"维护"或"维护"SharePoint OneDrive

用户在尝试对以下 **方案之** 一使用 SharePoint 或 OneDrive 时，可能会收到"维护只读"消息。 

-   计划或活动的维护活动。  通过导航到消息中心 [来检查它们](https://portal.office.com/adminportal/home#/messagecenter)。
-   可能发生的高优先级活动服务事件。 通过导航到"服务运行状况"，检查是否有 [公告/事件](https://portal.office.com/adminportal/home#/servicehealth)。
-   可能会由于服务器上可能持续不到 30 分钟的任何意外事件而发生的次要自动修复恢复方案。 
    
    这些次要恢复没有消息中心或服务运行状况帖子，但应该很快就会恢复正常。

在极少数情况下，我们观察到上面列出的三种方案之一是原因，并且服务已还原，但用户浏览器缓存尚未清除。

请在导航到网站之前尝试清除浏览器缓存。

1. 在浏览器Microsoft Edge，选择"设置"，然后选择"**隐私和安全"。**
2. 在 **"清除浏览"** 下 **，选择"选择要清除哪些内容"。**
3. 选择 **"Cookie 和保存的网站数据"，** 然后选择"清除 **"。**

>[!Note] 
> 当使用 Mozilla Firefox 或 Google Chrome 等其他浏览器时，这些步骤可能会有所不同。

>[!Note] 
> 另一个选项是，在SharePoint InPrivate OneDrive打开您的网站或网站。