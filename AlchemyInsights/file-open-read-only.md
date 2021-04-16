---
title: 文件打开只读
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813174"
---
# <a name="file-open-read-only"></a><span data-ttu-id="38764-102">文件打开只读</span><span class="sxs-lookup"><span data-stu-id="38764-102">File open read-only</span></span>

<span data-ttu-id="38764-103">你可能会发现，打开文件时，文件以只读状态打开。</span><span class="sxs-lookup"><span data-stu-id="38764-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="38764-104">在某些情况下，这是为了增加安全性，例如当你从 Internet 打开文件时，其他时候，可能是由于可更改的设置。</span><span class="sxs-lookup"><span data-stu-id="38764-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="38764-105">下面是一些以只读打开文件的情况，以及您可以采取一些步骤来更改这一点。</span><span class="sxs-lookup"><span data-stu-id="38764-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="38764-106">**我的防病毒导致他们打开只读**</span><span class="sxs-lookup"><span data-stu-id="38764-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="38764-107">某些防病毒程序可能会通过以只读的方式打开它们来保护你免受可能不安全的文件危害。</span><span class="sxs-lookup"><span data-stu-id="38764-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="38764-108">您可能需要与防病毒提供商联系，以了解如何调整这些设置。</span><span class="sxs-lookup"><span data-stu-id="38764-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="38764-109">例如，BitDefender 包含有关在此处添加应用程序排除项的内容： [如何在 Bitdefender 控制中心中添加应用程序或进程排除项](https://aka.ms/AA6098i)。</span><span class="sxs-lookup"><span data-stu-id="38764-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="38764-110">**文件属性是否设置为只读？**</span><span class="sxs-lookup"><span data-stu-id="38764-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="38764-111">可以通过右键单击文件并选择"属性"来检查文件属性。</span><span class="sxs-lookup"><span data-stu-id="38764-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="38764-112">如果选中只读属性，可以取消选中它，然后单击确定。</span><span class="sxs-lookup"><span data-stu-id="38764-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="38764-113">**内容位于受保护的视图中**</span><span class="sxs-lookup"><span data-stu-id="38764-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="38764-114">来自 Internet 和其他可能不安全的位置的文件可能包含病毒、蠕虫或其他可能损害计算机的恶意软件。</span><span class="sxs-lookup"><span data-stu-id="38764-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="38764-115">这通常也是你下载的电子邮件附件或文件的情况。</span><span class="sxs-lookup"><span data-stu-id="38764-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="38764-116">为了帮助保护计算机，这些可能不安全的位置中的文件在受保护的视图中打开。</span><span class="sxs-lookup"><span data-stu-id="38764-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="38764-117">通过使用受保护的视图，您可以读取文件并查看其内容，同时降低风险。</span><span class="sxs-lookup"><span data-stu-id="38764-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="38764-118">有关受保护的视图以及如何更改设置的信息，请参阅本文： [什么是受保护的视图？](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="38764-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="38764-119">**OneDrive 是否已满？**</span><span class="sxs-lookup"><span data-stu-id="38764-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="38764-120">如果文件存储在 OneDrive 上且 OneDrive 存储空间已满，那么在分配的空间不足之前，无法保存文档。</span><span class="sxs-lookup"><span data-stu-id="38764-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="38764-121">可以通过单击通知中心中的 OneDrive 图标并选择"管理存储"来检查 OneDrive 上的可用空间，也可以转到 、登录并记下屏幕左下角的已用空间 [https://onedrive.live.com](https://onedrive.live.com) 量。</span><span class="sxs-lookup"><span data-stu-id="38764-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="38764-122">**Office 是否激活？**</span><span class="sxs-lookup"><span data-stu-id="38764-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="38764-123">如果未激活 Office，或者你的订阅已过期，则你可能处于只读的缩减功能模式。</span><span class="sxs-lookup"><span data-stu-id="38764-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="38764-124">若要了解如何激活 Office，请参阅：Office 中的未授权产品和 [激活错误](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)。</span><span class="sxs-lookup"><span data-stu-id="38764-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="38764-125">**如果所有其他失败...**</span><span class="sxs-lookup"><span data-stu-id="38764-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="38764-126">尝试重新启动计算机</span><span class="sxs-lookup"><span data-stu-id="38764-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="38764-127">安装 Office 更新</span><span class="sxs-lookup"><span data-stu-id="38764-127">Install Office updates</span></span>
    
- <span data-ttu-id="38764-128">执行 Office 的联机修复</span><span class="sxs-lookup"><span data-stu-id="38764-128">Perform an Online repair of Office</span></span>
    

