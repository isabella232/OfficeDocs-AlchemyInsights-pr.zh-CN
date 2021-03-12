---
title: 1：1 呼叫录制
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733839"
---
# <a name="11-call-recording"></a><span data-ttu-id="353ba-102">1：1 呼叫录制</span><span class="sxs-lookup"><span data-stu-id="353ba-102">1:1 call recording</span></span>

<span data-ttu-id="353ba-103">管理员现在需要采取措施以继续允许用户录制 1：1 呼叫。</span><span class="sxs-lookup"><span data-stu-id="353ba-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="353ba-104">从 2021 年 4 月 12 日起，我们将开始强制执行新的 Teams 通话策略选项 *AllowCloudRecordingForCalls*。</span><span class="sxs-lookup"><span data-stu-id="353ba-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="353ba-105">目前，1：1 呼叫录制功能由 Teams 会议策略中的 *AllowCloudRecording* 选项控制。</span><span class="sxs-lookup"><span data-stu-id="353ba-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="353ba-106">如果允许用户录制 Teams 会议，他们还可以录制一对一通话。</span><span class="sxs-lookup"><span data-stu-id="353ba-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="353ba-107">如果你希望阻止所有用户录制一对一呼叫，则无需执行任何操作。</span><span class="sxs-lookup"><span data-stu-id="353ba-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="353ba-108">*AllowCloudRecordingForCalls* 呼叫策略选项$False启用。</span><span class="sxs-lookup"><span data-stu-id="353ba-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="353ba-109">此更改记录在下列消息中心帖子中 [ ： (Updated) 1：1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use Teams [PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="353ba-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="353ba-110">**若要在 1：1** 呼叫中启用呼叫录制：Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="353ba-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="353ba-111">**若要在 1：1** 呼叫中禁用呼叫录制：Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span><span class="sxs-lookup"><span data-stu-id="353ba-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

