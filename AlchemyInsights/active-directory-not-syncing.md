---
title: Active Directory 未同步
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697619"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="bdf42-102">Active Directory 未同步</span><span class="sxs-lookup"><span data-stu-id="bdf42-102">Active Directory not syncing</span></span>

<span data-ttu-id="bdf42-103">如果您收到同步错误，例如 "无最近同步"，或注意 Office 管理员门户中的目录同步状态说出 "上次同步时间超过3天前"，可能是 AADConnect 的设置不正确或权限不足，无法执行同步。</span><span class="sxs-lookup"><span data-stu-id="bdf42-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="bdf42-104">使用快速设置重新安装 AADConnect 可能会快速解决问题：</span><span class="sxs-lookup"><span data-stu-id="bdf42-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="bdf42-105">[下载 AADConnect 的最新版本](https://go.microsoft.com/fwlink/?LinkId=615771)。</span><span class="sxs-lookup"><span data-stu-id="bdf42-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="bdf42-106">[按照 express 安装的说明进行](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)操作。</span><span class="sxs-lookup"><span data-stu-id="bdf42-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="bdf42-107">有关 AADConnect 服务帐户的详细信息，请参阅 [Azure AD Connect：帐户和权限](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)。</span><span class="sxs-lookup"><span data-stu-id="bdf42-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
