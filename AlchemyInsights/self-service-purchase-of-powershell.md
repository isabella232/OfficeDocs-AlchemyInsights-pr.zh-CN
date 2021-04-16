---
title: PowerShell 的自助购买
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
- "9001212"
- "3516"
ms.openlocfilehash: 48b5b0a1be1bc03d45a531a1093f18a3f750c37d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51797711"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="857ec-102">PowerShell 的自助购买</span><span class="sxs-lookup"><span data-stu-id="857ec-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="857ec-103">若要使用 MSCommerce PowerShell 模块，需要将其安装在具有 TLS 1.2 的 Windows 10 设备上， (本地管理员权限) 。</span><span class="sxs-lookup"><span data-stu-id="857ec-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="857ec-104">导入并连接到 MSCommerce 模块。</span><span class="sxs-lookup"><span data-stu-id="857ec-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="857ec-105">当系统提示登录时，你将需要使用全局或帐单管理员角色凭据。</span><span class="sxs-lookup"><span data-stu-id="857ec-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="857ec-106">如果没有 TLS 1.2，在尝试获取或更新策略时可能会收到以下错误：</span><span class="sxs-lookup"><span data-stu-id="857ec-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="857ec-107">*ErrorMessage - 基础连接已关闭：发送 时发生意外错误*。</span><span class="sxs-lookup"><span data-stu-id="857ec-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



