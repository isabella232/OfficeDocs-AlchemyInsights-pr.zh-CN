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
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="45b03-102">在你单击 OneDrive 后重定向到 Delve</span><span class="sxs-lookup"><span data-stu-id="45b03-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="45b03-103">请参阅我们的详细[故障排除指南](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)。</span><span class="sxs-lookup"><span data-stu-id="45b03-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="45b03-104">若要解决此问题，Office 365 管理员必须向用户授予创建其 "我的网站" 网站的权限。</span><span class="sxs-lookup"><span data-stu-id="45b03-104">To resolve this problem, the Office 365 administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="45b03-105">这是因为在 "我的网站" 上创建了 OneDrive for business 页面。</span><span class="sxs-lookup"><span data-stu-id="45b03-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="45b03-106">若要授予此权限，请执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="45b03-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="45b03-107">在 SharePoint 管理中心中，单击 "**用户配置文件**"。</span><span class="sxs-lookup"><span data-stu-id="45b03-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="45b03-108">在 "**人员**" 部分，单击 "**管理用户权限**"。</span><span class="sxs-lookup"><span data-stu-id="45b03-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="45b03-109">添加需要权限才能创建 "我的网站" 网站的用户。</span><span class="sxs-lookup"><span data-stu-id="45b03-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="45b03-110">默认情况下，此设置设置为 "**除外部用户之外的所有人**"。</span><span class="sxs-lookup"><span data-stu-id="45b03-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="45b03-111">在添加用户、用户或组后，请确保已选中 "已添加用户"、"用户" 或 "组"，滚动到 "**权限**" 部分，然后选中 "**创建个人网站（个人存储、新闻源和关注的内容需要）**" 旁边的复选框。</span><span class="sxs-lookup"><span data-stu-id="45b03-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="45b03-112">单击 **"确定**"，然后让用户浏览到 OneDrive 页面以创建网站。</span><span class="sxs-lookup"><span data-stu-id="45b03-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
