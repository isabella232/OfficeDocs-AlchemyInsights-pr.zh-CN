---
title: 删除 Office 以前的 MSI 版本
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003886"
- "6940"
ms.openlocfilehash: 26ab610cb204149536bd23c830a1b8558892a7c0
ms.sourcegitcommit: c033720921cb9a06b9560eedef4f1935e69a846b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2020
ms.locfileid: "49680597"
---
# <a name="remove-prior-msi-versions-of-office"></a><span data-ttu-id="221d1-102">删除 Office 以前的 MSI 版本</span><span class="sxs-lookup"><span data-stu-id="221d1-102">Remove prior MSI versions of Office</span></span>

<span data-ttu-id="221d1-103">在安装 Office 365 专业增强 (，建议先删除 MSI) 版本的 Windows Installer。</span><span class="sxs-lookup"><span data-stu-id="221d1-103">I recommend removing prior Windows Installer (MSI) versions of Office before installing Office 365 ProPlus.</span></span> <span data-ttu-id="221d1-104">下面将说明如何执行此工作：</span><span class="sxs-lookup"><span data-stu-id="221d1-104">Here's how to do this:</span></span>

1. <span data-ttu-id="221d1-105">如果使用 MSI 安装 Office，可以使用 Office 部署工具 (ODT) 卸载 Office。</span><span class="sxs-lookup"><span data-stu-id="221d1-105">If you used MSI to install Office, you can use the Office Deployment Tool (ODT) to uninstall Office.</span></span> <span data-ttu-id="221d1-106">可以在文件文件中使用 RemoveMSI **configuration.xml** 元素。</span><span class="sxs-lookup"><span data-stu-id="221d1-106">You can use the RemoveMSI element in your **configuration.xml** file.</span></span>
1. <span data-ttu-id="221d1-107">按照本文中的说明操作 [：Office 365 安全&合规中心。](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="221d1-107">Follow the instruction in this article: [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span></span>