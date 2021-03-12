---
title: 在 Linux 计算机上配置和验证 MDATP 的排除项
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735629"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="0cc29-102">在 Linux 计算机上配置和验证 MDATP 的排除项</span><span class="sxs-lookup"><span data-stu-id="0cc29-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="0cc29-103">你可以从 MDATP 扫描中排除某些文件、文件夹、进程和进程打开的文件。</span><span class="sxs-lookup"><span data-stu-id="0cc29-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="0cc29-104">排除项有助于防止对组织唯一或自定义的软件和文件进行错误检测。</span><span class="sxs-lookup"><span data-stu-id="0cc29-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="0cc29-105">排除项还有助于缓解 MDATP 导致的性能问题。</span><span class="sxs-lookup"><span data-stu-id="0cc29-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="0cc29-106">若要了解更多信息，请参阅 [为适用于 Linux 的 MDATP 配置和验证排除项](https://go.microsoft.com/fwlink/?linkid=2144517)。</span><span class="sxs-lookup"><span data-stu-id="0cc29-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="0cc29-107">本文中介绍的排除项不适用于适用于 Linux 的 MDATP 的其他功能，包括终结点检测和响应 (EDR) 。</span><span class="sxs-lookup"><span data-stu-id="0cc29-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="0cc29-108">使用本文中所述的方法排除的文件仍可以触发 EDR 警报和其他检测功能。</span><span class="sxs-lookup"><span data-stu-id="0cc29-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
