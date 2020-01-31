---
title: OneDrive for Business Web OneDrive 重定向到 Delve
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 74151ed149c57ceebc841902796189f6638795a9
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571189"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>在你单击 OneDrive 后重定向到 Delve

请参阅我们的详细[故障排除指南](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)。

若要解决此问题，Office 365 管理员必须向用户授予创建其 "我的网站" 网站的权限。 这是因为在 "我的网站" 上创建了 OneDrive for business 页面。

若要授予此权限，请执行以下步骤：

1. 在 SharePoint 管理中心中，单击 "**用户配置文件**"。

2. 在 "**人员**" 部分，单击 "**管理用户权限**"。

3. 添加需要权限才能创建 "我的网站" 网站的用户。 默认情况下，此设置设置为 "**除外部用户之外的所有人**"。

4. 在添加用户、用户或组后，请确保已选中 "已添加用户"、"用户" 或 "组"，滚动到 "**权限**" 部分，然后选中 "**创建个人网站（个人存储、新闻源和关注的内容需要）**" 旁边的复选框。

5. 单击 **"确定**"，然后让用户浏览到 OneDrive 页面以创建网站。
