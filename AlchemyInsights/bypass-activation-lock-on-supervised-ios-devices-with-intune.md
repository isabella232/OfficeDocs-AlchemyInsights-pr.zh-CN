---
title: 使用 Intune 跳过受监督的 iOS 设备上的激活锁
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 743b5917c08b0a49a8c5791bdeb59a1672dd0fc7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757290"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="6ab7a-102">使用 Intune 跳过受监督的 iOS 设备上的激活锁</span><span class="sxs-lookup"><span data-stu-id="6ab7a-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="6ab7a-103">通过跳过 iOS 设备上的激活锁，当用户在公司设备上启用激活锁并从公司离职后，你可以更轻松地进行恢复。</span><span class="sxs-lookup"><span data-stu-id="6ab7a-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="6ab7a-104">跳过激活锁的先决条件包括：</span><span class="sxs-lookup"><span data-stu-id="6ab7a-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="6ab7a-105">设备是“受监督的设备”。</span><span class="sxs-lookup"><span data-stu-id="6ab7a-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="6ab7a-106">已使用 Intune 中的 iOS 设备限制策略成功启用激活锁。</span><span class="sxs-lookup"><span data-stu-id="6ab7a-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="6ab7a-107">此外，跳过激活锁时，应执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="6ab7a-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="6ab7a-108">实际拥有要擦除的设备。</span><span class="sxs-lookup"><span data-stu-id="6ab7a-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="6ab7a-109">在发出擦除命令之前先复制代码。</span><span class="sxs-lookup"><span data-stu-id="6ab7a-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="6ab7a-110">**注意：** 擦除代码不区分大小写，因此不需要“-”字符。</span><span class="sxs-lookup"><span data-stu-id="6ab7a-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="6ab7a-111">有关详细信息，请参阅[使用 Intune 跳过受监督的 iOS 设备上的激活锁](https://docs.microsoft.com/intune/device-activation-lock-bypass)。</span><span class="sxs-lookup"><span data-stu-id="6ab7a-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="6ab7a-112">**常见问题解答**</span><span class="sxs-lookup"><span data-stu-id="6ab7a-112">**FAQ**</span></span>

<span data-ttu-id="6ab7a-113">问：**我发出了从设备中删除公司数据的远程操作命令，而现在它处于挂起状态。**</span><span class="sxs-lookup"><span data-stu-id="6ab7a-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="6ab7a-114">答：为了成功完成远程操作，目标设备必须处于联机状态且运行正常。</span><span class="sxs-lookup"><span data-stu-id="6ab7a-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="6ab7a-115">在以下情况下，远程操作会保持挂起状态 30 天，或除非设备在以下情形下确认该命令：</span><span class="sxs-lookup"><span data-stu-id="6ab7a-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="6ab7a-116">没有连接。</span><span class="sxs-lookup"><span data-stu-id="6ab7a-116">Does not have connectivity.</span></span>
- <span data-ttu-id="6ab7a-117">使用 Intune 失去其管理状态。</span><span class="sxs-lookup"><span data-stu-id="6ab7a-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="6ab7a-118">如果你认为不会再签入某台设备，并且它不会删除公司数据，请选择“删除”。</span><span class="sxs-lookup"><span data-stu-id="6ab7a-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="6ab7a-119">删除操作将删除设备记录，使其不再显示在设备的 Intune 列表中。</span><span class="sxs-lookup"><span data-stu-id="6ab7a-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="6ab7a-120">为了使该设备再次激活，其用户必须重新注册它。</span><span class="sxs-lookup"><span data-stu-id="6ab7a-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="6ab7a-121">问：**为什么我无法使用某些远程操作？**</span><span class="sxs-lookup"><span data-stu-id="6ab7a-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="6ab7a-122">答：并非所有平台都支持所有远程设备操作。</span><span class="sxs-lookup"><span data-stu-id="6ab7a-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="6ab7a-123">以下远程操作特定于平台。</span><span class="sxs-lookup"><span data-stu-id="6ab7a-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="6ab7a-124">跳过激活锁（仅限 iOS）</span><span class="sxs-lookup"><span data-stu-id="6ab7a-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="6ab7a-125">全新启动（仅限 Windows）</span><span class="sxs-lookup"><span data-stu-id="6ab7a-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="6ab7a-126">丢失模式（仅限 iOS）</span><span class="sxs-lookup"><span data-stu-id="6ab7a-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="6ab7a-127">定位设备（仅限 iOS）</span><span class="sxs-lookup"><span data-stu-id="6ab7a-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="6ab7a-128">重新启动（仅限 Windows）</span><span class="sxs-lookup"><span data-stu-id="6ab7a-128">Restart (Windows only)</span></span>

<span data-ttu-id="6ab7a-129">有关各项操作的详细信息，请参阅[可用的设备操作](https://docs.microsoft.com/intune/device-management#available-device-actions)。</span><span class="sxs-lookup"><span data-stu-id="6ab7a-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>