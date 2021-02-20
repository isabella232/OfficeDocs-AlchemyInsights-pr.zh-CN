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
# <a name="hide-public-folders"></a>隐藏公用文件夹

**若要隐藏整个公用文件夹树，**：

使用本文 [的步骤](https://aka.ms/ControlPF) 选择性用户或所有用户隐藏整个公用文件夹树。

**若要隐藏特定公用文件夹或**：

1. 为需要访问公用文件夹的用户添加权限

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. 从 **权限** 列表中删除 **默认** 权限：

    `Remove-PublicFolderClientPermission \test1 -User Default`
