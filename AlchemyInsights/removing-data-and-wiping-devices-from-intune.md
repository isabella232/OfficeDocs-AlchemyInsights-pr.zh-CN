---
title: 从 Intune 删除数据和擦除设备
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
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416303"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="34617-102">从 Intune 删除数据和擦除设备</span><span class="sxs-lookup"><span data-stu-id="34617-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="34617-103">设备停用和设备擦除远程操作可用于删除由 Intune 管理的公司数据或执行出厂重置并将设备恢复为默认设置。</span><span class="sxs-lookup"><span data-stu-id="34617-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="34617-104">登录 Microsoft 365 设备管理，然后转到“**设备**” > “**所有设备**”。</span><span class="sxs-lookup"><span data-stu-id="34617-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="34617-105">选择要擦除的设备。</span><span class="sxs-lookup"><span data-stu-id="34617-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="34617-106">选择要执行的远程擦除类型。</span><span class="sxs-lookup"><span data-stu-id="34617-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="34617-107">停用只会删除组织信息，而完全擦除会将设备还原为出厂设置。</span><span class="sxs-lookup"><span data-stu-id="34617-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="34617-108">选择“**是**”进行确认。</span><span class="sxs-lookup"><span data-stu-id="34617-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="34617-109">擦除完成后，"设备"操作状态将显示为" *停用挂起*。</span><span class="sxs-lookup"><span data-stu-id="34617-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="34617-110">操作完成后，你将不能再在受管理的设备列表中看到该移动设备。</span><span class="sxs-lookup"><span data-stu-id="34617-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="34617-111">不能从加入 Azure AD 的设备中删除公司数据。</span><span class="sxs-lookup"><span data-stu-id="34617-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="34617-112">有关停用和擦除操作的影响的完整详细信息，包括保留内容及删除内容，请参阅以下文档：</span><span class="sxs-lookup"><span data-stu-id="34617-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="34617-113">[通过使用擦除、停用或手动取消上卷设备来删除](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe)。</span><span class="sxs-lookup"><span data-stu-id="34617-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="34617-114">如何只从 Intune 托管应用擦除企业数据</span><span class="sxs-lookup"><span data-stu-id="34617-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="34617-115">[擦除 macOS 设备应用更新](https://docs.microsoft.com/mem/intune/remote-actions/device-erase)。</span><span class="sxs-lookup"><span data-stu-id="34617-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>