---
title: 文件以只读状态打开
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6a828f8d-ff31-40a7-b701-b2339e771817
ms.openlocfilehash: 4c774864a03b7dbc099f64b7906fa4a0bc26c63c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525713"
---
# <a name="file-open-read-only"></a><span data-ttu-id="8b02c-102">文件以只读状态打开</span><span class="sxs-lookup"><span data-stu-id="8b02c-102">File open read-only</span></span>

<span data-ttu-id="8b02c-103">您可能会发现, 打开文件时, 文件以只读方式打开。</span><span class="sxs-lookup"><span data-stu-id="8b02c-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="8b02c-104">在某些情况下, 这是为了提高安全性 (例如, 从 internet 打开文件时) 以及其他时间, 这可能是由于可以更改的设置所致。</span><span class="sxs-lookup"><span data-stu-id="8b02c-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="8b02c-105">以下是文件以只读的形式打开的一些方案, 以及可执行的更改步骤。</span><span class="sxs-lookup"><span data-stu-id="8b02c-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="8b02c-106">**我的防病毒导致其以只读方式打开**</span><span class="sxs-lookup"><span data-stu-id="8b02c-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="8b02c-107">某些防病毒程序可能会通过以只读方式打开这些文件来保护其免受潜在的安全。</span><span class="sxs-lookup"><span data-stu-id="8b02c-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="8b02c-108">您可能需要与防病毒提供商确认, 以了解如何调整这些设置。</span><span class="sxs-lookup"><span data-stu-id="8b02c-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="8b02c-109">例如, BitDefender 包含以下内容: 在此处添加应用程序排除:[如何在 BitDefender 控制中心添加应用程序或进程排除项](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl)。</span><span class="sxs-lookup"><span data-stu-id="8b02c-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span></span>
  
 <span data-ttu-id="8b02c-110">**文件属性是否设置为只读？**</span><span class="sxs-lookup"><span data-stu-id="8b02c-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="8b02c-111">您可以通过右键单击文件, 然后选择 "属性" 来检查文件属性。</span><span class="sxs-lookup"><span data-stu-id="8b02c-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="8b02c-112">如果已选中只读属性, 则可以取消选中它, 然后单击 "确定"。</span><span class="sxs-lookup"><span data-stu-id="8b02c-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="8b02c-113">**内容位于受保护的视图中**</span><span class="sxs-lookup"><span data-stu-id="8b02c-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="8b02c-114">来自 Internet 和来自其他潜在不安全位置的文件可能包含病毒、蠕虫或可能损害计算机的其他类型的恶意软件。</span><span class="sxs-lookup"><span data-stu-id="8b02c-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="8b02c-115">通常情况下, 您下载的电子邮件附件或文件也是如此。</span><span class="sxs-lookup"><span data-stu-id="8b02c-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="8b02c-116">为了帮助保护你的计算机, 可以在受保护的视图中打开来自这些潜在不安全位置的文件。</span><span class="sxs-lookup"><span data-stu-id="8b02c-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="8b02c-117">通过使用受保护的视图, 可以读取文件并在降低风险的同时查看其内容。</span><span class="sxs-lookup"><span data-stu-id="8b02c-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="8b02c-118">有关受保护的视图和更改设置的详细信息, 请参阅本文:[什么是受保护的视图？](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="8b02c-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="8b02c-119">**OneDrive 是否已满？**</span><span class="sxs-lookup"><span data-stu-id="8b02c-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="8b02c-120">如果文件存储在 OneDrive 上, 且你的 OneDrive 存储空间已满, 你将无法保存该文档, 直到你已被分配空间所下。</span><span class="sxs-lookup"><span data-stu-id="8b02c-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="8b02c-121">您可以通过单击通知中心中的 OneDrive 图标并选择 "管理存储" 来检查 OneDrive 上的可用空间, 也可以转[http://onedrive.live.com](http://onedrive.live.com)到 "登录", 并记下屏幕左下角的可用空间量。</span><span class="sxs-lookup"><span data-stu-id="8b02c-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="8b02c-122">**Office 是否已激活？**</span><span class="sxs-lookup"><span data-stu-id="8b02c-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="8b02c-123">如果未激活 Office, 或者订阅已过期, 则可以处于只读功能模式下。</span><span class="sxs-lookup"><span data-stu-id="8b02c-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="8b02c-124">有关如何激活 Office 的信息, 请参阅: [office 中的无许可证产品和激活错误](https://support.office.com/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380)。</span><span class="sxs-lookup"><span data-stu-id="8b02c-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="8b02c-125">**如果所有其他操作均失败 .。。**</span><span class="sxs-lookup"><span data-stu-id="8b02c-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="8b02c-126">尝试重新启动计算机</span><span class="sxs-lookup"><span data-stu-id="8b02c-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="8b02c-127">安装 Office 更新</span><span class="sxs-lookup"><span data-stu-id="8b02c-127">Install Office updates</span></span>
    
- <span data-ttu-id="8b02c-128">执行 Office 的联机修复</span><span class="sxs-lookup"><span data-stu-id="8b02c-128">Perform an Online repair of Office</span></span>
    

