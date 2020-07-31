---
title: 暂停计划的更新
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2020
ms.locfileid: "46530584"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="d8acc-102">暂停计划的更新</span><span class="sxs-lookup"><span data-stu-id="d8acc-102">Pausing scheduled updates</span></span>

<span data-ttu-id="d8acc-103">发出暂停命令后，设备在下一次签入 Intune 前不会处理该命令。</span><span class="sxs-lookup"><span data-stu-id="d8acc-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="d8acc-104">因此，你的设备可能存在以下情况：</span><span class="sxs-lookup"><span data-stu-id="d8acc-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="d8acc-105">签入前已安装计划的更新。</span><span class="sxs-lookup"><span data-stu-id="d8acc-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="d8acc-106">在你发出暂停命令时已关闭电源。</span><span class="sxs-lookup"><span data-stu-id="d8acc-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="d8acc-107">在这种情况下，当设备接通电源后，它们可能已在签入前下载并安装了计划的更新。</span><span class="sxs-lookup"><span data-stu-id="d8acc-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>