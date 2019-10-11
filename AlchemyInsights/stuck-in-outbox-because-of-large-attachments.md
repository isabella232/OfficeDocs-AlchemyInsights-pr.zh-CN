---
title: 由于大型附件导致发件箱中的卡
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441296"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="0f4f4-102">修复发件箱中卡住的邮件</span><span class="sxs-lookup"><span data-stu-id="0f4f4-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="0f4f4-103">我们建议您从[Microsoft 支持和恢复助手](https://diagnostics.office.com/#/)工具中运行["我遇到了问题发送、接收或查找电子邮件问题"](https://aka.ms/SaRA-OutlookSendReceive)这一方案开始。</span><span class="sxs-lookup"><span data-stu-id="0f4f4-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="0f4f4-104">当邮件滞留在发件箱中时，最可能的原因是：</span><span class="sxs-lookup"><span data-stu-id="0f4f4-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="0f4f4-105">大型附件。</span><span class="sxs-lookup"><span data-stu-id="0f4f4-105">Large attachments.</span></span>
- <span data-ttu-id="0f4f4-106">未启用 "**连接后立即发送**" 选项。</span><span class="sxs-lookup"><span data-stu-id="0f4f4-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="0f4f4-107">要删除大附件，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="0f4f4-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="0f4f4-108">在 Outlook 中，选择 "**发送/接收** > **脱机工作**"。</span><span class="sxs-lookup"><span data-stu-id="0f4f4-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="0f4f4-109">在导航窗格中，选择 **"发件箱"**。</span><span class="sxs-lookup"><span data-stu-id="0f4f4-109">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="0f4f4-110">在此处，您可以执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="0f4f4-110">From here, you can:</span></span> 
    - <span data-ttu-id="0f4f4-111">删除邮件（选择它，然后选择 "**删除**"）。</span><span class="sxs-lookup"><span data-stu-id="0f4f4-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="0f4f4-112">将邮件拖到 "草稿" 文件夹中，双击以打开它，然后删除附件，选择它，然后选择 "**删除**"。</span><span class="sxs-lookup"><span data-stu-id="0f4f4-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="0f4f4-113">如果收到指示 Outlook 尝试传输邮件的错误，请关闭 Outlook。</span><span class="sxs-lookup"><span data-stu-id="0f4f4-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="0f4f4-114">可能需要几分钟才能退出。</span><span class="sxs-lookup"><span data-stu-id="0f4f4-114">It may take a few moments to exit.</span></span> <span data-ttu-id="0f4f4-115">如果 Outlook 未关闭，请按 Ctrl + Alt + Delete，然后选择 "**启动任务管理器**"。</span><span class="sxs-lookup"><span data-stu-id="0f4f4-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="0f4f4-116">在任务管理器中，选择 "**进程**" 选项卡，向下滚动到 "setup.exe"，然后选择 "**结束进程**"。</span><span class="sxs-lookup"><span data-stu-id="0f4f4-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="0f4f4-117">Outlook 关闭后，重新启动它并重复步骤2和3。</span><span class="sxs-lookup"><span data-stu-id="0f4f4-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="0f4f4-118">删除附件后，请单击 "脱机**发送/接收** > **工作**" 以恢复联机工作。</span><span class="sxs-lookup"><span data-stu-id="0f4f4-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="0f4f4-119">当您单击 "**发送**"，但未连接时，邮件也会陷入发件箱中。</span><span class="sxs-lookup"><span data-stu-id="0f4f4-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="0f4f4-120">单击 "**发送/接收**" 并查看 "**脱机工作**" 按钮。</span><span class="sxs-lookup"><span data-stu-id="0f4f4-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="0f4f4-121">如果是蓝色，则断开连接。</span><span class="sxs-lookup"><span data-stu-id="0f4f4-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="0f4f4-122">选择它以进行连接（该按钮变为白色），然后单击 "**全部发送**"。</span><span class="sxs-lookup"><span data-stu-id="0f4f4-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="0f4f4-123">若要**在连接时立即启用 Send**：</span><span class="sxs-lookup"><span data-stu-id="0f4f4-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="0f4f4-124">选择 "**高级**" "**文件** > **选项** >  "。</span><span class="sxs-lookup"><span data-stu-id="0f4f4-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="0f4f4-125">在 "**发送和接收**" 部分，选择 "**连接后立即发送**"，然后选择 **"确定"**。</span><span class="sxs-lookup"><span data-stu-id="0f4f4-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="0f4f4-126">有关完整的详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="0f4f4-126">For full details see:</span></span>
- [<span data-ttu-id="0f4f4-127">视频：发送或删除卡住的电子邮件</span><span class="sxs-lookup"><span data-stu-id="0f4f4-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="0f4f4-128">在 Outlook 中手动启动发送/接收操作之前，电子邮件将一直保留在 "发件箱" 文件夹中</span><span class="sxs-lookup"><span data-stu-id="0f4f4-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
