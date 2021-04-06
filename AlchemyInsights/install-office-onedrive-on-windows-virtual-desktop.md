---
title: 在 Windows Virtual Desktop 安装 Office 和 OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590264"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a><span data-ttu-id="33c9e-102">在 Windows Virtual Desktop 安装 Office 和 OneDrive</span><span class="sxs-lookup"><span data-stu-id="33c9e-102">Install Office and OneDrive on Windows Virtual Desktop</span></span>

1. <span data-ttu-id="33c9e-103">[准备和自定义主 VHD](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image)。</span><span class="sxs-lookup"><span data-stu-id="33c9e-103">[Prepare and customize a master VHD image](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image).</span></span> <span data-ttu-id="33c9e-104">如果尚未创建虚拟机 （VM），请创建虚拟机。</span><span class="sxs-lookup"><span data-stu-id="33c9e-104">Create a virtual machine (VM) if it hasn't already been created.</span></span>

1. <span data-ttu-id="33c9e-105">[在共享计算机激活模式下安装 Office](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode)。</span><span class="sxs-lookup"><span data-stu-id="33c9e-105">[Install Office in shared computer activation mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode).</span></span> <span data-ttu-id="33c9e-106">通过共享计算机激活，多个用户访问 Office。</span><span class="sxs-lookup"><span data-stu-id="33c9e-106">Shared computer activation allows multiple users to access Office.</span></span>

1. <span data-ttu-id="33c9e-107">[按计算机模式安装 OneDrive](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode)。</span><span class="sxs-lookup"><span data-stu-id="33c9e-107">[Install OneDrive in per-machine mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode).</span></span> <span data-ttu-id="33c9e-108">通常，OneDrive 是按用户安装的，但此处应按计算机进行安装。</span><span class="sxs-lookup"><span data-stu-id="33c9e-108">Normally, OneDrive is installed per user, but here, it should be installed per machine.</span></span>