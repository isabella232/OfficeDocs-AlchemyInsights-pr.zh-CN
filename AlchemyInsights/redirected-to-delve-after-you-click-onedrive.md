---
title: OneDrive for BusinessWeb OneDrive重定向到Delve
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 295dea987cd14ea848d2bf802f57429642d554b9661dc4dbfc805a447b7d0ede
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922977"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>单击"Delve后重定向到OneDrive

请参阅我们的详细 [疑难解答指南](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)。

若要解决此问题，管理员必须授予用户创建其"我的网站"网站的权限。 这是因为在"OneDrive for Business"上创建了"网站"页面。

若要授予此权限，请按照以下步骤操作：

1. 在管理SharePoint，单击 **"用户配置文件"。**

2. 在"**人员"** 部分，单击 **"管理用户权限"。**

3. 添加需要权限才能创建其"我的网站"网站的用户。 默认情况下，此设置设置为除外部用户 **以外的所有人**。

4. 添加用户、用户或组后，请确保已选择添加的用户、用户或组，滚动到"权限"部分，然后选中"创建个人网站 ("旁边的复选框（个人存储、新闻源和关注的内容 **) ）。**

5. 单击 **"** 确定"，然后让用户浏览到OneDrive创建网站。
