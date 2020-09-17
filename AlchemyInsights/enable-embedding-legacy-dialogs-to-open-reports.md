---
title: 支持嵌入旧版对话框以打开报告
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: 285933e607ac7e58256709f0c9cf2851250ce211
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806425"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="3e8f1-102">支持嵌入旧版对话框以打开报告</span><span class="sxs-lookup"><span data-stu-id="3e8f1-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="3e8f1-103">**症状**</span><span class="sxs-lookup"><span data-stu-id="3e8f1-103">**Symptom**</span></span>

<span data-ttu-id="3e8f1-104">用户无法打开报告。</span><span class="sxs-lookup"><span data-stu-id="3e8f1-104">Users are unable to open reports.</span></span> <span data-ttu-id="3e8f1-105">“出现错误。</span><span class="sxs-lookup"><span data-stu-id="3e8f1-105">"Something has gone wrong.</span></span> <span data-ttu-id="3e8f1-106">请查看技术详细信息获取更多信息。”</span><span class="sxs-lookup"><span data-stu-id="3e8f1-106">Check technical details for more details."</span></span>

<span data-ttu-id="3e8f1-107">**原因**</span><span class="sxs-lookup"><span data-stu-id="3e8f1-107">**Cause**</span></span>

<span data-ttu-id="3e8f1-108">无法在 UCI 中加载报告，并显示错误“表单描述符为 NULL 或未定义”。</span><span class="sxs-lookup"><span data-stu-id="3e8f1-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="3e8f1-109">UCI 中的报告仍然需要旧版对话框，因此客户系统需要启用 *allowacyacydialogsemdding*。</span><span class="sxs-lookup"><span data-stu-id="3e8f1-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="3e8f1-110">**解决方案**</span><span class="sxs-lookup"><span data-stu-id="3e8f1-110">**Solution**</span></span>

1. <span data-ttu-id="3e8f1-111">转到 **“设置”>“管理”>“系统设置”>“常规”** 选项卡。</span><span class="sxs-lookup"><span data-stu-id="3e8f1-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="3e8f1-112">将“支持在统一界面浏览器客户端中嵌入某些旧版对话框”设置为“**是**”。</span><span class="sxs-lookup"><span data-stu-id="3e8f1-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
