---
title: '与 filename 的效果相同 [RULE #-Description]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e248c2ee3cbb9a86f21c1f36be10c893df76ff52
ms.sourcegitcommit: 3070905131e6d8449981231a3551c0bb4ca38ae6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/14/2019
ms.locfileid: "30634494"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="342a5-102">必需 Alchemy 标头 H1, H2's 不起作用。</span><span class="sxs-lookup"><span data-stu-id="342a5-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="342a5-103">用于 Alchemy 创作的最佳做法和指南:</span><span class="sxs-lookup"><span data-stu-id="342a5-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="342a5-104">**不在文件夹中嵌套 Alchemy 见解**-这将断开 url 结构。</span><span class="sxs-lookup"><span data-stu-id="342a5-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="342a5-105">我们正在寻求解决此情况的情况。</span><span class="sxs-lookup"><span data-stu-id="342a5-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="342a5-106">**AlchemyInsights**文件夹中的文件应具有文件名中[Alchemy 合作伙伴门户](https://alchemyportal.azurewebsites.net)中的规则 ID 和规则名称。</span><span class="sxs-lookup"><span data-stu-id="342a5-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="342a5-107">ex.</span><span class="sxs-lookup"><span data-stu-id="342a5-107">ex.</span></span> <span data-ttu-id="342a5-108">***976-启用-保留-保留***</span><span class="sxs-lookup"><span data-stu-id="342a5-108">***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="342a5-109">将此文件顶部的元数据用作模板。</span><span class="sxs-lookup"><span data-stu-id="342a5-109">Use the metadata at the top of this file as your template.</span></span> <span data-ttu-id="342a5-110">不需要任何其他内容。</span><span class="sxs-lookup"><span data-stu-id="342a5-110">Nothing else is required.</span></span>
1. <span data-ttu-id="342a5-111">在[Alchemy 合作伙伴门户](https://alchemyportal.azurewebsites.net)中, 向下导航到 "**客户洞察力标题:** " 部分, 并将其用作洞察力的 H1 标题的起始点。</span><span class="sxs-lookup"><span data-stu-id="342a5-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="342a5-112">Alchemy 见解必须在顶部只有一个 H1, 否则它们将在生产中中断。</span><span class="sxs-lookup"><span data-stu-id="342a5-112">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="342a5-113">H2s 不呈现任何内容, 因此使用**粗体**或其他约定表示单独的节。</span><span class="sxs-lookup"><span data-stu-id="342a5-113">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="342a5-114">接下来, 使用 Alchemy 规则页面的 "客户见解" 部分中的草稿材料填写正文文本</span><span class="sxs-lookup"><span data-stu-id="342a5-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="342a5-115">项目符号列表正常</span><span class="sxs-lookup"><span data-stu-id="342a5-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="342a5-116">编号列表</span><span class="sxs-lookup"><span data-stu-id="342a5-116">Numbered lists too</span></span>
    1. <span data-ttu-id="342a5-117">**粗体**和*斜体*为-正常</span><span class="sxs-lookup"><span data-stu-id="342a5-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="342a5-118">链接应始终是 **"web 上的链接"/external**或指向**UI 元素的深层链接**, 而不是内部链接。</span><span class="sxs-lookup"><span data-stu-id="342a5-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="342a5-119">这实际上已经是太长了。</span><span class="sxs-lookup"><span data-stu-id="342a5-119">And this is really already a bit too long.</span></span> <span data-ttu-id="342a5-120">最佳实践大约为400个字符---------------------------------</span><span class="sxs-lookup"><span data-stu-id="342a5-120">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="342a5-121">准备好内容后, 将其纳入活动分支。</span><span class="sxs-lookup"><span data-stu-id="342a5-121">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="342a5-122">然后, 转到 " [Alchemy 合作伙伴门户](https://alchemyportal.azurewebsites.net)", 并在 "url" 字段中输入文件名。</span><span class="sxs-lookup"><span data-stu-id="342a5-122">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="342a5-123">确保查看并发布的见解显示 "是", 然后单击 "更新规则"。</span><span class="sxs-lookup"><span data-stu-id="342a5-123">Make sure Insight reviewed and published says "yes" and then click Update Rule.</span></span> <span data-ttu-id="342a5-124">**(这将在门户的新版本中显示 prettier-即将发布。)**
 ![url 字段](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="342a5-124">**(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

