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
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696912"
---
# <a name="11-call-recording"></a><span data-ttu-id="a516c-102">1：1 呼叫录制</span><span class="sxs-lookup"><span data-stu-id="a516c-102">1:1 call recording</span></span>

<span data-ttu-id="a516c-103">如果在 **一** 对一呼叫中"开始录制"按钮灰显，则需要更改受影响用户的策略设置。</span><span class="sxs-lookup"><span data-stu-id="a516c-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span>   

<span data-ttu-id="a516c-104">从 2021 年 5 月 31 开始，我们将开始强制使用新的 Teams调用策略 *AllowCloudRecordingForCalls*。</span><span class="sxs-lookup"><span data-stu-id="a516c-104">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="a516c-105">在此更改之前，1：1 呼叫录制由 *AllowCloudRecording* 会议策略Teams控制。</span><span class="sxs-lookup"><span data-stu-id="a516c-105">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="a516c-106">此更改记录在消息中心文章： (更新)  [ 1：1 呼叫录制策略简介中](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)。</span><span class="sxs-lookup"><span data-stu-id="a516c-106">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="a516c-107">*AllowCloudRecordingForCalls*  默认情况下，呼叫策略选项 **$False** 策略选项。</span><span class="sxs-lookup"><span data-stu-id="a516c-107">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="a516c-108">如果你希望阻止所有用户录制一对一呼叫，则无需执行任何操作。</span><span class="sxs-lookup"><span data-stu-id="a516c-108">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="a516c-109">若要在 1：1 呼叫中为所有用户启用呼叫记录，Teams PowerShell 运行以下 cmdlet：</span><span class="sxs-lookup"><span data-stu-id="a516c-109">To enable call recording for all users in 1:1 calls use Teams PowerShell to run the following cmdlet:</span></span> 

<span data-ttu-id="a516c-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="a516c-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="a516c-111">或者，你可以创建新策略，并将 **-AllowCloudRecordingForCalls** 设置为 $true **并将该** 策略分配给你的用户。</span><span class="sxs-lookup"><span data-stu-id="a516c-111">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="a516c-112">有关详细信息，请参阅 ["1：1 呼叫录制策略控件 (几乎！) 此处](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)。</span><span class="sxs-lookup"><span data-stu-id="a516c-112">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
