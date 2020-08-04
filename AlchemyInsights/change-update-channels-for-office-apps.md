---
title: 更改适用于 Office 的更新通道
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 4939682a6ca95c4f5475ee6aedea48c9ce83df7f
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431368"
---
# <a name="change-update-channels-for-office-apps"></a><span data-ttu-id="946e0-102">更改适用于 Office 的更新通道</span><span class="sxs-lookup"><span data-stu-id="946e0-102">Change update channels for Office apps</span></span>

<span data-ttu-id="946e0-103">对于全新的 Office 安装，请使用 Office 软件下载设置选择所需的更新通道，然后安装（或重新安装） Office 应用。</span><span class="sxs-lookup"><span data-stu-id="946e0-103">For new Office installations, use Office Software Download Settings to select the desired update channel, and then install (or re-install) Office apps.</span></span> <span data-ttu-id="946e0-104">有关更多信息，请参阅[在 Office 365 中管理软件下载设置](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365)。</span><span class="sxs-lookup"><span data-stu-id="946e0-104">For more info, see [Manage software download settings in Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365).</span></span> 

<span data-ttu-id="946e0-105">**注意** 使用 Office 软件下载设置选择的更新通道适用于使用 O365 门户执行新安装的所有用户。</span><span class="sxs-lookup"><span data-stu-id="946e0-105">**Note** The update channel selected using the Office Software Download Settings applies to all users performing new installations using the O365 portal.</span></span> <span data-ttu-id="946e0-106">有关详细信息，请参阅[在电脑或 Mac 上下载并安装或重新安装 Microsoft 365 或 Office 2019](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658)。</span><span class="sxs-lookup"><span data-stu-id="946e0-106">For more info, see [Download and install or reinstall Microsoft 365 or Office 2019 on a PC or Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).</span></span>   

<span data-ttu-id="946e0-107">对于现有 Office 安装，请使用 Office 部署工具（ODT）切换到其他更新通道：</span><span class="sxs-lookup"><span data-stu-id="946e0-107">For existing Office installations, use the Office Deployment Tool (ODT) to switch to a different update channel:</span></span>  

1. <span data-ttu-id="946e0-108">从 [Microsoft下载中心](https://go.microsoft.com/fwlink/p/?LinkID=626065)下载最新版本的 Office 部署工具（setup.exe）。</span><span class="sxs-lookup"><span data-stu-id="946e0-108">Download the latest version of the Office Deployment Tool (setup.exe) from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
2. <span data-ttu-id="946e0-109">标识要切换到的频道名称。</span><span class="sxs-lookup"><span data-stu-id="946e0-109">Identify the name of the channel that you want to switch to.</span></span> <span data-ttu-id="946e0-110">有关详细信息，请参阅 [Office 部署工具的配置选项](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element)。</span><span class="sxs-lookup"><span data-stu-id="946e0-110">For more info, see [Configuration options for the Office Deployment Tool](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).</span></span>
3. <span data-ttu-id="946e0-111">创建一个配置XML文件，指定适当的通道名称，例如 update.xml。</span><span class="sxs-lookup"><span data-stu-id="946e0-111">Create a configuration XML file specifying the appropriate channel name, for example, update.xml.</span></span>  
    <span data-ttu-id="946e0-112">a.</span><span class="sxs-lookup"><span data-stu-id="946e0-112">a.</span></span> <Configuration>  
    <span data-ttu-id="946e0-113">b.</span><span class="sxs-lookup"><span data-stu-id="946e0-113">b.</span></span> <span data-ttu-id="946e0-114"><更新 **通道="每月"** /></span><span class="sxs-lookup"><span data-stu-id="946e0-114"><Updates **Channel="Monthly"** /></span></span>  
    <span data-ttu-id="946e0-115">c.</span><span class="sxs-lookup"><span data-stu-id="946e0-115">c.</span></span> </Configuration>
4. <span data-ttu-id="946e0-116">从提升的命令提示符处，切换到 setup.exe 所在的文件夹位置并运行以下命令：</span><span class="sxs-lookup"><span data-stu-id="946e0-116">From an elevated command prompt, switch to the folder location where setup.exe resides and run the following command:</span></span>  
    <span data-ttu-id="946e0-117">a.</span><span class="sxs-lookup"><span data-stu-id="946e0-117">a.</span></span> <span data-ttu-id="946e0-118">setup.exe /configure update.xml</span><span class="sxs-lookup"><span data-stu-id="946e0-118">setup.exe /configure update.xml</span></span>
5. <span data-ttu-id="946e0-119">启动 Office 应用程序（例如 Excel ），然后选择“**文件**” > “**帐户**”。</span><span class="sxs-lookup"><span data-stu-id="946e0-119">Start an Office application (such as Excel), and then select **File** > **Account**.</span></span> <span data-ttu-id="946e0-120">在“产品信息”部分中，选择“**更新选项**” > “**立即更新**”。</span><span class="sxs-lookup"><span data-stu-id="946e0-120">In the Product Information section, select **Update Options** > **Update Now**.</span></span>

<span data-ttu-id="946e0-121">有关更多信息，请参阅[如何切换现有 Office 应用的更新通道](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel)。</span><span class="sxs-lookup"><span data-stu-id="946e0-121">For more information, see [How to switch update channels for existing Office Apps](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel).</span></span> 

<span data-ttu-id="946e0-122">若要切换所选用户组的更新通道或使用配置管理器（SCCM），请使用 GPO 配置更新通道设置。</span><span class="sxs-lookup"><span data-stu-id="946e0-122">For switching update channels for a selected group of users or by using Configuration Manager (SCCM), configure the Update Channel setting using GPO.</span></span> <span data-ttu-id="946e0-123">有关详细信息，请参阅 [Microsoft 365 应用版的更新频道概述](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy)。</span><span class="sxs-lookup"><span data-stu-id="946e0-123">For more info, see [Overview of update channels for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy).</span></span> <span data-ttu-id="946e0-124">有关详细信息，请参阅[如何管理适用于 IT专业人员的 Office 365 ProPlus 通道](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813)和[使用 Microsoft Endpoint Configuration Manager 管理 Microsoft 365 应用版更新](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager)。</span><span class="sxs-lookup"><span data-stu-id="946e0-124">For details, see [How to manage Office 365 ProPlus Channels for IT Pros](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) and [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).</span></span>