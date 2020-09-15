---
title: 在 Yammer 中打开或下载文件时遇到问题
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
- "6041"
- "9003112"
ms.openlocfilehash: de335e27624caf5a91bdc2913570eba92f627282
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695639"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="aa9c0-102">在 Yammer 中打开或下载文件时遇到问题</span><span class="sxs-lookup"><span data-stu-id="aa9c0-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="aa9c0-103">经典 Yammer 支持将文件上传到消息和组的多个选项。</span><span class="sxs-lookup"><span data-stu-id="aa9c0-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="aa9c0-104">根据网络配置，文件默认存储在 SharePoint 中。</span><span class="sxs-lookup"><span data-stu-id="aa9c0-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="aa9c0-105">新版 Yammer 中的文件选取器尚无法支持经典 Yammer 中提供的所有选项。</span><span class="sxs-lookup"><span data-stu-id="aa9c0-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="aa9c0-106">未来的更新将会添加其他功能。</span><span class="sxs-lookup"><span data-stu-id="aa9c0-106">A future update will add additional features.</span></span> <span data-ttu-id="aa9c0-107">有关详细信息，请参阅[将文件或图像附加到 Yammer 对话帖子](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8)。</span><span class="sxs-lookup"><span data-stu-id="aa9c0-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="aa9c0-108">**无法打开或下载文件**</span><span class="sxs-lookup"><span data-stu-id="aa9c0-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="aa9c0-109">文件可能上传到 Yammer，但同时又链接到 SharePoint Online 中的文件。</span><span class="sxs-lookup"><span data-stu-id="aa9c0-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="aa9c0-110">若要解决此问题，首先必须确定文件的位置。</span><span class="sxs-lookup"><span data-stu-id="aa9c0-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="aa9c0-111">如果已将文件上传到 Yammer，则它将具有 \*.yammer.com URL。</span><span class="sxs-lookup"><span data-stu-id="aa9c0-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="aa9c0-112">确保已取消阻止所需 URL 和 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="aa9c0-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="aa9c0-113">有关详细信息，请参阅博客文章[不建议针对 Yammer 使用硬编码的 IP 地址](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592)。</span><span class="sxs-lookup"><span data-stu-id="aa9c0-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="aa9c0-114">检查某个也是全局管理员身份的用户是否可以下载该文件。</span><span class="sxs-lookup"><span data-stu-id="aa9c0-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="aa9c0-115">如果文件是专用的，则可能需要使用“专用内容模式”。</span><span class="sxs-lookup"><span data-stu-id="aa9c0-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="aa9c0-116">有关详细信息，请参 [监视 Yammer 中的专用内容](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content)。</span><span class="sxs-lookup"><span data-stu-id="aa9c0-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="aa9c0-117">**Yammer 网络级别的来宾和 SharePoint Online 中的文件**</span><span class="sxs-lookup"><span data-stu-id="aa9c0-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="aa9c0-118">[Yammer 中的网络级别来宾](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests)不使用 Azure AD B2B，并且只能在 Yammer 服务内部活动，因此不能访问存储在 SharePoint 中的 Yammer 文件。</span><span class="sxs-lookup"><span data-stu-id="aa9c0-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="aa9c0-119">请创建可使用 AAD B2B 标识访问 SharePoint Online 中的文档库的外部 AAD B2B 用户。</span><span class="sxs-lookup"><span data-stu-id="aa9c0-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="aa9c0-120">有关未来在 Yammer 中提供 Azure AD B2B 来宾支持的详细信息，请参阅[Yammer 预览版中的企业对企业 (B2B) 来宾支持 - 客户条款和常见问题解答](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer)。</span><span class="sxs-lookup"><span data-stu-id="aa9c0-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>