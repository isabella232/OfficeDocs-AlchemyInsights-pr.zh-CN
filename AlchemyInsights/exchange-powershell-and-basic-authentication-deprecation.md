---
title: Exchange PowerShell 和基本身份验证弃用
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813462"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="330f5-102">Exchange PowerShell 和基本身份验证弃用</span><span class="sxs-lookup"><span data-stu-id="330f5-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="330f5-103">有关如何在不使用基本身份验证的情况下连接到 Exchange Online PowerShell 的最新信息，[请转到此处](https://aka.ms/exops-docs)。</span><span class="sxs-lookup"><span data-stu-id="330f5-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="330f5-104">PowerShell V2 模块不使用基本身份验证。</span><span class="sxs-lookup"><span data-stu-id="330f5-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="330f5-105">请注意，仍需在客户端计算机上启用基本身份验证。</span><span class="sxs-lookup"><span data-stu-id="330f5-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="330f5-106">新版 PowerShell V2 模块使用新式身份验证建立连接，以启用所有基于 REST 的 V2 Cmdlet。</span><span class="sxs-lookup"><span data-stu-id="330f5-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="330f5-107">除了 V2 cmdlet 之外，还可访问需要建立远程 PowerShell 会话的旧版远程 PowerShell （RPS） Cmdlet。</span><span class="sxs-lookup"><span data-stu-id="330f5-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="330f5-108">在 Windows 计算机上建立 RPS 会话需要在客户端计算机上启用 WinRM 基本身份验证，即使该模块使用新式身份验证机制向该服务进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="330f5-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="330f5-109">WinRM 基本身份验证管道用于传输新式身份验证令牌。</span><span class="sxs-lookup"><span data-stu-id="330f5-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="330f5-110">如果客户端计算机上禁用了 WinRM 基本身份验证，新版 V2 cmdlet 将继续工作（但旧版 RPS cmdlet 不会）。</span><span class="sxs-lookup"><span data-stu-id="330f5-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
