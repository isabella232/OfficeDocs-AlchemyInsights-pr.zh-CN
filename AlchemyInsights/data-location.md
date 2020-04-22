---
title: 数据位置
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655272"
---
# <a name="data-location"></a><span data-ttu-id="f317b-102">数据位置</span><span class="sxs-lookup"><span data-stu-id="f317b-102">Data location</span></span>

<span data-ttu-id="f317b-103">你可以在管理中心或通过 PowerShell 连接到 Exchange Online 来查看你的租户的位置。</span><span class="sxs-lookup"><span data-stu-id="f317b-103">You can view the location of your tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="f317b-104">**管理中心：**</span><span class="sxs-lookup"><span data-stu-id="f317b-104">**Admin center:**</span></span>
1. <span data-ttu-id="f317b-105">登录到[管理中心](https://admin.microsoft.com/Adminportal/Home)。</span><span class="sxs-lookup"><span data-stu-id="f317b-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="f317b-106">选择 "**设置** > **组织配置文件**"。</span><span class="sxs-lookup"><span data-stu-id="f317b-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="f317b-107">在 "**数据位置**" 下，选择 "**查看详细信息**"。</span><span class="sxs-lookup"><span data-stu-id="f317b-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="f317b-108">**PowerShell**</span><span class="sxs-lookup"><span data-stu-id="f317b-108">**PowerShell:**</span></span>
1. <span data-ttu-id="f317b-109">使用 Windows PowerShell 连接到 Exchange Online。</span><span class="sxs-lookup"><span data-stu-id="f317b-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="f317b-110">执行[OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet 可显示租户的属性列表。</span><span class="sxs-lookup"><span data-stu-id="f317b-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant's properties.</span></span> 
3. <span data-ttu-id="f317b-111">查看 OrganizationId 属性。</span><span class="sxs-lookup"><span data-stu-id="f317b-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="f317b-112">当您具有 EXO 和 SPO 的数据位置时，可以确定您的[数据所在位置](https://products.office.com/where-is-your-data-located)可能使用的其他服务的数据位置。</span><span class="sxs-lookup"><span data-stu-id="f317b-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>