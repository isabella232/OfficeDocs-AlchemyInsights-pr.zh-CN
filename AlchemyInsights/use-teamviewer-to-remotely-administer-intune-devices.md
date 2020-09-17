---
title: 使用 TeamViewer 远程管理 Intune 设备
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: e931b2092ab049bc01c600344cbd4702848abcd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798438"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="eb348-102">使用 TeamViewer 远程管理 Intune 设备</span><span class="sxs-lookup"><span data-stu-id="eb348-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="eb348-103">可使用 [TeamViewer](https://www.teamviewer.com/) 远程管理由 Intune 管理的设备。</span><span class="sxs-lookup"><span data-stu-id="eb348-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="eb348-104">若要使用 TeamViewer 管理 Intune，请使用以下步骤：</span><span class="sxs-lookup"><span data-stu-id="eb348-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="eb348-105">首先从 TeamViewer 获取凭据，以在 Intune 上设置 TeamViewer 连接器。</span><span class="sxs-lookup"><span data-stu-id="eb348-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="eb348-106">这允许管理员在“设备”下的 TeamViewer 连接器用户界面中输入凭据，这是一项一次性操作，用于在 Intune 和 TeamViewer 服务之间建立关联。</span><span class="sxs-lookup"><span data-stu-id="eb348-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="eb348-107">**第 1 部分：使用远程设备启动会话**</span><span class="sxs-lookup"><span data-stu-id="eb348-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="eb348-108">在“**所有设备**”下，选择要用来启动远程会话的设备。</span><span class="sxs-lookup"><span data-stu-id="eb348-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="eb348-109">从 **…更多**中，选择“**新建远程协助会话**”。</span><span class="sxs-lookup"><span data-stu-id="eb348-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="eb348-110">选择“**是**”可确认你想要建立远程会话。</span><span class="sxs-lookup"><span data-stu-id="eb348-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="eb348-111">TeamViewer 服务确认“启动新远程会话”请求后，将在设备概述（或 Essentials）窗格的详细信息中看到“**启动远程协助**”选项。</span><span class="sxs-lookup"><span data-stu-id="eb348-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="eb348-112">选择“**查看更多**”以展开窗格并显示“远程协助”状态。</span><span class="sxs-lookup"><span data-stu-id="eb348-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="eb348-113">选择“**启动远程会话**”以在管理员端启动会话。</span><span class="sxs-lookup"><span data-stu-id="eb348-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="eb348-114">选择下载 TeamViewer 二进制文件（Windows），然后选择“**运行**”。</span><span class="sxs-lookup"><span data-stu-id="eb348-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="eb348-115">**注意**可以忽略打开到 TeamViewer 网站的任何 Web 浏览器页面。</span><span class="sxs-lookup"><span data-stu-id="eb348-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="eb348-116">确认对 TeamViewer 应用的请求，以便在设备上进行更改（仅限 Windows）。</span><span class="sxs-lookup"><span data-stu-id="eb348-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="eb348-117">TeamViewer 应用程序启动并包含用于验证与远程设备的连接的会话代码。</span><span class="sxs-lookup"><span data-stu-id="eb348-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="eb348-118">**第 2 部分：在面向远程会话的设备上**</span><span class="sxs-lookup"><span data-stu-id="eb348-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="eb348-119">打开 Intune 公司门户。</span><span class="sxs-lookup"><span data-stu-id="eb348-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="eb348-120">查找通知标志：“你的 IT 管理员正在请求控制此设备的远程协助会话”，然后选择通知。</span><span class="sxs-lookup"><span data-stu-id="eb348-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="eb348-121">选择下载 TeamViewer 应用程序，或者从 app store 中确认下载 TeamViewer 应用，然后选择“**运行**”。</span><span class="sxs-lookup"><span data-stu-id="eb348-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="eb348-122">**注意**可以忽略打开到 TeamViewer 网站的任何 Web 浏览器页面。</span><span class="sxs-lookup"><span data-stu-id="eb348-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="eb348-123">确认对 TeamViewer 应用的请求，以便在设备上进行更改（仅限 Windows）。</span><span class="sxs-lookup"><span data-stu-id="eb348-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="eb348-124">TeamViewer 应用程序启动并包含用于验证与远程设备的连接的会话代码。</span><span class="sxs-lookup"><span data-stu-id="eb348-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="eb348-125">弹出窗口询问是否要允许开始会话。</span><span class="sxs-lookup"><span data-stu-id="eb348-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="eb348-126">**注意**由 TeamViewer 服务生成的会话代码仅供一次性使用。</span><span class="sxs-lookup"><span data-stu-id="eb348-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="eb348-127">如果失去连接，则必须：</span><span class="sxs-lookup"><span data-stu-id="eb348-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="eb348-128">关闭远程设备和管理工作站上的 TeamViewer 应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="eb348-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="eb348-129">关闭远程设备上的公司门户。</span><span class="sxs-lookup"><span data-stu-id="eb348-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="eb348-130">从管理门户启动一个新的 "新建远程协助会话"。</span><span class="sxs-lookup"><span data-stu-id="eb348-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="eb348-131">重新打开远程设备上的公司门户以接收新的通知。</span><span class="sxs-lookup"><span data-stu-id="eb348-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="eb348-132">与以前一样，在远程设备和管理工作站上下载并打开 TeamViewer 应用程序。</span><span class="sxs-lookup"><span data-stu-id="eb348-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>