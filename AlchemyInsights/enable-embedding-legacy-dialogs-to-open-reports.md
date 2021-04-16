---
title: 支持嵌入旧版对话框以打开报告
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
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814254"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="c5a0f-102">支持嵌入旧版对话框以打开报告</span><span class="sxs-lookup"><span data-stu-id="c5a0f-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="c5a0f-103">**症状**</span><span class="sxs-lookup"><span data-stu-id="c5a0f-103">**Symptom**</span></span>

<span data-ttu-id="c5a0f-104">用户无法打开报告。</span><span class="sxs-lookup"><span data-stu-id="c5a0f-104">Users are unable to open reports.</span></span> <span data-ttu-id="c5a0f-105">“出现错误。</span><span class="sxs-lookup"><span data-stu-id="c5a0f-105">"Something has gone wrong.</span></span> <span data-ttu-id="c5a0f-106">请查看技术详细信息获取更多信息。”</span><span class="sxs-lookup"><span data-stu-id="c5a0f-106">Check technical details for more details."</span></span>

<span data-ttu-id="c5a0f-107">**原因**</span><span class="sxs-lookup"><span data-stu-id="c5a0f-107">**Cause**</span></span>

<span data-ttu-id="c5a0f-108">无法在 UCI 中加载报告，并显示错误“表单描述符为 NULL 或未定义”。</span><span class="sxs-lookup"><span data-stu-id="c5a0f-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="c5a0f-109">UCI 中的报告仍然需要旧版对话框，因此客户系统需要启用 *allowacyacydialogsemdding*。</span><span class="sxs-lookup"><span data-stu-id="c5a0f-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="c5a0f-110">**解决方案**</span><span class="sxs-lookup"><span data-stu-id="c5a0f-110">**Solution**</span></span>

1. <span data-ttu-id="c5a0f-111">转到 **“设置”>“管理”>“系统设置”>“常规”** 选项卡。</span><span class="sxs-lookup"><span data-stu-id="c5a0f-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="c5a0f-112">将“支持在统一界面浏览器客户端中嵌入某些旧版对话框”设置为“**是**”。</span><span class="sxs-lookup"><span data-stu-id="c5a0f-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
