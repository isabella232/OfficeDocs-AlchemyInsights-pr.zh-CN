---
title: 在 Intune 中自动清理陈旧设备
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 49a15132253c59189e343aeaa1c11d450b344896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715011"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="e0a51-102">在 Intune 中自动清理陈旧设备</span><span class="sxs-lookup"><span data-stu-id="e0a51-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="e0a51-103">Intune 允许管理员配置 90 和 270 天之间的时间间隔，之后将从服务中删除陈旧设备。</span><span class="sxs-lookup"><span data-stu-id="e0a51-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="e0a51-104">此设置是组织范围的，激活后将立即生效。</span><span class="sxs-lookup"><span data-stu-id="e0a51-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="e0a51-105">在超过设置的时间段内未签入 Intune 服务器的任何设备都将被永久删除。</span><span class="sxs-lookup"><span data-stu-id="e0a51-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="e0a51-106">**注意** 只有 MDM 设备对象才有资格执行此清除操作。</span><span class="sxs-lookup"><span data-stu-id="e0a51-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="e0a51-107">仅排除了 EAS 设备对象。</span><span class="sxs-lookup"><span data-stu-id="e0a51-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="e0a51-108">有关根据设备清理设置及其“状态”何时可以删除设备的其他信息：</span><span class="sxs-lookup"><span data-stu-id="e0a51-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="e0a51-109">设置：**上次签入日期后删除设备：是（指定天数内的某些值 (N)）**</span><span class="sxs-lookup"><span data-stu-id="e0a51-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="e0a51-110">根据设置中配置的值 (N)，Intune 服务会在上次成功签入的指定天数内删除设备。</span><span class="sxs-lookup"><span data-stu-id="e0a51-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="e0a51-111">设置：**上次签入日期后删除设备：否**</span><span class="sxs-lookup"><span data-stu-id="e0a51-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="e0a51-112">设备证书过期且未续订 180 天后，将删除该设备。</span><span class="sxs-lookup"><span data-stu-id="e0a51-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="e0a51-113">**注意** 在两种情况下，必须在 Intune 中成功登记设备。</span><span class="sxs-lookup"><span data-stu-id="e0a51-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="e0a51-114">第一次使用 Intune 服务签入设备的过程中将发生登记。</span><span class="sxs-lookup"><span data-stu-id="e0a51-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="e0a51-115">如果设备向 Intune 成功注册但未在 Intune 中登记，则设备将在注册后 270 天内删除。</span><span class="sxs-lookup"><span data-stu-id="e0a51-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="e0a51-116">（头 90 天将设备标记为已吊销，接下来的 180 天删除记录。）</span><span class="sxs-lookup"><span data-stu-id="e0a51-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="e0a51-117">Intune 控制台中当前没有任何机制可用于确定任何给定设备的设备认证到期日期。</span><span class="sxs-lookup"><span data-stu-id="e0a51-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>