---
title: 公用文件夹迁移批处理未完成，显示已同步
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: 33302110249b02aef87639792ebfd9cafd6638c0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771484"
---
# <a name="public-folder-migration-batch-not-completing-shows-synced"></a><span data-ttu-id="b366c-102">公用文件夹迁移批处理未完成，显示已同步</span><span class="sxs-lookup"><span data-stu-id="b366c-102">Public folder migration batch not completing, shows synced</span></span>

<span data-ttu-id="b366c-103">你可能已启动迁移批处理的完成，但迁移批处理的状态在很长一段时间内持续显示为“已同步”。</span><span class="sxs-lookup"><span data-stu-id="b366c-103">You may have initiated completion of migration batch and status of the migration batch continues showing "Synced" for very long time.</span></span> <span data-ttu-id="b366c-104">这是正常的现象。</span><span class="sxs-lookup"><span data-stu-id="b366c-104">This is expected behavior.</span></span>

<span data-ttu-id="b366c-105">迁移批处理的状态往往会仍保持在“已同步”状态几个小时，然后才会切换到“正在完成”。</span><span class="sxs-lookup"><span data-stu-id="b366c-105">It's common for the status of migration batch to remain on Synced for a few hours before it switches to Completing.</span></span> <span data-ttu-id="b366c-106">对于涉及大量目标邮箱的迁移，如果没有任何基础公用文件夹迁移请求失败或被隔离，则保持在已同步状态超过 24 小时的情况是正常的。</span><span class="sxs-lookup"><span data-stu-id="b366c-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the Synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="b366c-107">请为迁移批处理留出 24-48 小时的时间来完成任务。</span><span class="sxs-lookup"><span data-stu-id="b366c-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>
