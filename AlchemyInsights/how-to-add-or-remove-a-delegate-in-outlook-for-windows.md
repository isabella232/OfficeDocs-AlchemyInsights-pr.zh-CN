---
title: 如何在 Outlook for Windows 中添加或删除代理
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
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571800"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a><span data-ttu-id="73769-102">如何在 Outlook for Windows 中添加或删除代理</span><span class="sxs-lookup"><span data-stu-id="73769-102">How to add or remove a Delegate in Outlook for Windows</span></span>

<span data-ttu-id="73769-103">若要在 Outlook for Windows 中添加委派，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="73769-103">To add a Delegate in Outlook for Windows:</span></span> 

1. <span data-ttu-id="73769-104">单击 " **文件** " 选项卡，然后单击 " **帐户设置**"，然后选择 " **委派访问权限**"。</span><span class="sxs-lookup"><span data-stu-id="73769-104">Click on the **File** tab followed by **Account Settings**, and then choose **Delegate Access**.</span></span>
2. <span data-ttu-id="73769-105">单击 " **添加**"。</span><span class="sxs-lookup"><span data-stu-id="73769-105">Click on **Add**.</span></span> <span data-ttu-id="73769-106">如果未显示 " **添加** "，则 Outlook 和 Exchange 之间可能不存在活动连接。</span><span class="sxs-lookup"><span data-stu-id="73769-106">If **Add** doesn’t appear, an active connection might not exist between Outlook and Exchange.</span></span> <span data-ttu-id="73769-107">Outlook 状态栏显示连接状态。</span><span class="sxs-lookup"><span data-stu-id="73769-107">The Outlook status bar displays the connection status.</span></span>
3. <span data-ttu-id="73769-108">键入要指定为代理的人员的姓名，或在搜索结果列表中搜索并选择名称。</span><span class="sxs-lookup"><span data-stu-id="73769-108">Type the name of the person you want to designate as your delegate, or search and choose the name in the search results list.</span></span>

    > [!NOTE]
    > <span data-ttu-id="73769-109">代理必须是组织的 Exchange 全局地址列表中 (GAL) 的人员。</span><span class="sxs-lookup"><span data-stu-id="73769-109">The delegate must be a person in your organization's Exchange Global Address List (GAL).</span></span>
4. <span data-ttu-id="73769-110">单击 " **添加** "，然后单击 **"确定"**。</span><span class="sxs-lookup"><span data-stu-id="73769-110">Click on **Add** followed by **OK**.</span></span>
5. <span data-ttu-id="73769-111">在 " **代理权限** " 对话框中，接受默认权限设置或选择 "Exchange 文件夹的自定义访问级别"。</span><span class="sxs-lookup"><span data-stu-id="73769-111">In the **Delegate Permissions** dialog box, accept the default permission settings or select custom access levels for Exchange folders.</span></span>

    - <span data-ttu-id="73769-112">如果代理需要仅处理会议请求和响应的权限，则默认权限设置（如代理）将 **接收发送给我的与会议相关的邮件的副本** ，这是足够的。</span><span class="sxs-lookup"><span data-stu-id="73769-112">If a delegate needs permission to work only with meeting requests and responses, the default permission settings such as **Delegate receives copies of meeting-related messages sent to me** are sufficient.</span></span> <span data-ttu-id="73769-113">您可以将 **收件箱** 权限设置保留为 **无**。</span><span class="sxs-lookup"><span data-stu-id="73769-113">You can leave the **Inbox** permission setting at **None**.</span></span> <span data-ttu-id="73769-114">会议请求和响应将直接转到代理的 "收件箱"。</span><span class="sxs-lookup"><span data-stu-id="73769-114">Meeting requests and responses will go directly to the delegate's inbox.</span></span>

    > [!NOTE]
    > <span data-ttu-id="73769-115">默认情况下，授予代理 **(可以读取、创建和修改** 对 " **日历** " 文件夹的项目) 权限。</span><span class="sxs-lookup"><span data-stu-id="73769-115">By default, the delegate is granted **Editor (can read, create, and modify items)** permission to your **Calendar** folder.</span></span> <span data-ttu-id="73769-116">当代理代表您响应会议时，它会自动添加到 " **日历** " 文件夹中。</span><span class="sxs-lookup"><span data-stu-id="73769-116">When the delegate responds to a meeting on your behalf, it is automatically added to your **Calendar** folder.</span></span>

5. <span data-ttu-id="73769-117">若要发送邮件以通知代理已更改的权限，请选中 " **自动向代理发送邮件概述这些权限** " 复选框。</span><span class="sxs-lookup"><span data-stu-id="73769-117">To send a message to notify the delegate of the changed permissions, select the **Automatically send a message to delegate summarizing these permissions** check box.</span></span>
6. <span data-ttu-id="73769-118">如果需要，请选中 " **代理可以查看我的私人性质项目** " 复选框。</span><span class="sxs-lookup"><span data-stu-id="73769-118">If you want, select the **Delegate can see my private items** check box.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="73769-119">此设置会影响所有 Exchange 文件夹。</span><span class="sxs-lookup"><span data-stu-id="73769-119">This setting affects all Exchange folders.</span></span> <span data-ttu-id="73769-120">这包括所有邮件、联系人、日历、任务、便笺和日记文件夹。</span><span class="sxs-lookup"><span data-stu-id="73769-120">This includes all Mail, Contacts, Calendar, Tasks, Notes, and Journal folders.</span></span> <span data-ttu-id="73769-121">无法在仅指定的文件夹中授予对私人性质项目的访问权限。</span><span class="sxs-lookup"><span data-stu-id="73769-121">There is no way to grant access to private items in only specified folders.</span></span>

7. <span data-ttu-id="73769-122">选择“**确定**”。</span><span class="sxs-lookup"><span data-stu-id="73769-122">Choose **OK**.</span></span>

    > [!NOTE]
    >
    > - <span data-ttu-id="73769-123">使用 "代表发送" 权限发送的邮件在 " **发件人**" 旁边包含代理和您的姓名。</span><span class="sxs-lookup"><span data-stu-id="73769-123">Messages sent with Send on Behalf permissions include both the delegate's and your names next to **From**.</span></span> <span data-ttu-id="73769-124">使用 "代理发送" 权限发送邮件时，将只显示您的名称。</span><span class="sxs-lookup"><span data-stu-id="73769-124">When a message is sent with Send As permissions, only your name appears.</span></span>
    > - <span data-ttu-id="73769-125">一旦将某人添加为代理人，他们就可以将您的 Exchange 邮箱添加到其 Outlook 配置文件中。</span><span class="sxs-lookup"><span data-stu-id="73769-125">Once you add someone as a delegate, they can add your Exchange mailbox to their Outlook profile.</span></span> <span data-ttu-id="73769-126">有关说明，请参阅 [管理其他人的邮件和日历项目](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5)。</span><span class="sxs-lookup"><span data-stu-id="73769-126">For instructions, see [Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span></span>

<span data-ttu-id="73769-127">若要在 Outlook for Windows 中删除代理，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="73769-127">To remove a Delegate in Outlook for Windows:</span></span>

1. <span data-ttu-id="73769-128">单击 " **文件** " 选项卡。</span><span class="sxs-lookup"><span data-stu-id="73769-128">Click on the **File** tab.</span></span>
2. <span data-ttu-id="73769-129">单击 " **帐户设置** "，然后单击 " **代理访问**"。</span><span class="sxs-lookup"><span data-stu-id="73769-129">Click on **Account Settings** followed by **Delegate Access**.</span></span>
3. <span data-ttu-id="73769-130">选择要更改其权限的代理人的名称，然后单击 " **删除** " 后再单击 **"确定"**。</span><span class="sxs-lookup"><span data-stu-id="73769-130">Choose the name of the delegate for whom you want to change permissions, and then click on **Remove** followed by **OK**.</span></span>
