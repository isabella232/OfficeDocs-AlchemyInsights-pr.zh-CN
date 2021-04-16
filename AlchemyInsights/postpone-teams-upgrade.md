---
title: 推迟 Teams 升级
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
- "2737"
- "4000006"
ms.openlocfilehash: abbf696b1554743bda188704272bfd85fe6f94e2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51801221"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="2d9b4-102">如何推迟 Microsoft 推动的 Teams 升级</span><span class="sxs-lookup"><span data-stu-id="2d9b4-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="2d9b4-103">**重要** 提示：我们可以帮助你使用支持诊断修复此问题，但看起来你未使用新管理中心。</span><span class="sxs-lookup"><span data-stu-id="2d9b4-103">**Important**: We can help fix this for you using a support diagnostic, but it looks like you are not using the New Admin Center.</span></span> <span data-ttu-id="2d9b4-104">若要使用"新建管理中心"，请从右上方滑动切换，右上方显示" **新建管理** 中心"。</span><span class="sxs-lookup"><span data-stu-id="2d9b4-104">To use the New Admin Center, slide the toggle in the top right that says **new admin center** to the right.</span></span> <span data-ttu-id="2d9b4-105">使用"新建管理中心"，单击" **需要帮助** ？"小组件，键入"推迟 Teams 升级"，然后按照提示运行诊断。</span><span class="sxs-lookup"><span data-stu-id="2d9b4-105">Using the New Admin Center, click the **Need Help?** widget, type "Postpone Teams Upgrade", then follow the prompts to run the diagnostic.</span></span>

<span data-ttu-id="2d9b4-106">如果你收到有关从 Skype for Business 到 Microsoft Teams 的 Microsoft 驱动自动升级的通信，并且你希望将自动升级推迟至以后日期，则全局管理员可以登录到[Teams](https://admin.teams.microsoft.com/dashboard)管理门户，在选择Microsoft Teams 升级下的"刷新状态"按钮后，选择"推迟"按钮。</span><span class="sxs-lookup"><span data-stu-id="2d9b4-106">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and, after selecting the **Refresh Status** button under Microsoft Teams Upgrade, select the **Postpone** button.</span></span> <span data-ttu-id="2d9b4-107">若要查看租户自动升级到 Microsoft Teams 的新日期，请刷新 Teams 管理门户页面。</span><span class="sxs-lookup"><span data-stu-id="2d9b4-107">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="2d9b4-108">**注意：** 只有 **收到** 有关自动升级的消息中心通知时，"推迟"按钮才可用。</span><span class="sxs-lookup"><span data-stu-id="2d9b4-108">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="2d9b4-109">全局管理员还可以运行 [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) 来了解有关其当前升级状态的信息。</span><span class="sxs-lookup"><span data-stu-id="2d9b4-109">Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span>
