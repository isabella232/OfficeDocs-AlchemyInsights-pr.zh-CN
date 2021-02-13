---
title: 将 Microsoft Edge 添加到 Microsoft Intune
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177986"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="9f040-102">将 Microsoft Edge 添加到 Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="9f040-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="9f040-103">若要能够部署、配置、监视和保护 Microsoft Edge for Windows 10，必须先将其添加到 Microsoft Intune。</span><span class="sxs-lookup"><span data-stu-id="9f040-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="9f040-104">Intune 支持 Microsoft Edge 77 和更高版本。</span><span class="sxs-lookup"><span data-stu-id="9f040-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="9f040-105">Intune 将检测任何预先存在的 Microsoft Edge 安装。</span><span class="sxs-lookup"><span data-stu-id="9f040-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="9f040-106">如果在用户上下文中安装了 Microsoft Edge，系统安装会覆盖用户上下文中的安装。</span><span class="sxs-lookup"><span data-stu-id="9f040-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="9f040-107">如果在系统上下文中安装了 Microsoft Edge，将报告安装成功。</span><span class="sxs-lookup"><span data-stu-id="9f040-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="9f040-108">对于用户上下文中所有频道，系统上下文中安装的 Microsoft Edge 将覆盖预安装的 Microsoft Edge 77 和更高版本。</span><span class="sxs-lookup"><span data-stu-id="9f040-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="9f040-109">**先决条件**</span><span class="sxs-lookup"><span data-stu-id="9f040-109">**Prerequisite**</span></span>

<span data-ttu-id="9f040-110">Windows 10 版本 1709 或更高版本</span><span class="sxs-lookup"><span data-stu-id="9f040-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="9f040-111">**将 Microsoft Edge 添加到 Intune 的步骤**</span><span class="sxs-lookup"><span data-stu-id="9f040-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="9f040-112">[在 Intune 中配置应用](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)。</span><span class="sxs-lookup"><span data-stu-id="9f040-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="9f040-113">[配置应用信息](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)。</span><span class="sxs-lookup"><span data-stu-id="9f040-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="9f040-114">[配置应用设置](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)。</span><span class="sxs-lookup"><span data-stu-id="9f040-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="9f040-115">[选择范围标记（可选）](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)。</span><span class="sxs-lookup"><span data-stu-id="9f040-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="9f040-116">[添加应用](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)。</span><span class="sxs-lookup"><span data-stu-id="9f040-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="9f040-117">有关更多帮助，请参阅 [疑难解答](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)。</span><span class="sxs-lookup"><span data-stu-id="9f040-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




