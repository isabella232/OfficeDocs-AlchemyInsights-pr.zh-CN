---
title: 有关夜灯显示设置的帮助
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123026"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="24132-102">有关夜灯显示设置的帮助</span><span class="sxs-lookup"><span data-stu-id="24132-102">Help with the night light display setting</span></span>

<span data-ttu-id="24132-103">若要深入了解夜灯显示设置，请参阅 [在 Windows 10 设备夜间显示](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)。</span><span class="sxs-lookup"><span data-stu-id="24132-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="24132-104">如果"设置"中夜灯选项灰显，请检查显示驱动程序：</span><span class="sxs-lookup"><span data-stu-id="24132-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="24132-105">点击任务栏的搜索框，键入 **设备管理器**，然后从搜索结果中选择 **设备管理器**。</span><span class="sxs-lookup"><span data-stu-id="24132-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="24132-106">展开 **显示适配器**。</span><span class="sxs-lookup"><span data-stu-id="24132-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="24132-107">遗憾的是，如果你的设备使用 DisplayLink 驱动程序或基本显示驱动程序，则夜灯功能不可用。</span><span class="sxs-lookup"><span data-stu-id="24132-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="24132-108">夜灯功能利用最新的图形技术，因此你可能需要更新显示驱动程序：</span><span class="sxs-lookup"><span data-stu-id="24132-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="24132-109">若要检查更新，请转到 **开始** > **设置** > **更新与安全** > **Windows 更新** > **检查更新**。</span><span class="sxs-lookup"><span data-stu-id="24132-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="24132-110">或</span><span class="sxs-lookup"><span data-stu-id="24132-110">OR</span></span>

- <span data-ttu-id="24132-111">访问硬件制造商的支持网站，手动下载并安装最新的显示驱动程序。</span><span class="sxs-lookup"><span data-stu-id="24132-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="24132-112">在注册表中重置夜灯</span><span class="sxs-lookup"><span data-stu-id="24132-112">Reset night light in the registry</span></span>

<span data-ttu-id="24132-113">如果更新显示驱动程序不起作用，则可能需要在注册表中重置夜灯。</span><span class="sxs-lookup"><span data-stu-id="24132-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="24132-114">**注意：** 建议仅向高级用户提供此疑难解答步骤。</span><span class="sxs-lookup"><span data-stu-id="24132-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="24132-115">如果注册表修改不当，可能会出现严重问题。</span><span class="sxs-lookup"><span data-stu-id="24132-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="24132-116">为增强保护，请在修改前备份注册表，以便出现问题时可以还原。</span><span class="sxs-lookup"><span data-stu-id="24132-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="24132-117">在搜索框中，键入 **regedit**，然后在搜索结果中选择 **注册表编辑器**。</span><span class="sxs-lookup"><span data-stu-id="24132-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="24132-118">转到下面的注册表项：</span><span class="sxs-lookup"><span data-stu-id="24132-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="24132-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="24132-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="24132-120">导出并删除以下子项：$$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="24132-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="24132-121">导出并删除以下子项：$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="24132-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="24132-122">重启 Windows，验证夜灯选项是否可用。</span><span class="sxs-lookup"><span data-stu-id="24132-122">Restart Windows and verify if the night light options are available.</span></span>


