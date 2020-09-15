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
ms.openlocfilehash: 24330dffb38be14dd369960ff86d4650d60c55ec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47701273"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="c7345-102">从 Intune 删除数据和擦除设备</span><span class="sxs-lookup"><span data-stu-id="c7345-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="c7345-103">设备停用和设备擦除远程操作可用于删除由 Intune 管理的公司数据或执行出厂重置并将设备恢复为默认设置。</span><span class="sxs-lookup"><span data-stu-id="c7345-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="c7345-104">登录 Microsoft 365 设备管理，然后转到“**设备**” > “**所有设备**”。</span><span class="sxs-lookup"><span data-stu-id="c7345-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="c7345-105">选择要擦除的设备。</span><span class="sxs-lookup"><span data-stu-id="c7345-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="c7345-106">选择要执行的远程擦除类型。</span><span class="sxs-lookup"><span data-stu-id="c7345-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="c7345-107">停用只会删除组织信息，而完全擦除会将设备还原为出厂设置。</span><span class="sxs-lookup"><span data-stu-id="c7345-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="c7345-108">选择“**是**”进行确认。</span><span class="sxs-lookup"><span data-stu-id="c7345-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="c7345-109">在擦除完成之前，设备操作状态将显示为“等待停用”。</span><span class="sxs-lookup"><span data-stu-id="c7345-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="c7345-110">操作完成后，你将不能再在受管理的设备列表中看到该移动设备。</span><span class="sxs-lookup"><span data-stu-id="c7345-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="c7345-111">**注意** 无法从已加入 Azure AD 的设备中删除公司数据。</span><span class="sxs-lookup"><span data-stu-id="c7345-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="c7345-112">有关停用和擦除操作的影响的完整详细信息（包括保留的内容和删除的内容），请参阅[使用擦除、停用或手动取消注册设备来删除设备](https://docs.microsoft.com/intune/devices-wipe)。</span><span class="sxs-lookup"><span data-stu-id="c7345-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="c7345-113">若要擦除 macOS 设备中的所有数据，请参阅[擦除 macOS 设备中的所有数据](https://docs.microsoft.com/intune/device-erase)。</span><span class="sxs-lookup"><span data-stu-id="c7345-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>