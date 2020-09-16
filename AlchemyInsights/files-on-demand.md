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
ms.openlocfilehash: e0ba83778179abefe3ac4fe3e8ab0303d65ad929
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745298"
---
# <a name="configure-files-on-demand"></a><span data-ttu-id="f1e0c-102">配置文件随选</span><span class="sxs-lookup"><span data-stu-id="f1e0c-102">Configure Files On-Demand</span></span>

<span data-ttu-id="f1e0c-103">OneDrive 文件随选可帮助访问 OneDrive 中的所有文件，而无需下载所有这些文件和使用设备上的存储空间。</span><span class="sxs-lookup"><span data-stu-id="f1e0c-103">OneDrive Files On-Demand helps you access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

<span data-ttu-id="f1e0c-104">要在电脑上配置文件随选，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="f1e0c-104">To configure Files On-Demand on your PC:</span></span>

1. <span data-ttu-id="f1e0c-105">选择Windows任务栏通知区域中的白色或蓝色**OneDrive**云图标。</span><span class="sxs-lookup"><span data-stu-id="f1e0c-105">Select the white or blue **OneDrive** cloud icon in the Windows taskbar notification area.</span></span> <span data-ttu-id="f1e0c-106">选择 \*\* 帮助 & "设置 \*\* 齿轮图标 > **设置s**。</span><span class="sxs-lookup"><span data-stu-id="f1e0c-106">Select the **Help & Settings** gear icon > **Settings**.</span></span>
2. <span data-ttu-id="f1e0c-107">在“**设置**”选项卡上，选中“**节省空间并在需要使用时下载文件**”复选框。</span><span class="sxs-lookup"><span data-stu-id="f1e0c-107">On the **Settings** tab, select the **Save space and download files as you use them** box.</span></span>  

<span data-ttu-id="f1e0c-108">还可以使用注册表配置文件随选。</span><span class="sxs-lookup"><span data-stu-id="f1e0c-108">You can also configure Files On-Demand using the registry.</span></span>

<span data-ttu-id="f1e0c-109">如果禁用此设置，Windows 10 用户的同步行为会与旧版 Windows 用户相同，并且无法启用文件随选。</span><span class="sxs-lookup"><span data-stu-id="f1e0c-109">If you disable this setting, Windows 10 users have the same sync behavior as users of previous versions of Windows, and aren't able to turn on Files On-Demand.</span></span> <span data-ttu-id="f1e0c-110">如果未配置此选项，则用户可以打开或关闭文件随选。</span><span class="sxs-lookup"><span data-stu-id="f1e0c-110">If you do not configure this setting, users can turn Files On-Demand on or off.</span></span>

<span data-ttu-id="f1e0c-111">启用此策略会将下面的注册表项值设置为 1。</span><span class="sxs-lookup"><span data-stu-id="f1e0c-111">Enabling this policy sets the following registry key value to 1.</span></span> <span data-ttu-id="f1e0c-112">禁用此策略会将以下注册表键值设置为0。</span><span class="sxs-lookup"><span data-stu-id="f1e0c-112">Disabling this policy sets the following registry key value to 0.</span></span>

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

<span data-ttu-id="f1e0c-113">如果您在 "设置 "中看不到 "随选文件 "选项，请确保 "Windows Cloud Files Filter Driver "服务的启动类型设置为 2 (AUTO_START)。</span><span class="sxs-lookup"><span data-stu-id="f1e0c-113">If you can't see the Files On-Demand option in "Settings," make sure the service "Windows Cloud Files Filter Driver" start type is set to 2 (AUTO_START).</span></span> <span data-ttu-id="f1e0c-114">启用此功能会将以下注册表键值设置为2。</span><span class="sxs-lookup"><span data-stu-id="f1e0c-114">Enabling this feature sets the following registry key value to 2.</span></span>

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`