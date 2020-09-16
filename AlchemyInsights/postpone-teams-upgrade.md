---
title: 推迟团队升级
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2737"
- "4000006"
ms.openlocfilehash: ae0611df247790200d0192e018ff5f0128f23cb4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741761"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="2ad5c-102">如何推迟 Microsoft 驱动的团队升级</span><span class="sxs-lookup"><span data-stu-id="2ad5c-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="2ad5c-103">**重要说明**：我们可以使用支持诊断为你提供帮助，但看起来你没有使用新的管理中心。</span><span class="sxs-lookup"><span data-stu-id="2ad5c-103">**Important**: We can help fix this for you using a support diagnostic, but it looks like you are not using the New Admin Center.</span></span> <span data-ttu-id="2ad5c-104">若要使用新管理中心，请在右上部向右滑动新的 " **管理中心** " 的开关。</span><span class="sxs-lookup"><span data-stu-id="2ad5c-104">To use the New Admin Center, slide the toggle in the top right that says **new admin center** to the right.</span></span> <span data-ttu-id="2ad5c-105">使用新管理中心，单击 " **需要帮助？** " 小部件，键入 "推迟团队升级"，然后按照提示运行诊断。</span><span class="sxs-lookup"><span data-stu-id="2ad5c-105">Using the New Admin Center, click the **Need Help?** widget, type "Postpone Teams Upgrade", then follow the prompts to run the diagnostic.</span></span>

<span data-ttu-id="2ad5c-106">如果你收到了有关从 Skype for Business 到 Microsoft 团队的 Microsoft 驱动的自动升级的通信，并且你希望将自动升级推迟到更晚的日期，全局管理员可以登录到 [团队管理门户](https://admin.teams.microsoft.com/dashboard) ，并在 "Microsoft 团队升级" 下选择 " **刷新状态** " 按钮后，选择 " **延迟** " 按钮。</span><span class="sxs-lookup"><span data-stu-id="2ad5c-106">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and, after selecting the **Refresh Status** button under Microsoft Teams Upgrade, select the **Postpone** button.</span></span> <span data-ttu-id="2ad5c-107">若要查看租户自动升级到 Microsoft 团队的新日期，请刷新 "团队管理门户" 页。</span><span class="sxs-lookup"><span data-stu-id="2ad5c-107">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="2ad5c-108">**注意：** 仅当您收到有关自动升级的消息中心通知时，" **延期** " 按钮才可用。</span><span class="sxs-lookup"><span data-stu-id="2ad5c-108">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="2ad5c-109">全局管理员还可以运行 [CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) 以了解有关其当前升级状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2ad5c-109">Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span>
