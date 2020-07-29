---
title: Intune 设备清单
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
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434582"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="aae41-102">Intune 设备清单</span><span class="sxs-lookup"><span data-stu-id="aae41-102">Intune Device Inventory</span></span>

<span data-ttu-id="aae41-103">“设备”边栏选项卡使管理员能够按设备深入了解 Intune 中管理的设备。</span><span class="sxs-lookup"><span data-stu-id="aae41-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="aae41-104">所显示的信息包括：硬件、发现的应用程序、设备合规性状态和设备配置状态。</span><span class="sxs-lookup"><span data-stu-id="aae41-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="aae41-105">硬件和发现的应用程序的清单数据将按七天周期收集。</span><span class="sxs-lookup"><span data-stu-id="aae41-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="aae41-106">根据设备操作系统以及设备是个人拥有还是企业拥有，报告的应用程序和硬件特定元素会有所不同。</span><span class="sxs-lookup"><span data-stu-id="aae41-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="aae41-107">有关详细信息，请参阅[查看 Intune 中的设备详细信息](https://docs.microsoft.com/intune/device-inventory)。</span><span class="sxs-lookup"><span data-stu-id="aae41-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="aae41-108">**常见问题解答**</span><span class="sxs-lookup"><span data-stu-id="aae41-108">**FAQ**</span></span>

<span data-ttu-id="aae41-109">问：我没有收到注册了 Intune 的 Windows 设备上存在的应用程序的完整清单。</span><span class="sxs-lookup"><span data-stu-id="aae41-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="aae41-110">这是为什么？</span><span class="sxs-lookup"><span data-stu-id="aae41-110">Why not?</span></span>

<span data-ttu-id="aae41-111">答：此时，仅列出被标识为公司设备的 Windows 10 电脑的新式应用。</span><span class="sxs-lookup"><span data-stu-id="aae41-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="aae41-112">Intune 不会收集有关在这些设备上安装的 Win32 应用的信息。</span><span class="sxs-lookup"><span data-stu-id="aae41-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="aae41-113">答：为什么不从所有设备收集电话号码？</span><span class="sxs-lookup"><span data-stu-id="aae41-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="aae41-114">答：例如，当你运行移动设备清单报告时，在 Intune 中被归类为公司设备的电话不会用其完整电话号码标识。</span><span class="sxs-lookup"><span data-stu-id="aae41-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="aae41-115">“自带设备办公”电话号码总是用星号 (\*\*\*\*) 部分屏蔽，并且只显示最后四位数字。</span><span class="sxs-lookup"><span data-stu-id="aae41-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>