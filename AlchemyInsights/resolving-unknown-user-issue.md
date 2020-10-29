---
title: 解决团队聊天中的未知用户的问题
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003807"
- "6809"
ms.openlocfilehash: 523c11cb9d5c4696703c67c2a6b3184f5d12f8e7
ms.sourcegitcommit: d151b09064df3fb573ae07a387a08d98a9553b9b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/28/2020
ms.locfileid: "48785563"
---
# <a name="resolving-issue-with-unknown-user-in-teams-chat"></a><span data-ttu-id="1b6cf-102">解决团队聊天中的 "未知用户" 问题</span><span class="sxs-lookup"><span data-stu-id="1b6cf-102">Resolving issue with "Unknown User" in Teams Chat</span></span>

<span data-ttu-id="1b6cf-103">有时，已删除的用户将显示为 "未知用户"。</span><span class="sxs-lookup"><span data-stu-id="1b6cf-103">At times, a removed user will appear as "Unknown User".</span></span> <span data-ttu-id="1b6cf-104">这是一个 [已知问题](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/removed-user-appears-as-unknown)。</span><span class="sxs-lookup"><span data-stu-id="1b6cf-104">This is a [known issue](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/removed-user-appears-as-unknown).</span></span>

<span data-ttu-id="1b6cf-105">如果您永久看到在团队聊天中显示为 "未知用户" 的用户，请尝试清除缓存：</span><span class="sxs-lookup"><span data-stu-id="1b6cf-105">If you are persistently seeing users showing as "Unknown User" in Teams chats, try and clear the cache:</span></span>

1.  <span data-ttu-id="1b6cf-106">右键单击任务栏中的 "团队" 图标。</span><span class="sxs-lookup"><span data-stu-id="1b6cf-106">Right-click the Teams icon in the taskbar.</span></span> <span data-ttu-id="1b6cf-107">单击 "  **退出** "。</span><span class="sxs-lookup"><span data-stu-id="1b6cf-107">Click  **Quit** .</span></span>
2.  <span data-ttu-id="1b6cf-108">浏览到计算机上的 %appdata%\Microsoft\teams\ 文件夹，然后删除该目录中的所有文件。</span><span class="sxs-lookup"><span data-stu-id="1b6cf-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>

<span data-ttu-id="1b6cf-109">您可以通过确保匿名用户在大厅中等待，来阻止这些用户加入会议。</span><span class="sxs-lookup"><span data-stu-id="1b6cf-109">You can prevent anonymous users from joining meetings by ensuring that they wait in the lobby.</span></span> <span data-ttu-id="1b6cf-110">有关详细信息，请参阅 [更改团队会议的参与者设置](https://support.microsoft.com/office/change-participant-settings-for-a-teams-meeting-53261366-dbd5-45f9-aae9-a70e6354f88e)。</span><span class="sxs-lookup"><span data-stu-id="1b6cf-110">For more information, see [Change participant settings for a Teams meeting](https://support.microsoft.com/office/change-participant-settings-for-a-teams-meeting-53261366-dbd5-45f9-aae9-a70e6354f88e).</span></span>
