---
title: 隐藏公用文件夹
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50294637"
---
# <a name="hide-public-folders"></a><span data-ttu-id="64024-102">隐藏公用文件夹</span><span class="sxs-lookup"><span data-stu-id="64024-102">Hide public folders</span></span>

<span data-ttu-id="64024-103">**若要隐藏整个公用文件夹树，**：</span><span class="sxs-lookup"><span data-stu-id="64024-103">**To hide entire public folder tree**:</span></span>

<span data-ttu-id="64024-104">使用本文 [的步骤](https://aka.ms/ControlPF) 选择性用户或所有用户隐藏整个公用文件夹树。</span><span class="sxs-lookup"><span data-stu-id="64024-104">Use the steps in [this](https://aka.ms/ControlPF) article to hide entire public folder tree from selective or all users.</span></span>

<span data-ttu-id="64024-105">**若要隐藏特定公用文件夹或**：</span><span class="sxs-lookup"><span data-stu-id="64024-105">**To hide a specific public folder**:</span></span>

1. <span data-ttu-id="64024-106">为需要访问公用文件夹的用户添加权限</span><span class="sxs-lookup"><span data-stu-id="64024-106">Add permissions for users who need to access the public folder</span></span>

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. <span data-ttu-id="64024-107">从 **权限** 列表中删除 **默认** 权限：</span><span class="sxs-lookup"><span data-stu-id="64024-107">Remove the user **Default** from the **permission** list:</span></span>

    `Remove-PublicFolderClientPermission \test1 -User Default`
