---
title: '相同文件名是最佳 [规则 #-说明]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 278a26f4b986a85e33442baef690d3bb44462ace
ms.sourcegitcommit: 32355b76d45b730a069575efeec708149d4aeaa3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/01/2019
ms.locfileid: "29697120"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="cec0c-102">所需的 Alchemy 标头 H1、 H2 的不起作用。</span><span class="sxs-lookup"><span data-stu-id="cec0c-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="cec0c-103">最佳做法和 Alchemy 创作的指导原则：</span><span class="sxs-lookup"><span data-stu-id="cec0c-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="cec0c-p101">**不要将嵌套文件夹中的 Alchemy 见解**-这将中断的 url 结构。我们正在修复此研究。</span><span class="sxs-lookup"><span data-stu-id="cec0c-p101">**Do not nest Alchemy Insights in folders**- this will break the url structure. We're looking into fixing this.</span></span>
1. <span data-ttu-id="cec0c-106">**AlchemyInsights**文件夹中的文件应具有文件名中的规则 ID 和从[Alchemy 合作伙伴门户](https://alchemyportal.azurewebsites.net)的规则名称。</span><span class="sxs-lookup"><span data-stu-id="cec0c-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="cec0c-p102">例如***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="cec0c-p102">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="cec0c-p103">在此文件的顶部用作模板的元数据。没有任何其他是必需的。</span><span class="sxs-lookup"><span data-stu-id="cec0c-p103">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="cec0c-111">在[Alchemy 合作伙伴门户](https://alchemyportal.azurewebsites.net)中，导航到部分**客户洞察标题：** 和使用洞察您 H1 标题的为起始点。</span><span class="sxs-lookup"><span data-stu-id="cec0c-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="cec0c-p104">Alchemy 见解必须仅单个 H1 顶部或他们在生产中将中断。是使用**加粗**或以表示单独的各节其他约定，不呈现 H2s。</span><span class="sxs-lookup"><span data-stu-id="cec0c-p104">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="cec0c-114">接下来，填写 Alchemy 规则页的客户洞察力部分中使用的草稿材料的正文文本</span><span class="sxs-lookup"><span data-stu-id="cec0c-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="cec0c-115">项目符号列表都可以精细</span><span class="sxs-lookup"><span data-stu-id="cec0c-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="cec0c-116">太编号列表</span><span class="sxs-lookup"><span data-stu-id="cec0c-116">Numbered lists too</span></span>
    1. <span data-ttu-id="cec0c-117">**加粗**和*倾斜*是 a-ok</span><span class="sxs-lookup"><span data-stu-id="cec0c-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="cec0c-118">链接应始终为 **"链接到 web"/ 外部**或**深入指向 UI 元素**，不包括内部的链接。</span><span class="sxs-lookup"><span data-stu-id="cec0c-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="cec0c-p105">这是真正已有点太长。最佳做法是即将 400 个字符--</span><span class="sxs-lookup"><span data-stu-id="cec0c-p105">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="cec0c-p106">准备您的内容后，请将其拖到 live 分支。然后，转到[Alchemy 合作伙伴门户](https://alchemyportal.azurewebsites.net)url 字段中输入文件名。请确保洞察审核和发布说"是"，然后单击更新规则。**（这将看起来更加美观门户-释放提供的新版本中。）**
 ![url 字段](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="cec0c-p106">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. **(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

