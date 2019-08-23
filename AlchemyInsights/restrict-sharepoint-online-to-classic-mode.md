---
title: 将 SharePoint Online 限制为经典模式
ms.author: kirks
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: e7ecfd8c2f1a532355bfb8c2c0a846fc0d6e88b1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551549"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="85980-102">将 SharePoint Online 限制为经典模式</span><span class="sxs-lookup"><span data-stu-id="85980-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="85980-103">有些组织仍需要经典模式体验。</span><span class="sxs-lookup"><span data-stu-id="85980-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="85980-104">虽然没有计划在粒度级别删除经典模式, 但不再可能将整个组织 (租户) 限制为列表和库的经典模式。</span><span class="sxs-lookup"><span data-stu-id="85980-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="85980-105">管理员可通过以下方式来管理采用经典模式的各个列表和库, 具体方法是使用我们在以下级别提供的具体选择退出开关:</span><span class="sxs-lookup"><span data-stu-id="85980-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="85980-106">site collection</span><span class="sxs-lookup"><span data-stu-id="85980-106">site collection</span></span>
- <span data-ttu-id="85980-107">网站</span><span class="sxs-lookup"><span data-stu-id="85980-107">site</span></span>
- <span data-ttu-id="85980-108">list</span><span class="sxs-lookup"><span data-stu-id="85980-108">list</span></span>
- <span data-ttu-id="85980-109">图书馆</span><span class="sxs-lookup"><span data-stu-id="85980-109">library</span></span>

<span data-ttu-id="85980-110">此外, 使用新式不支持的某些功能和自定义项的列表仍将自动切换到经典模式。</span><span class="sxs-lookup"><span data-stu-id="85980-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="85980-111">从2019年4月1日起, 禁用租户级别的过程退出新式列表, 库将在5月31日 (2019) 开始并继续。</span><span class="sxs-lookup"><span data-stu-id="85980-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="85980-112">由于租户自愿退出, 以经典模式的列表和库将自动移动到新式。</span><span class="sxs-lookup"><span data-stu-id="85980-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="85980-113">如果需要经典模式, 请参阅此处的[](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023)详细信息和 PnP Powershell 说明,[此处](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout)介绍了可用于今天使用经典模式体验的选项和工具。</span><span class="sxs-lookup"><span data-stu-id="85980-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
