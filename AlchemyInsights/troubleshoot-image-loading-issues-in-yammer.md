---
title: 排查 Yammer 中的图像加载问题
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: cf330adbf3f3a92d4b90768c7dd8bada6333db80
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690233"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="429e9-102">排查 Yammer 中的图像加载问题</span><span class="sxs-lookup"><span data-stu-id="429e9-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="429e9-103">当 Yammer 中的照片和文件预览出现问题时，请检查是否所有用户都遇到此问题，它是否发生在移动设备上以及在上传附件时是否可再现，以便进行故障排除。</span><span class="sxs-lookup"><span data-stu-id="429e9-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="429e9-104">**个人资料照片问题**</span><span class="sxs-lookup"><span data-stu-id="429e9-104">**Profile photo issues**</span></span>  

<span data-ttu-id="429e9-105">如果最终用户通过 Microsoft 365 登录 Yammer，则必须更改其个人资料，包括个人资料照片。</span><span class="sxs-lookup"><span data-stu-id="429e9-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="429e9-106">如果不允许用户更新个人资料，则管理员可以为该用户执行更新。</span><span class="sxs-lookup"><span data-stu-id="429e9-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="429e9-107">有关详细信息，请参阅[在 Office Delve 中查看和更新个人资料](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba)。</span><span class="sxs-lookup"><span data-stu-id="429e9-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="429e9-108">有关个人资料编辑的信息（包括个人资料照片），请参阅[更改我的 Yammer 个人资料和设置](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851)。</span><span class="sxs-lookup"><span data-stu-id="429e9-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="429e9-109">更新的个人资料照片与个人资料属性的同步方式不同。</span><span class="sxs-lookup"><span data-stu-id="429e9-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="429e9-110">用户必须登录才能启动其个人资料照片的同步。</span><span class="sxs-lookup"><span data-stu-id="429e9-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="429e9-111">有关信息，请参阅[用户个人资料图片是否会从 Office 365 更新到 Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer)。</span><span class="sxs-lookup"><span data-stu-id="429e9-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="429e9-112">有关 Yammer 的用户生命周期的信息，请参阅[在 Yammer 用户的整个生命周期中通过 Office 365 对其进行管理](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle)。</span><span class="sxs-lookup"><span data-stu-id="429e9-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="429e9-113">有关个人资料图片同步在 Microsoft 365 中如何工作的详细信息，请参阅[有关 Microsoft 365 中的个人资料图片同步的信息](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a)。</span><span class="sxs-lookup"><span data-stu-id="429e9-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="429e9-114">**文档预览和图像缩略图问题**</span><span class="sxs-lookup"><span data-stu-id="429e9-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="429e9-115">将文件或图像发布到 Yammer 后，可能不会显示预览，原因如下：</span><span class="sxs-lookup"><span data-stu-id="429e9-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="429e9-116">文件已损坏，无法进行处理。</span><span class="sxs-lookup"><span data-stu-id="429e9-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="429e9-117">该文件最近尚未上传到 SharePoint Online，或者 Yammer 出于其他原因具有无效的元数据。</span><span class="sxs-lookup"><span data-stu-id="429e9-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="429e9-118">已阻止加载预览图像所需的 URL。</span><span class="sxs-lookup"><span data-stu-id="429e9-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="429e9-119">发布前，用户已删除文件预览。</span><span class="sxs-lookup"><span data-stu-id="429e9-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="429e9-120">服务问题已阻止生成预览。</span><span class="sxs-lookup"><span data-stu-id="429e9-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="429e9-121">**注意** 链接和文件上传的预览可能会有所不同。</span><span class="sxs-lookup"><span data-stu-id="429e9-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="429e9-122">指向 Internet 文件的链接或需要其他身份验证的链接可能无法正确显示。</span><span class="sxs-lookup"><span data-stu-id="429e9-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="429e9-123">有关详细信息，请参阅[将文件或图像附加到 Yammer 邮件](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf)。</span><span class="sxs-lookup"><span data-stu-id="429e9-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 