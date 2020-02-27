---
title: PowerShell 的自我服务购买
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: 5e47e08e3309b3d58908e10ee06021da00f230bb
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091665"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="971a8-102">PowerShell 的自我服务购买</span><span class="sxs-lookup"><span data-stu-id="971a8-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="971a8-103">若要使用 MSCommerce PowerShell 模块，需要将其安装在带 TLS 1.2 的 Windows 10 设备上（需要本地管理员权限）。</span><span class="sxs-lookup"><span data-stu-id="971a8-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="971a8-104">导入并连接到 MSCommerce 模块。</span><span class="sxs-lookup"><span data-stu-id="971a8-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="971a8-105">当系统提示您登录时，将需要使用全局或帐单管理员角色凭据。</span><span class="sxs-lookup"><span data-stu-id="971a8-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="971a8-106">如果没有 TLS 1.2，则在尝试获取或更新策略时可能会收到以下错误：</span><span class="sxs-lookup"><span data-stu-id="971a8-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="971a8-107">*ErrorMessage-基础连接已关闭：发送时发生意外错误*。</span><span class="sxs-lookup"><span data-stu-id="971a8-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>


