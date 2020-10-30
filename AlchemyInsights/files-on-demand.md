---
title: 文件随选
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
- "6432"
- "9003530"
ms.openlocfilehash: 4e3da81ee048c6257e05b998c0f457fa433738fd
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791284"
---
# <a name="configure-files-on-demand"></a><span data-ttu-id="047ce-102">配置文件随选</span><span class="sxs-lookup"><span data-stu-id="047ce-102">Configure Files On-Demand</span></span>

<span data-ttu-id="047ce-103">“文件随选”需要 [Windows 10 Fall Creators Update](https://go.microsoft.com/fwlink/p/?linkid=859040)（版本 1709 或更高版本）或 WIndows Server 2019 和 OneDrive 内部版本 17.3.7064.1005 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="047ce-103">OneDrive Files On-Demand requires [Windows 10 Fall Creators Update](https://go.microsoft.com/fwlink/p/?linkid=859040) (version 1709 or later) or Windows Server 2019 and OneDrive build 17.3.7064.1005 or later.</span></span>

<span data-ttu-id="047ce-104">OneDrive 文件随选可帮助访问 OneDrive 中的所有文件，而无需下载所有这些文件和使用设备上的存储空间。</span><span class="sxs-lookup"><span data-stu-id="047ce-104">OneDrive Files On-Demand helps you access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

<span data-ttu-id="047ce-105">要在电脑上配置文件随选，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="047ce-105">To configure Files On-Demand on your PC:</span></span>

1. <span data-ttu-id="047ce-106">选择Windows任务栏通知区域中的白色或蓝色 **OneDrive** 云图标。</span><span class="sxs-lookup"><span data-stu-id="047ce-106">Select the white or blue **OneDrive** cloud icon in the Windows taskbar notification area.</span></span> <span data-ttu-id="047ce-107">选择 **帮助 & "设置** 齿轮图标 > **设置s** 。</span><span class="sxs-lookup"><span data-stu-id="047ce-107">Select the **Help & Settings** gear icon > **Settings** .</span></span>
2. <span data-ttu-id="047ce-108">在“ **设置** ”选项卡上，选中“ **节省空间并在需要使用时下载文件** ”复选框。</span><span class="sxs-lookup"><span data-stu-id="047ce-108">On the **Settings** tab, select the **Save space and download files as you use them** box.</span></span>  

<span data-ttu-id="047ce-109">还可以使用注册表配置文件随选。</span><span class="sxs-lookup"><span data-stu-id="047ce-109">You can also configure Files On-Demand using the registry.</span></span>

<span data-ttu-id="047ce-110">如果禁用此设置，Windows 10 用户的同步行为会与旧版 Windows 用户相同，并且无法启用文件随选。</span><span class="sxs-lookup"><span data-stu-id="047ce-110">If you disable this setting, Windows 10 users have the same sync behavior as users of previous versions of Windows, and aren't able to turn on Files On-Demand.</span></span> <span data-ttu-id="047ce-111">如果未配置此选项，则用户可以打开或关闭文件随选。</span><span class="sxs-lookup"><span data-stu-id="047ce-111">If you do not configure this setting, users can turn Files On-Demand on or off.</span></span>

<span data-ttu-id="047ce-112">启用此策略会将下面的注册表项值设置为 1。</span><span class="sxs-lookup"><span data-stu-id="047ce-112">Enabling this policy sets the following registry key value to 1.</span></span> <span data-ttu-id="047ce-113">禁用此策略会将以下注册表键值设置为0。</span><span class="sxs-lookup"><span data-stu-id="047ce-113">Disabling this policy sets the following registry key value to 0.</span></span>

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

<span data-ttu-id="047ce-114">如果您在 "设置 "中看不到 "随选文件 "选项，请确保 "Windows Cloud Files Filter Driver "服务的启动类型设置为 2 (AUTO_START)。</span><span class="sxs-lookup"><span data-stu-id="047ce-114">If you can't see the Files On-Demand option in "Settings," make sure the service "Windows Cloud Files Filter Driver" start type is set to 2 (AUTO_START).</span></span> <span data-ttu-id="047ce-115">启用此功能会将以下注册表键值设置为2。</span><span class="sxs-lookup"><span data-stu-id="047ce-115">Enabling this feature sets the following registry key value to 2.</span></span>

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`