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
ms.openlocfilehash: 8cdadf34a059856338d7f40528446b70373465e4
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702080"
---
# <a name="11-call-recording"></a><span data-ttu-id="cab64-102">1：1 呼叫录制</span><span class="sxs-lookup"><span data-stu-id="cab64-102">1:1 call recording</span></span>

<span data-ttu-id="cab64-103">如果在 **一** 对一呼叫中"开始录制"按钮灰显，则需要更改受影响用户的策略设置。</span><span class="sxs-lookup"><span data-stu-id="cab64-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span> <span data-ttu-id="cab64-104">若要检查策略设置，请通过键入 **上面的 Diag： Teams 1：1 呼叫** 录制来为受到影响的用户运行诊断。</span><span class="sxs-lookup"><span data-stu-id="cab64-104">To check the policy setting, run the Diagnostic for the impacted user by typing **Diag: Teams 1:1 Call Recording** above.</span></span>     

<span data-ttu-id="cab64-105">从 2021 年 5 月 31 开始，我们将开始强制使用新的 Teams调用策略 *AllowCloudRecordingForCalls*。</span><span class="sxs-lookup"><span data-stu-id="cab64-105">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="cab64-106">在此更改之前，1：1 呼叫录制由 *AllowCloudRecording* 会议策略Teams控制。</span><span class="sxs-lookup"><span data-stu-id="cab64-106">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="cab64-107">此更改记录在消息中心文章： (更新)  [ 1：1 呼叫录制策略简介中](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)。</span><span class="sxs-lookup"><span data-stu-id="cab64-107">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="cab64-108">*AllowCloudRecordingForCalls*  默认情况下，呼叫策略选项 **$False** 策略选项。</span><span class="sxs-lookup"><span data-stu-id="cab64-108">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="cab64-109">如果你希望阻止所有用户录制一对一呼叫，则无需执行任何操作。</span><span class="sxs-lookup"><span data-stu-id="cab64-109">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="cab64-110">若要在一对一呼叫中为所有用户启用呼叫记录，Teams [PowerShell](/microsoftteams/teams-powershell-install)运行以下 cmdlet：</span><span class="sxs-lookup"><span data-stu-id="cab64-110">To enable call recording for all users in 1:1 calls use [Teams PowerShell](/microsoftteams/teams-powershell-install) to run the following cmdlet:</span></span> 

<span data-ttu-id="cab64-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="cab64-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="cab64-112">或者，你可以创建新策略，并将 **-AllowCloudRecordingForCalls** 设置为 $true **并将该** 策略分配给你的用户。</span><span class="sxs-lookup"><span data-stu-id="cab64-112">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="cab64-113">有关详细信息，请参阅 ["1：1 呼叫录制策略控件 (几乎！) 此处](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)。</span><span class="sxs-lookup"><span data-stu-id="cab64-113">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
