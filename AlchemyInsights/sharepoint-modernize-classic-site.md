---
title: 新式网站作为根网站
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid:
- "9000153"
- "1692"
ms.openlocfilehash: 6f55f1c63551027cc5522d296cb3f3f342356d95
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2019
ms.locfileid: "36576656"
---
# <a name="modernize-your-classic-sharepoint-site"></a><span data-ttu-id="05533-102">现代化您的经典 SharePoint 网站</span><span class="sxs-lookup"><span data-stu-id="05533-102">Modernize your classic SharePoint site</span></span>

<span data-ttu-id="05533-103">如需切换到新式用户界面，需要完成以下操作：</span><span class="sxs-lookup"><span data-stu-id="05533-103">To make the switch to a modern user interface, you need to focus on the following:</span></span>

- <span data-ttu-id="05533-104">将**列表和库**转换为使用新式用户界面（也称为新式列表和库体验）。</span><span class="sxs-lookup"><span data-stu-id="05533-104">Transitioning your **lists and libraries** to use the modern user interface (also referred to as the modern list and library experience).</span></span>
- <span data-ttu-id="05533-105">将您的**网站页面**从经典 wiki 和 web 部件页转换为新式客户端页面。</span><span class="sxs-lookup"><span data-stu-id="05533-105">Transforming your **site pages** from classic wiki and web part pages into modern client-side pages.</span></span>
- <span data-ttu-id="05533-106">创建**新式网站**（工作组网站或通信网站）。</span><span class="sxs-lookup"><span data-stu-id="05533-106">Creating **modern sites** (Team site or Communication Site).</span></span>

<span data-ttu-id="05533-107">通过以下方式现代化化你的体验：</span><span class="sxs-lookup"><span data-stu-id="05533-107">Modernize your experience by:</span></span>
- <span data-ttu-id="05533-108">[使用新式用户界面显示列表和库](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries)，这可通过替换自定义、从使用的视图中删除不兼容的列，或（最后一招）将数据移到与新式用户界面兼容的列表类型来实现。</span><span class="sxs-lookup"><span data-stu-id="05533-108">[Enabling lists and libraries to show in the modern user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries) by replacing customizations, removing incompatible columns from the used views, or (as a last resort) moving data into a modern user interface-compatible list type.</span></span>
- <span data-ttu-id="05533-109">将[网站连接到 Office 365 组](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group)，这将为网站提供新式主页，并允许网站使用，例如，邮箱或 Microsoft Planner。</span><span class="sxs-lookup"><span data-stu-id="05533-109">[Connecting your site to an Office 365 group](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group), which gives your site a modern home page and enables your site to use, for example, a mailbox or Microsoft Planner.</span></span> <span data-ttu-id="05533-110">这使您可以使用 "日历" 和 "任务列表" 的新式版本。</span><span class="sxs-lookup"><span data-stu-id="05533-110">This enables you to use a modern version of a calendar and task list.</span></span>
- <span data-ttu-id="05533-111">[创建新式页面](https://support.office.com/article/create-and-use-modern-pages-on-a-sharepoint-site-b3d46deb-27a6-4b1e-87b8-df851e503dec)是使用图像、Excel、Word 和 PowerPoint 文档、视频等共享想法的绝佳方式。</span><span class="sxs-lookup"><span data-stu-id="05533-111">[Creating modern pages](https://support.office.com/article/create-and-use-modern-pages-on-a-sharepoint-site-b3d46deb-27a6-4b1e-87b8-df851e503dec), is a great way to share ideas using images, Excel, Word and PowerPoint documents, video, and more.</span></span>
- <span data-ttu-id="05533-112">[创建新式客户端页面](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-site-pages)，并将其配置为与关键经典 Wiki 页面和 Web 部件页“相似”。</span><span class="sxs-lookup"><span data-stu-id="05533-112">[Creating modern client-side pages](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-site-pages) and configuring these to be "similar" to your key classic wiki and web part pages.</span></span> <span data-ttu-id="05533-113">应对网站的关键页面执行编程页面转换，因为转换所有页面会占用大量资源，并且通常不需要。</span><span class="sxs-lookup"><span data-stu-id="05533-113">Programmatic page transformation should be done for the key pages of your sites, as transforming all pages is resource-intensive and often not needed.</span></span> <span data-ttu-id="05533-114">为了帮助进行此分类，SharePoint 新式化扫描程序会提供当前 Wiki 页面和 Web 部件页的使用情况信息。</span><span class="sxs-lookup"><span data-stu-id="05533-114">To assist in this triage, the SharePoint Modernization scanner can give you usage information about the current wiki and web part pages.</span></span>
- <span data-ttu-id="05533-115">[创建新式网站](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d)。</span><span class="sxs-lookup"><span data-stu-id="05533-115">[Creating modern sites](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span> <span data-ttu-id="05533-116">应该创建团队网站还是应该创建通信网站？</span><span class="sxs-lookup"><span data-stu-id="05533-116">Should I create a team site or a communication site?</span></span>

<span data-ttu-id="05533-117">其他信息：</span><span class="sxs-lookup"><span data-stu-id="05533-117">Additional Info:</span></span> 
- <span data-ttu-id="05533-118">有关将经典 SharePoint 网站新式化到新式体验的分步概述，请参阅[现代化您的经典 Sharepoint 网站](https://docs.microsoft.com/sharepoint/dev/transform/modernize-classic-sites)。</span><span class="sxs-lookup"><span data-stu-id="05533-118">For a step-by-step overview of modernizing your classic SharePoint Sites to the modern experience, see [Modernize your classic SharePoint Sites](https://docs.microsoft.com/sharepoint/dev/transform/modernize-classic-sites).</span></span>
- <span data-ttu-id="05533-119">请参阅[新式体验](https://docs.microsoft.com/sharepoint/guide-to-sharepoint-modern-experience)指南。</span><span class="sxs-lookup"><span data-stu-id="05533-119">See a guide to [Modern Experience](https://docs.microsoft.com/sharepoint/guide-to-sharepoint-modern-experience).</span></span>
- <span data-ttu-id="05533-120">请参阅[SharePoint 经典和新式体验](https://support.office.com/article/sharepoint-classic-and-modern-experiences-5725c103-505d-4a6e-9350-300d3ec7d73f)。</span><span class="sxs-lookup"><span data-stu-id="05533-120">See [SharePoint Classic and Modern experiences](https://support.office.com/article/sharepoint-classic-and-modern-experiences-5725c103-505d-4a6e-9350-300d3ec7d73f).</span></span> 




