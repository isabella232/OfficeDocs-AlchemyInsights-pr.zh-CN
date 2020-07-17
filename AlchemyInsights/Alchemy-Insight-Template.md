---
title: 与 filename 的效果最好
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750960"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="23d17-102">"必需的 Alchemy 标头 H1，H2's 不起作用。"</span><span class="sxs-lookup"><span data-stu-id="23d17-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="23d17-103">用于 Alchemy 创作的最佳做法和指南：</span><span class="sxs-lookup"><span data-stu-id="23d17-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="23d17-104">**不在文件夹中嵌套 Alchemy 见解**-这将断开 url 结构。</span><span class="sxs-lookup"><span data-stu-id="23d17-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="23d17-105">我们正在寻求解决此情况的情况。</span><span class="sxs-lookup"><span data-stu-id="23d17-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="23d17-106">**AlchemyInsights**文件夹中的文件的大小写文件名应带有带空格的连字符（ex）。</span><span class="sxs-lookup"><span data-stu-id="23d17-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="23d17-107">操作***方法-保留 "启用-保留***"。</span><span class="sxs-lookup"><span data-stu-id="23d17-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="23d17-108">将规则 ID 或存储桶 ID 包含在 ms. 自定义域中的[Alchemy 合作伙伴门户](https://alchemyportal.azurewebsites.net)中。</span><span class="sxs-lookup"><span data-stu-id="23d17-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="23d17-109">ex.</span><span class="sxs-lookup"><span data-stu-id="23d17-109">ex.</span></span> <span data-ttu-id="23d17-110">***ms. custom：100021***</span><span class="sxs-lookup"><span data-stu-id="23d17-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="23d17-111">将此文件顶部的元数据的其余部分用作模板。</span><span class="sxs-lookup"><span data-stu-id="23d17-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="23d17-112">在[Alchemy 合作伙伴门户](https://alchemyportal.azurewebsites.net)中，向下导航到 "**客户洞察力标题：** " 部分，并将其用作洞察力的 H1 标题的起始点。</span><span class="sxs-lookup"><span data-stu-id="23d17-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="23d17-113">Alchemy 见解必须在顶部只有一个 H1，否则它们将在生产中中断。</span><span class="sxs-lookup"><span data-stu-id="23d17-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="23d17-114">H2s 不呈现任何内容，因此使用**粗体**或其他约定表示单独的节。</span><span class="sxs-lookup"><span data-stu-id="23d17-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="23d17-115">接下来，使用 Alchemy 规则页面的 "客户见解" 部分中的草稿材料填写正文文本</span><span class="sxs-lookup"><span data-stu-id="23d17-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="23d17-116">项目符号列表正常</span><span class="sxs-lookup"><span data-stu-id="23d17-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="23d17-117">编号列表</span><span class="sxs-lookup"><span data-stu-id="23d17-117">Numbered lists too</span></span>
    1. <span data-ttu-id="23d17-118">**粗体**和*斜体*为-正常</span><span class="sxs-lookup"><span data-stu-id="23d17-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="23d17-119">链接应始终是 **"web 上的链接"/External**或指向**UI 元素的深层链接**，而不是内部链接。</span><span class="sxs-lookup"><span data-stu-id="23d17-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="23d17-120">目前尚不支持图片，但这在路线图中。</span><span class="sxs-lookup"><span data-stu-id="23d17-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="23d17-121">这实际上已经是太长了。</span><span class="sxs-lookup"><span data-stu-id="23d17-121">And this is really already a bit too long.</span></span> <span data-ttu-id="23d17-122">最佳实践大约为400个字符---------------------------------</span><span class="sxs-lookup"><span data-stu-id="23d17-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="23d17-123">准备好内容后，将其纳入活动分支。</span><span class="sxs-lookup"><span data-stu-id="23d17-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="23d17-124">然后，转到 " [Alchemy 合作伙伴门户](https://alchemyportal.azurewebsites.net)"，并在 "url" 字段中输入文件名。</span><span class="sxs-lookup"><span data-stu-id="23d17-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 