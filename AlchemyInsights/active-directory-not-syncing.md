---
title: Active Directory 未同步
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822841"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="b9216-102">Active Directory 未同步</span><span class="sxs-lookup"><span data-stu-id="b9216-102">Active Directory not syncing</span></span>

<span data-ttu-id="b9216-103">如果您收到同步错误（如"最近未同步"）或注意到 Office 管理门户中的目录同步状态显示"上次同步时间超过 3 天"，可能是 AADConnect 的设置不正确或权限不足，无法执行同步。</span><span class="sxs-lookup"><span data-stu-id="b9216-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="b9216-104">使用快速设置重新安装 AADConnect 可能会快速解决问题：</span><span class="sxs-lookup"><span data-stu-id="b9216-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="b9216-105">[下载最新版本的 AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771)。</span><span class="sxs-lookup"><span data-stu-id="b9216-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="b9216-106">[按照快速安装的说明进行操作](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)。</span><span class="sxs-lookup"><span data-stu-id="b9216-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="b9216-107">有关 AADConnect 服务帐户的详细信息，请参阅 [Azure AD Connect：帐户和权限](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)。</span><span class="sxs-lookup"><span data-stu-id="b9216-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
