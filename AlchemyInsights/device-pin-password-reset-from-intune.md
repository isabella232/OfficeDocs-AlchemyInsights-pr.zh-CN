---
title: 从 Intune 重置设备 PIN 码/密码
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1278"
- "6700008"
ms.openlocfilehash: 66255fc87a55161158aa4121d68d7ccd04b552ec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730977"
---
# <a name="device-pinpassword-reset-from-intune"></a><span data-ttu-id="81976-102">从 Intune 重置设备 PIN 码/密码</span><span class="sxs-lookup"><span data-stu-id="81976-102">Device pin/password reset from Intune</span></span>

<span data-ttu-id="81976-103">可使用“删除密码”操作，删除密码或强制用户在 Intune 中为运行 iOS 或 Android 的设备创建新密码。</span><span class="sxs-lookup"><span data-stu-id="81976-103">You can remove a passcode or force a user to create a new passcode in Intune for a device running iOS or Android by using the Remove Passcode action.</span></span>

<span data-ttu-id="81976-104">仅特定操作系统类型和工作配置文件类型支持此操作。</span><span class="sxs-lookup"><span data-stu-id="81976-104">Only specific operating system types and work profile types support this action.</span></span>

<span data-ttu-id="81976-105">有关支持的平台以及如何触发重置密码操作的详细信息，请参阅[在 Intune 中重置或删除设备密码](https://docs.microsoft.com/intune/device-passcode-reset)。</span><span class="sxs-lookup"><span data-stu-id="81976-105">For details about supported platforms and how to trigger the reset passcode action, see [Reset or remove a device passcode in Intune](https://docs.microsoft.com/intune/device-passcode-reset).</span></span>

<span data-ttu-id="81976-106">在运行 Windows 10 移动版操作系统的设备上，可以使用“PIN 重置”操作将现有 PIN 重置为新值。</span><span class="sxs-lookup"><span data-stu-id="81976-106">You can reset an existing pin to a new value using the Pin Reset action on devices running the Windows 10 Mobile operating system.</span></span> <span data-ttu-id="81976-107">这允许用户解锁设备并根据需要设置新 PIN。</span><span class="sxs-lookup"><span data-stu-id="81976-107">This allows the user to unlock the device and set a new pin as appropriate.</span></span> <span data-ttu-id="81976-108">有关详细信息，请参阅[使用 Intune 重置 Windows 设备上的密码](https://docs.microsoft.com/intune/device-windows-pin-reset)。</span><span class="sxs-lookup"><span data-stu-id="81976-108">For more info, see [Reset the passcode on Windows devices using Intune](https://docs.microsoft.com/intune/device-windows-pin-reset).</span></span>