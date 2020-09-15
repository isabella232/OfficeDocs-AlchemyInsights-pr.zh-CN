---
title: Yammer 实时事件创建错误
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002495"
- "5112"
ms.openlocfilehash: 1b342b17e4b91804a75c46352f3ef7d7814bfcee
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47675432"
---
# <a name="live-events-in-yammer-creation-errors"></a><span data-ttu-id="40b2c-102">Yammer 实时事件创建错误</span><span class="sxs-lookup"><span data-stu-id="40b2c-102">Live events in Yammer creation errors</span></span>

<span data-ttu-id="40b2c-103">**创建 Yammer 实时事件**</span><span class="sxs-lookup"><span data-stu-id="40b2c-103">**Yammer Live Event creation**</span></span>

<span data-ttu-id="40b2c-104">Yammer 将始终显示创建实时事件的选项。</span><span class="sxs-lookup"><span data-stu-id="40b2c-104">Yammer will show the option to create a live event at all times.</span></span> <span data-ttu-id="40b2c-105">在某些情况下，用户可能不符合创建实时事件的先决条件，并会在尝试创建实时事件时收到错误。</span><span class="sxs-lookup"><span data-stu-id="40b2c-105">In some cases, a user may not meet the prerequisites for creating a live event and receive an error when they attempt to create it.</span></span> <span data-ttu-id="40b2c-106">下面各项介绍了此问题的常见原因，并为最终用户提供解决方法。</span><span class="sxs-lookup"><span data-stu-id="40b2c-106">The items below cover common reasons for this problem and provide ways to resolve it for end users.</span></span>

<span data-ttu-id="40b2c-107">**谁可以创建实时事件**</span><span class="sxs-lookup"><span data-stu-id="40b2c-107">**Who can create live events**</span></span>
- <span data-ttu-id="40b2c-108">Office 365 企业版 E1、E3 或 E5 许可证，或 Office 365 A3 或 A5 许可证。</span><span class="sxs-lookup"><span data-stu-id="40b2c-108">An Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license.</span></span>
- <span data-ttu-id="40b2c-109">在 Microsoft Teams 管理中心创建实时事件的权限。</span><span class="sxs-lookup"><span data-stu-id="40b2c-109">Permission to create live events in Microsoft Teams admin center.</span></span>
- <span data-ttu-id="40b2c-110">在 Microsoft Stream 中创建实时事件的权限（适用于使用外部广播应用或设备制作的事件）。</span><span class="sxs-lookup"><span data-stu-id="40b2c-110">Permission to create live events in Microsoft Stream (for events produced using an external broadcasting app or device).</span></span>
- <span data-ttu-id="40b2c-111">组织中的正式团队成员身份（不能是来宾或来自其他组织）。</span><span class="sxs-lookup"><span data-stu-id="40b2c-111">Full team membership in the org (can’t be a guest or from another org).</span></span>
- <span data-ttu-id="40b2c-112">私人会议计划、屏幕共享、IP 会议共享、已在 Team 会议策略中打开。</span><span class="sxs-lookup"><span data-stu-id="40b2c-112">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

<span data-ttu-id="40b2c-113">**创建实时事件策略**</span><span class="sxs-lookup"><span data-stu-id="40b2c-113">**Live event creation policies**</span></span>

<span data-ttu-id="40b2c-114">Yammer 遵循 Stream 的 Office 365 租户中设置的实时事件策略。</span><span class="sxs-lookup"><span data-stu-id="40b2c-114">Yammer follows the Live Event policies set in your Office 365 tenant for Stream.</span></span> <span data-ttu-id="40b2c-115">默认情况下，组织中的所有人均可创建实时事件。</span><span class="sxs-lookup"><span data-stu-id="40b2c-115">By default, everyone in your organization can create a live event.</span></span> <span data-ttu-id="40b2c-116">管理员可能会[对此设置进行更改，这可能会阻止用户创建实时事件](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating)。</span><span class="sxs-lookup"><span data-stu-id="40b2c-116">Administrators may [make changes to this setting which may prevent users from creating a live event](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span></span> <span data-ttu-id="40b2c-117">如果用户收到策略错误，请务必检查用户是否具有创建实时事件的权限。</span><span class="sxs-lookup"><span data-stu-id="40b2c-117">It is important to check that users have permissions to create live events if they receive a policy error.</span></span>
