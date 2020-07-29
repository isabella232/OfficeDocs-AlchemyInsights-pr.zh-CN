---
title: 使用 Intune 查找丢失的 iOS 设备
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
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434569"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="0d212-102">使用 Intune 查找丢失的 iOS 设备</span><span class="sxs-lookup"><span data-stu-id="0d212-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="0d212-103">启用 iOS 设备上的丢失模式后，管理员可在锁屏上显示邮件和联系人电话号码。</span><span class="sxs-lookup"><span data-stu-id="0d212-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="0d212-104">启用丢失模式后，管理员可以使用“查找设备”操作来识别设备的物理位置。</span><span class="sxs-lookup"><span data-stu-id="0d212-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="0d212-105">Intune 中的 "定位设备" 操作适用于 iOS 设备，用于显示特定设备在地图上的位置。</span><span class="sxs-lookup"><span data-stu-id="0d212-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="0d212-106">若要执行此操作，iOS 设备必须位于：</span><span class="sxs-lookup"><span data-stu-id="0d212-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="0d212-107">监督模式</span><span class="sxs-lookup"><span data-stu-id="0d212-107">Supervised mode</span></span>
- <span data-ttu-id="0d212-108">丢失模式</span><span class="sxs-lookup"><span data-stu-id="0d212-108">Lost mode</span></span>

<span data-ttu-id="0d212-109">有关详细信息，请参阅 [使用 Intune 在 iOS/iPadOS 设备上启用丢失模式](https://docs.microsoft.com/intune/device-lost-mode)，[使用 Intune 找到丢失的或失窃的 iOS/iPadOS 设备](https://docs.microsoft.com/intune/device-locate)。</span><span class="sxs-lookup"><span data-stu-id="0d212-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="0d212-110">**常见问题解答**</span><span class="sxs-lookup"><span data-stu-id="0d212-110">**FAQ**</span></span>

<span data-ttu-id="0d212-111">问：我发出了从设备中删除公司数据的远程操作命令，而现在它处于挂起状态。</span><span class="sxs-lookup"><span data-stu-id="0d212-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="0d212-112">答：为了成功完成远程操作，目标设备必须处于联机状态且运行正常。</span><span class="sxs-lookup"><span data-stu-id="0d212-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="0d212-113">在以下情况下，远程操作会保持挂起状态 30 天，或除非在以下情形下确认该命令：</span><span class="sxs-lookup"><span data-stu-id="0d212-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="0d212-114">设备没有连接时</span><span class="sxs-lookup"><span data-stu-id="0d212-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="0d212-115">设备使用 Intune 失去其管理状态。</span><span class="sxs-lookup"><span data-stu-id="0d212-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="0d212-116">如果你认为不会再签入某台设备，并且它不能删除公司数据，请选择“删除”。</span><span class="sxs-lookup"><span data-stu-id="0d212-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="0d212-117">删除操作将删除设备记录，使其不再显示在设备的 Intune 列表中。</span><span class="sxs-lookup"><span data-stu-id="0d212-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="0d212-118">如果设备再次处于活动状态，则其用户必须重新注册。</span><span class="sxs-lookup"><span data-stu-id="0d212-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="0d212-119">问：为什么我无法使用某些远程操作？</span><span class="sxs-lookup"><span data-stu-id="0d212-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="0d212-120">答：并非所有平台都支持所有远程设备操作。</span><span class="sxs-lookup"><span data-stu-id="0d212-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="0d212-121">以下远程操作是特定于平台的，因此它们仅可用于指定的平台。</span><span class="sxs-lookup"><span data-stu-id="0d212-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="0d212-122">跳过激活锁（仅限 iOS）</span><span class="sxs-lookup"><span data-stu-id="0d212-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="0d212-123">全新启动（仅限 Windows）</span><span class="sxs-lookup"><span data-stu-id="0d212-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="0d212-124">丢失模式（仅限 iOS）</span><span class="sxs-lookup"><span data-stu-id="0d212-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="0d212-125">定位设备（仅限 iOS）</span><span class="sxs-lookup"><span data-stu-id="0d212-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="0d212-126">重新启动（仅限 Windows）</span><span class="sxs-lookup"><span data-stu-id="0d212-126">Restart (Windows only)</span></span>

<span data-ttu-id="0d212-127">有关各项操作的详细信息，请参阅[可用的设备操作](https://docs.microsoft.com/intune/device-management#available-device-actions)。</span><span class="sxs-lookup"><span data-stu-id="0d212-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>