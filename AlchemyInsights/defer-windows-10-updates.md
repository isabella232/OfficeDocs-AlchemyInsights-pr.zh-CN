---
title: 推迟 Windows 10 更新
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1128"
- "6700007"
ms.openlocfilehash: 233354386eb319860f25b3929b6be528438cc865
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680413"
---
# <a name="defer-windows-10-updates"></a><span data-ttu-id="16608-102">推迟 Windows 10 更新</span><span class="sxs-lookup"><span data-stu-id="16608-102">Defer Windows 10 updates</span></span>

<span data-ttu-id="16608-103">若要推迟推送给用户的 Windows 10 更新，请按照以下步骤操作：</span><span class="sxs-lookup"><span data-stu-id="16608-103">To defer the Windows 10 updates pushed to users, follow these steps:</span></span>

1. <span data-ttu-id="16608-104">登录 Azure 门户。</span><span class="sxs-lookup"><span data-stu-id="16608-104">Sign in to the Azure portal.</span></span>
2. <span data-ttu-id="16608-105">选择“**软件更新**”  >  “**Windows 10 更新通道**”。</span><span class="sxs-lookup"><span data-stu-id="16608-105">Select  **Software Updates**  >  **Windows 10 Update Rings**.</span></span>
3. <span data-ttu-id="16608-106">如果没有更新通道，请选择相关选项来新建一个。</span><span class="sxs-lookup"><span data-stu-id="16608-106">If you don't have an update ring, select the option to create a new one.</span></span>
4. <span data-ttu-id="16608-107">输入名称和可选说明，然后选择“**设置配置**”。</span><span class="sxs-lookup"><span data-stu-id="16608-107">Enter a name and optional description, and then select  **Settings Configure**.</span></span>
5. <span data-ttu-id="16608-108">自定义推迟不同更新的时间范围。</span><span class="sxs-lookup"><span data-stu-id="16608-108">Customize the timeframe for deferring different updates.</span></span> <span data-ttu-id="16608-109">最大推迟时间基于更新类型：</span><span class="sxs-lookup"><span data-stu-id="16608-109">Maximum deferred time is based on the type of update:</span></span>
    - <span data-ttu-id="16608-110">**质量更新** - 自发布之日起，最长可推迟 30 天。</span><span class="sxs-lookup"><span data-stu-id="16608-110">**Quality updates**  can be deferred up to 30 days from their release.</span></span>
    - <span data-ttu-id="16608-111">**功能更新** - 自发布之日起，最长可推迟 180 天。</span><span class="sxs-lookup"><span data-stu-id="16608-111">**Feature updates**  can be deferred up to 180 days from their release.</span></span>
