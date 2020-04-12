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
- "9002385"
- "4645"
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232620"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="d6afe-102">修复发件箱中卡住的邮件</span><span class="sxs-lookup"><span data-stu-id="d6afe-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="d6afe-103">我们建议您从受影响的计算机上的[Microsoft 支持和恢复助手](https://diagnostics.office.com/#/)工具中运行["我遇到了问题，无法发送、接收或查找电子邮件"](https://aka.ms/SaRA-OutlookSendReceive)这一方案开始。</span><span class="sxs-lookup"><span data-stu-id="d6afe-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="d6afe-104">当邮件滞留在发件箱中时，最可能的原因是附件较大，或者 "连接后立即发送" 选项未启用。</span><span class="sxs-lookup"><span data-stu-id="d6afe-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="d6afe-105">**删除大附件**</span><span class="sxs-lookup"><span data-stu-id="d6afe-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="d6afe-106">单击 "**发送/接收** > **脱机工作**"。</span><span class="sxs-lookup"><span data-stu-id="d6afe-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="d6afe-107">在导航窗格中，单击 **"发件箱**"。</span><span class="sxs-lookup"><span data-stu-id="d6afe-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="d6afe-108">在此处，您可以执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="d6afe-108">From here, you can:</span></span> 
    - <span data-ttu-id="d6afe-109">删除邮件。</span><span class="sxs-lookup"><span data-stu-id="d6afe-109">Delete the message.</span></span> <span data-ttu-id="d6afe-110">只需选择它并单击 "**删除**"。</span><span class="sxs-lookup"><span data-stu-id="d6afe-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="d6afe-111">将邮件拖到 "**草稿" 文件夹**中，双击以打开该邮件，然后删除该附件（单击它并单击 "**删除**"）。</span><span class="sxs-lookup"><span data-stu-id="d6afe-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="d6afe-112">如果出现错误，则表明 Outlook 正在尝试传输邮件，请关闭 Outlook。</span><span class="sxs-lookup"><span data-stu-id="d6afe-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="d6afe-113">可能需要几分钟才能退出。</span><span class="sxs-lookup"><span data-stu-id="d6afe-113">It may take a few moments to exit.</span></span> <span data-ttu-id="d6afe-114">如果 Outlook 不关闭，请按**Ctrl + Alt + Delete** ，然后单击 "**启动任务管理器**"。</span><span class="sxs-lookup"><span data-stu-id="d6afe-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="d6afe-115">在任务管理器中，选择 "**进程**" 选项卡，向下滚动到 "setup.exe"，然后单击 "**结束进程**"。</span><span class="sxs-lookup"><span data-stu-id="d6afe-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="d6afe-116">Outlook 关闭后，重新启动 Outlook 并重复步骤2-3。</span><span class="sxs-lookup"><span data-stu-id="d6afe-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="d6afe-117">删除附件后，请单击 "脱机**发送/接收** > **工作**" 以取消选择该按钮，然后恢复联机工作。</span><span class="sxs-lookup"><span data-stu-id="d6afe-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="d6afe-118">当您单击 "**发送**"，但未连接时，邮件也会陷入发件箱中。</span><span class="sxs-lookup"><span data-stu-id="d6afe-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="d6afe-119">单击 "**发送/接收**" 并查看 "**脱机工作**" 按钮。</span><span class="sxs-lookup"><span data-stu-id="d6afe-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="d6afe-120">如果是蓝色，则断开连接。</span><span class="sxs-lookup"><span data-stu-id="d6afe-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="d6afe-121">单击以进行连接（该按钮变为白色），然后单击 "**全部发送**"。</span><span class="sxs-lookup"><span data-stu-id="d6afe-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="d6afe-122">**启用 "在连接时立即发送"**</span><span class="sxs-lookup"><span data-stu-id="d6afe-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="d6afe-123">在“文件”选项卡上，单击“选项”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="d6afe-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="d6afe-124">在 "Outlook 选项" 对话框中，单击 "**高级**"。</span><span class="sxs-lookup"><span data-stu-id="d6afe-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="d6afe-125">在 "发送和接收" 部分，单击以启用 "**连接后立即发送**"。</span><span class="sxs-lookup"><span data-stu-id="d6afe-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="d6afe-126">单击“**确定**”。</span><span class="sxs-lookup"><span data-stu-id="d6afe-126">Click **OK**.</span></span>
 
<span data-ttu-id="d6afe-127">有关完整的详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="d6afe-127">For full details, see:</span></span>
- [<span data-ttu-id="d6afe-128">视频：发送或删除卡住的电子邮件</span><span class="sxs-lookup"><span data-stu-id="d6afe-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="d6afe-129">在 Outlook 中手动启动发送/接收操作之前，电子邮件将一直保留在 "发件箱" 文件夹中</span><span class="sxs-lookup"><span data-stu-id="d6afe-129">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
